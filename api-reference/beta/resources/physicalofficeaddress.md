---
title: Tipo de recurso physicalOfficeAddress
description: Representa o endereço comercial de um recurso, como um contato ou evento.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: dkershaw10
ms.openlocfilehash: 55faeb615225aa7c3f3f3c9babf69ad8f9952fc8acdf2d5bf9f05b1a94edc236
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54187606"
---
# <a name="physicalofficeaddress-resource-type"></a>Tipo de recurso physicalOfficeAddress

Namespace: microsoft.graph

Representa o endereço comercial de um recurso, como um contato organizacional.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|city|Cadeia de caracteres|A cidade.|
|countryOrRegion|String|O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".|
|officeLocation  | String | Office local, como construção e número de escritório para um contato organizacional.  |
|postalCode|Cadeia de caracteres|O código de endereçamento postal, ou CEP.|
|state|Cadeia de caracteres|O estado.|
|street|Cadeia de caracteres|O tipo de logradouro (rua, alameda, avenida, etc.).|

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


