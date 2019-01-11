---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: 179c0bb1e5c82d7f2af17dcbcae08be8726f2ecd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888932"
---
# <a name="currencycolumn-resource-type"></a>Tipo de recurso CurrencyColumn

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

**currencyColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna representam moeda.

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **currencyColumn**.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição
|:--------------|:-------|:----------------------------------------------------
| **locale**    | string | Especifica a localidade da qual o símbolo de moeda deverá ser inferido.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
