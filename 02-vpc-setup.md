# VPC & Networking Setup

## Corporate VPC

1. Navigate to the VPC Dashboard.
2. Click `Create VPC`.
3. **Name tag**: `Corp_Main_VPC`
4. **Description**: "Main VPC for corporate network."
5. CIDR Block: `10.0.0.0/16`
6. Tenancy: Default
7. IPv6 CIDR Block: Assign it according to your requirements.
8. Service Endpoints: Select any required AWS services.
9. Click `Create`.

## Subnets
Every subnet you create should be linked to your VPC. Here are detailed steps for each:

### VPN Subnet:

1. Click `Subnets`, then `Create subnet`.
2. **VPC**: Select `Corp_Main_VPC`.
3. **Name tag**: `Corp_VPN_Sub`
4. **Description**: "Subnet for VPN connections."
5. CIDR Block: `10.0.1.0/24`
6. Availability Zone: Select based on preference (e.g., us-east-1a).
7. IPv6 CIDR Block: Assign if required.
8. Click `Create`.

### Application Server Subnet:

1. Click `Subnets`, then `Create subnet`.
2. **VPC**: Select `Corp_Main_VPC`.
3. **Name tag**: `Corp_AppServer_Sub`
4. **Description**: "Subnet for application servers."
5. CIDR Block: `10.0.2.0/24`
6. Availability Zone: Select another one for high availability (e.g., us-east-1b).
7. Click `Create`.

### Web Server Subnet:

1. Click `Subnets`, then `Create subnet`.
2. **VPC**: Select `Corp_Main_VPC`.
3. **Name tag**: `Corp_WebServer_Sub`
4. **Description**: "Subnet for web servers."
5. CIDR Block: `10.0.3.0/24`
6. Availability Zone: (e.g., us-east-1c).
7. Click `Create`.

### Database Server Subnet:

1. Click `Subnets`, then `Create subnet`.
2. **VPC**: Select `Corp_Main_VPC`.
3. **Name tag**: `Corp_DbServer_Sub`
4. **Description**: "Subnet for database servers."
5. CIDR Block: `10.0.4.0/24`
6. Availability Zone: (e.g., us-east-1d).
7. Click `Create`.

### Build Environment Subnet:

1. Click `Subnets`, then `Create subnet`.
2. **VPC**: Select `Corp_Main_VPC`.
3. **Name tag**: `Corp_BuildEnv_Sub`
4. **Description**: "Subnet for build environment."
5. CIDR Block: `10.0.5.0/24`
6. Availability Zone: (e.g., us-east-1a).
7. Click `Create`.

... (If you have more subnets, continue with the same method)
