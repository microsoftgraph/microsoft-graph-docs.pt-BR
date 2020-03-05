---
title: tipo de recurso physicalOfficeAddress
description: Representa o endereço comercial de um recurso, como um contato ou um evento.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 24ad96681d099871f8b936308fadf04fafecb6d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521846"
---
# <a name="physicalofficeaddress-resource-type"></a>tipo de recurso physicalOfficeAddress

Namespace: Microsoft. Graph

Representa o endereço comercial de um recurso, como um contato organizacional.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|city|String|A cidade.|
|countryOrRegion|String|O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".|
|officeLocation  | String | Local do Office, como o prédio e o número do escritório de um contato organizacional.  |
|postalCode|String|O código de endereçamento postal, ou CEP.|
|state|Cadeia de caracteres|O estado.|
|street|String|O tipo de logradouro (rua, alameda, avenida, etc.).|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalOfficeAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "officeLocation": "string",
  "postalCode": "string",
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalOfficeAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
