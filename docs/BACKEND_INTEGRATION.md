# Backend Integration Checklist

The mobile UI is functional, but the following production services are currently demo flows or placeholders.

## Authentication and identity

- Mobile OTP provider
- User authentication/session API
- Optional Aadhaar/identity verification workflow
- Secure token refresh and logout

## Property and land data

- Property listing/detail APIs
- Wishlist persistence
- Land/revenue record provider
- Court case search service
- Khata/Khasra/Tehsil/District master data

## Documents and reports

- Secure document upload
- AI Land Report generation
- Report status updates
- Report download/storage
- Blockchain validation or registry status where applicable

## Commercial services

- Service catalog/pricing API
- Cart/request API
- GST/tax values from backend
- Razorpay or chosen payment gateway
- Backend payment verification
- Order history API

## Maps and visits

- Maps provider/API key
- Property coordinates
- Site-visit booking API
- Owner/contact workflow

## Security rules

- Never place private API secrets in the mobile app.
- `EXPO_PUBLIC_*` values are visible to clients and must be publishable.
- Payment signatures, OTP credentials, database credentials, blockchain private keys, and service-account credentials belong only on the backend.
- The production API must independently validate every client request.
