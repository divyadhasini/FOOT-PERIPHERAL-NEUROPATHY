# FOOT-PERIPHERAL-NEUROPATHY
Foot Peripheral Neuropathy reduces sensation in the feet, making injuries and ulcers difficult to detect. Our AI-powered system monitors foot pressure, temperature, gait, and vibration to identify abnormalities, assess neuropathy and ulcer risk, and provide real-time alerts for early intervention and preventive care.
# Foot Peripheral Neuropathy Monitoring & Early Warning System

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python Version](https://img.shields.io/badge/python-3.10%2B-blue.svg)](https://www.python.org/)
[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)]()
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

An end-to-end AI/IoT monitoring system for continuous tracking of plantar pressure, localized skin temperature, gait dynamics, and vibration perception thresholds. Designed to predict Diabetic Foot Ulcer (DFU) risks and enable proactive clinical intervention for patients suffering from Peripheral Neuropathy.

---

## Problem Overview

Peripheral Neuropathy impairs peripheral sensory nerve function in the feet, significantly diminishing a patient's ability to detect pain, pressure micro-traumas, or thermal injuries. 

* **The Clinical Gap:** Unnoticed tissue damage and friction leads to subcutaneous inflammation, tissue necrosis, and full-thickness plantar ulcers.
* **The Solution:** Continuous multi-sensor tracking via smart insoles paired with an On-Device & Cloud AI pipeline that computes real-time **Ulcer Risk Scores (URS)** and alerts healthcare providers and patients prior to skin breakdown.

---

## Key Features

* **Multi-Modal Data Acquisition:**
  * **Plantar Pressure Mapping:** High-density piezoresistive array tracks peak focal pressure and spatial load redistribution.
  * **Thermal Asymmetry Detection:** Dual-foot differential IR temperature sensors flag localized hyperthermia ($\Delta T > 2.2^\circ\text{C}$ clinical threshold).
  * **Gait & Dynamic Stability:** 6-axis IMU (Accelerometer + Gyroscope) captures stride asymmetry, foot-drop, stance duration, and cadence variability.
  * **Vibration Perception Threshold (VPT):** Micro-vibrational feedback routines to assess tactile loss over time.
* **Edge & Cloud AI Analytics:**
  * **Edge Inference:** On-device low-latency detection of dangerous pressure-duration thresholds ($P \times \Delta t$).
  * **Cloud ML Risk Engine:** Time-series transformer/LSTM models predicting 7-day ulceration probability.
* **Real-Time Alert System:** Multi-channel alerting (Push Notifications, SMS, Clinician Dashboard) triggered on critical anomalies.

---
