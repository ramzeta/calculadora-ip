# Calculadora IP - Funciones y Lógica

Este documento describe la lógica detrás de las principales funciones de una calculadora IP.

## Funciones

### 1. Determinación de Subredes
- **Entrada**: Dirección IP y máscara de subred (o CIDR).
- **Proceso**: Operación AND bit a bit entre la dirección IP y la máscara de subred.
- **Salida**: Dirección de la subred.

### 2. Cálculo de la Dirección de Broadcast
- **Entrada**: Dirección de subred y máscara de subred.
- **Proceso**: Invertir la máscara de subred y realizar una operación OR bit a bit con la dirección de subred.
- **Salida**: Dirección de broadcast de la subred.

### 3. Análisis de Rangos de Direcciones IP
- **Entrada**: Dirección de subred y máscara de subred.
- **Proceso**: Calcular la primera y última dirección IP en la subred.
- **Salida**: Rango de direcciones IP utilizables.

### 4. Conversión entre CIDR y Máscara de Subred
- **Entrada**: Notación CIDR o máscara de subred.
- **Proceso**: Convertir CIDR a máscara o contar bits 1 en la máscara.
- **Salida**: Máscara de subred o notación CIDR.

### 5. Cálculo de Direcciones Host
- **Entrada**: Máscara de subred o CIDR.
- **Proceso**: Calcular el número de direcciones host utilizables.
- **Salida**: Número de direcciones host utilizables.

### 6. Validación de Direcciones IP
- **Entrada**: Dirección IP.
- **Proceso**: Verificar el formato y rango de cada segmento.
- **Salida**: Booleano (válida o no).

### 7. Soporte para IPv6 (Si es aplicable)
- **Entrada**: Dirección IPv6.
- **Proceso**: Adaptación de las funciones a IPv6.
- **Salida**: Depende de la función específica.

## Nota
Estos son conceptos básicos para cada función. La implementación requiere un entendimiento sólido de direcciones IP, notación CIDR, y operaciones a nivel de bits.
