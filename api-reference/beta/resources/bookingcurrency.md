---
title: tipo de recurso de bookingCurrency
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: a68b88160e42217f3605c4a4bb30f692e8dafc06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034591"
---
# <a name="bookingcurrency-resource-type"></a>tipo de recurso de bookingCurrency

 > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.
 
Representa uma moeda monetária compatíveis com uma [bookingBusiness](bookingbusiness.md).


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Lista bookingCurrencies](../api/bookingcurrency-list.md) | coleção [bookingCurrency](bookingcurrency.md) |Obtenha uma lista de objetos de **bookingCurrency** disponíveis para uma empresa Microsoft Bookings.|
|[Obter bookingCurrency](../api/bookingcurrency-get.md) | [bookingCurrency](bookingcurrency.md) |Obtenha as propriedades de um objeto **bookingCurrency** .|


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Um código de moeda de 3 caracteres, com base em [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html). Por exemplo, o código de moeda para o dólar americano é USD e para o Dólar australiano é AUD. Somente leitura.|
|símbolo|String| O símbolo da moeda. Por exemplo, o símbolo de moeda para o dólar americano e para o Dólar australiano é $.  |

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingCurrency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->