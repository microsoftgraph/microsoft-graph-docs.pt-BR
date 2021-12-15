---
title: Tipo de recurso bookingCurrency
description: Representa uma moeda monetária suportada por um bookingBusiness.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 47cddfdf3a127941414ceaccba500d4bba357aa3
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524991"
---
# <a name="bookingcurrency-resource-type"></a>Tipo de recurso bookingCurrency

Namespace: microsoft.graph

Representa uma moeda monetária suportada por [um bookingBusiness](bookingbusiness.md).


## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar bookingCurrencies](../api/bookingcurrency-list.md) | [coleção bookingCurrency](bookingcurrency.md) |Obter uma lista de **objetos bookingCurrency** disponíveis para uma empresa do Microsoft Bookings.|
|[Obter bookingCurrency](../api/bookingcurrency-get.md) | [bookingCurrency](bookingcurrency.md) |Obter as propriedades de um **objeto bookingCurrency.**|


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres| Um código de moeda de 3 caracteres, com base na [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html). Por exemplo, o código de moeda para o dólar americano é USD e para o dólar australiano é AUD. Somente leitura.|
|symbol|Cadeia de caracteres| O símbolo da moeda. Por exemplo, o símbolo de moeda para o dólar americano e para o dólar australiano é $.  |

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCurrency"
}-->

```json
{
  "id": "String (identifier)",
  "symbol": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingCurrency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


