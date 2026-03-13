def vertical_position(v_vertical, time): #defines the fuction and variables
    message=int(v_vertical * time - 0.5 * 9.8 * (time ** 2)) #the function
    return message #out put of the fuction

def burnout_velocity(acceleration , burn_time):
    mess4 = float(acceleration * burn_time)
    return mess4
def range_distance(v_horizontal , total_flight_time):
    mess5 = float(v_horizontal * total_flight_time)
    return mess5
from math import sqrt
def time_to_apogee(v_vertical, g):
    message = int(v_vertical / g)
    return message

def time_fall(apogee, g):
    message2 = int(sqrt((2 * apogee) / g))
    return message2

def total_flight_time(burn_time, time_to_apogee1, time_fall):
    message3 = int(burn_time) + int(time_to_apogee1) + int(time_fall)
    return message3

#time_to_apogee = v_vertical / g

#time_fall = sqrt((2 * apogee) / g)
#total_flight_time = burn_time + time_to_apogee + time_fall

#range_distance = v_horizontal * total_flight_time

import numpy as np
from math import sin
def newApogee(vertVelocity, horzVelocity, boVelocity, boHeight):
    g = 9.8
    burnout_angle = np.arctan2(vertVelocity,horzVelocity)
    height_after_thrust = ((boVelocity**2)*(sin(burnout_angle))**2)/(2*g)
    apogeeis = boHeight + height_after_thrust
    return apogeeis


def bheight(accel, burn_t):
    burnoutHeight = 0.5*accel*(burn_t**2)
    return burnoutHeight

import matplotlib.pyplot as plt
def trajectory(px,py):
    plt.figure(num=0, figsize=(10,6))
    plt.plot(px,py, color='blue', linewidth=5, label='Trajectory')
    plt.xlabel('Horizontal Position (m)')
    plt.ylabel('Vertical Position (m)')
    plt.title('Rocket Trajectory')
    plt.grid(True)
    plt.axis('equal')
    plt.legend()
    plt.show()
