# Project Flow

## Main User Flow

1. Resident opens the Pole Map
2. Resident selects a pole
3. Resident submits a Quick Report
4. Complaint is stored in Room Database
5. Repair Tracker shows the complaint status
6. Panchayat admin unlocks Panchayat Mode using the PIN
7. Panchayat admin assigns or fixes the complaint
8. Energy Saved screen updates for fixed `Burning in Day` issues

## Offline-First Behavior

- Reports are written to Room Database first
- Sync status starts as `Pending`
- Firebase sync runs only when internet and Firebase configuration are available
- Local Room data remains the working source of truth

## Main Modules

- **Pole Map**: shows ward-wise pole status
- **Quick Report**: captures `Working`, `Fused`, or `Burning in Day`
- **Repair Tracker**: tracks complaint progress
- **Panchayat Mode**: protected admin workflow
- **Energy Saved**: shows saved kWh and approximate INR impact
- **Settings**: manages theme and sync display
- **GenAI Summary**: shows summary with fallback logic
