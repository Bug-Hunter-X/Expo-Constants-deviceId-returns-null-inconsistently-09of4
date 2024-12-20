# Expo Constants.deviceId Returns Null Inconsistent

This repository demonstrates a bug in Expo where `Constants.deviceId` sometimes returns `null` unexpectedly.  The issue impacts applications requiring unique device identifiers for functionality like user authentication or analytics.  The provided code examples showcase the problem and a potential workaround.

## Problem

The `Constants.deviceId` API in Expo is intended to provide a unique identifier for each device. However, under certain conditions (still under investigation), the API returns `null`, leading to unexpected behavior and data inconsistencies.

## Solution

The solution provided involves checking for `null` and providing an alternative fallback mechanism.  This is not an ideal solution, as it relies on generating IDs client-side. Ideally, Expo should provide a more reliable method for obtaining a stable device ID.  Contributions are welcome to further investigate the root cause and find a more robust solution.