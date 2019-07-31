---
title: tipo de recurso bookingNamedEntity
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 7eba40effa1ef5107a97e2acd075dad0c5e350f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013098"
---
# <a name="bookingnamedentity-resource-type"></a>tipo de recurso bookingNamedEntity

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Este é um tipo base para entidades de livros da Microsoft que fornecem um nome de exibição, por exemplo, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|String|Um nome para a entidade derivada, que faz interface com clientes.|
|id|String| A ID da entidade derivada. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingNamedEntity"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingNamedEntity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
