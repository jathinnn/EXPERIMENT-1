#!/usr/bin/env python3
# version1_hardcoded.py
# Predict temperature using hardcoded coefficients

def predict_temperature(a: float, b: float, c: float, t: float) -> float:
    """Quadratic temperature model: T(t) = a*t^2 + b*t + c"""
    return a * t**2 + b * t + c

def main():
    # Coefficients for the model (hardcoded)
    a = 0.5
    b = -3.0
    c = 28.0
    t = 5.0  # e.g., 5th hour/day

    T = predict_temperature(a, b, c, t)
    print(f"[Hardcoded] Predicted temperature at t={t}: {T:.2f}°C")

if __name__ == "__main__":
    main()

