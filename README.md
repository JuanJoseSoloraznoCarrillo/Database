# DW_Planta Database

## Overview

This project contains the SQL script to create the `DW_Planta` database and its associated tables. The `DW_Planta` database is designed for data warehousing purposes, storing information about clients, products, branches, time, vendors, and sales.

## Description

The script `DW_Plants.sql` creates the `DW_Planta` database, sets various database options, and defines the schema for the following tables:
- `D_CLIENTE`: Stores client information.
- `D_PRODUCTO`: Stores product information.
- `D_SUCURSAL`: Stores branch information.
- `D_TIEMPO`: Stores time information.
- `D_VENDEDOR`: Stores vendor information.
- `H_VENTAS`: Stores sales transactions.

## Usage

1. Open SQL Server Management Studio (SSMS).
2. Connect to your SQL Server instance.
3. Open the `DW_Plants.sql` script file.
4. Execute the script to create the `DW_Planta` database and its tables.

## Tables

### D_CLIENTE

Stores client information.

| Column          | Data Type   | Description          |
|-----------------|-------------|----------------------|
| `id_cliente`    | `nvarchar`  | Client ID (Primary Key) |
| `nombre_cliente`| `nvarchar`  | Client name          |
| `edad`          | `int`       | Client age           |
| `estado_civil`  | `nvarchar`  | Marital status       |

### D_PRODUCTO

Stores product information.

| Column            | Data Type   | Description          |
|-------------------|-------------|----------------------|
| `id_producto`     | `nvarchar`  | Product ID (Primary Key) |
| `nombre_producto` | `nvarchar`  | Product name         |
| `familia_producto`| `nvarchar`  | Product family       |

### D_SUCURSAL

Stores branch information.

| Column            | Data Type   | Description          |
|-------------------|-------------|----------------------|
| `id_sucursal`     | `int`       | Branch ID (Primary Key) |
| `nombre_sucursal` | `nvarchar`  | Branch name          |
| `nombre_ciudad`   | `nvarchar`  | City name            |

### D_TIEMPO

Stores time information.

| Column            | Data Type   | Description          |
|-------------------|-------------|----------------------|
| `id_tiempo`       | `nvarchar`  | Time ID (Primary Key) |
| `mes`             | `int`       | Month                |
| `ano`             | `int`       | Year                 |

### D_VENDEDOR

Stores vendor information.

| Column            | Data Type   | Description          |
|-------------------|-------------|----------------------|
| `id_vendedor`     | `int`       | Vendor ID (Primary Key) |
| `nombre_vendedor` | `nvarchar`  | Vendor name          |
| `tipo_capacitacion`| `nvarchar` | Training type        |
| `hora_capacitacion`| `int`      | Training hours       |

### H_VENTAS

Stores sales transactions.

| Column            | Data Type   | Description          |
|-------------------|-------------|----------------------|
| `id_venta`        | `int`       | Sale ID (Primary Key, Identity) |
| `id_producto`     | `nvarchar`  | Product ID           |
| `id_sucursal`     | `int`       | Branch ID            |
| `id_cliente`      | `nvarchar`  | Client ID            |
| `id_vendedor`     | `int`       | Vendor ID            |
| `id_tiempo`       | `nvarchar`  | Time ID              |
| `cantidad_venta`  | `int`       | Sale quantity        |
| `monto_venta`     | `int`       | Sale amount          |

## Contact

For any questions or inquiries, please contact Juan Jose Solorzano at [juanjose.solorzano.c@gmail.com](mailto:juanjose.solorzano.c@gmail.com).