---
title: tipo de recurso bookingCurrency
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: c1d56dde0c239245f6724040229df7d417a79613
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508000"
---
# <a name="bookingcurrency-resource-type"></a>tipo de recurso bookingCurrency

Namespace: Microsoft. Graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa uma moeda monetária suportada por um [bookingBusiness](bookingbusiness.md).


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar bookingCurrencies](../api/bookingcurrency-list.md) | coleção [bookingCurrency](bookingcurrency.md) |Obtenha uma lista de objetos **bookingCurrency** disponíveis para uma empresa de livros da Microsoft.|
|[Obter bookingCurrency](../api/bookingcurrency-get.md) | [bookingCurrency](bookingcurrency.md) |Obter as propriedades de um objeto **bookingCurrency** .|


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Um código de moeda de 3 caracteres, com base na [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html). Por exemplo, o código de moeda dos Dólar dos EUA é USD, e para o dólar australiano é AUD. Somente leitura.|
|formato|String| O símbolo da moeda. Por exemplo, o símbolo de moeda dos dólar americano e para o dólar australiano é $.  |

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
