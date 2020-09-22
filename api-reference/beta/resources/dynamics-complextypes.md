---
title: JSON de tipos complexos
description: Tipos de dados complexos no JSON para Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 77d2f7c5c491bf6e86a6df1a05b4a1cdd7788187
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040056"
---
# <a name="complex-types-json"></a>JSON de tipos complexos

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Estes são os vários tipos complexos no Dynamics 365 Business central. Você pode ver o uso desses tipos complexos nos vários métodos individuais que fazem uso deles.

## <a name="postal-address"></a>Endereço postal

Representa um tipo complexo de endereço postal no Dynamics 365 Business central.

### <a name="properties"></a>Propriedades
| Propriedade     | Tipo       |Descrição             |
|:-------------|:---------|:-----------------------|
|street        |string    |Rua do endereço postal.  |
|city          |string    |Cidade do endereço postal.    |
|estado         |string    |Estado do endereço postal.   |
|countryLetterCode|string |Código postal carta de país (palavra de dois caracteres)|
|postalCode    |string    |Código de post de endereço postal|

```json
"PostalAddress" 
{ 
"street": "string",
"city": "string", 
"state": "string", 
"countryLetterCode": "string", 
"postalCode": "string" 
} 
 ```



