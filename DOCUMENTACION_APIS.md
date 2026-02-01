# Documentación Técnica de APIs - Zapatillas JyR

Esta documentación describe los servicios web desarrollados para la plataforma "Zapatillas JyR".

## 1. Introducción
La API ha sido construida utilizando **FastAPI**, lo que permite una documentación interactiva automática a través de Swagger UI.

## 2. Especificación de Endpoints

### Módulo de Productos
| Endpoint | Método | Descripción | Parámetros |
| :--- | :--- | :--- | :--- |
| `/products` | GET | Obtiene el catálogo completo. | Ninguno |
| `/products` | POST | Crea un nuevo producto. | JSON (ProductCreate) |

### Módulo de Usuarios
| Endpoint | Método | Descripción | Parámetros |
| :--- | :--- | :--- | :--- |
| `/users/register` | POST | Registra un nuevo usuario. | JSON (UserCreate) |

### Módulo de Pedidos
| Endpoint | Método | Descripción | Parámetros |
| :--- | :--- | :--- | :--- |
| `/orders` | POST | Genera una orden de compra. | JSON (OrderCreate), user_id |

## 3. Acceso a Documentación Interactiva
Una vez ejecutado el servidor, la documentación detallada (OpenAPI) está disponible en:
- **Swagger UI:** `http://localhost:8000/docs`
- **ReDoc:** `http://localhost:8000/redoc`
