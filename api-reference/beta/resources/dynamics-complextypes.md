---
title: JSON de tipos complexos
description: Tipos de dados complexos no JSON para Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4fc4d4f53014f5b8c656cd069cadf7b19190e0f0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543159"
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

