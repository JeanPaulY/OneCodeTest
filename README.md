# OneCodeTest

#Coded this in my CSCI 151 at Highline College

#pragma once
#include <iostream>
#include <string>

class Car {
public:
	Car(std::string vin, float price);
	bool operator<(const Car& rhs);
	std::string vin() const;
	float price() const;
private:
	std::string _vin;
	float _price;
};
std::ostream& operator<<(std::ostream& out, const Car& car);
