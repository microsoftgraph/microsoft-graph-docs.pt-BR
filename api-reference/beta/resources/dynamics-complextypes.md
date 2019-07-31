---
title: JSON de tipos complexos
description: Tipos de dados complexos no JSON para Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: bb61450ab7f1d62d459f525f6341093f25b1686f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012636"
---
# <a name="complex-types-json"></a>JSON de tipos complexos
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

