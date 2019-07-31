---
title: tipo de recurso bookingPerson
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 3c8db7aca957878247193207e00e969d8ddfc98e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974161"
---
# <a name="bookingperson-resource-type"></a>tipo de recurso bookingPerson

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Este é um tipo base para uma pessoa em um Microsoft bookings Business, que pode ser um [bookingCustomer](bookingcustomer.md) ou [bookingStaffMember](bookingstaffmember.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|Cadeia de caracteres|Um nome para a entidade derivada, que faz interface com clientes.|
|emailAddress|String|O endereço de email da pessoa.|
|id|String| A ID da entidade derivada. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingPerson"
}-->

```json
{
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
