---
title: tipo de recurso itemInsightsSettings
description: Representa as configurações de privacidade de informações.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5d05a9fdf3a901fcddd55207bec373a3a0736afa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089326"
---
# <a name="iteminsightssettings-resource-type"></a>tipo de recurso itemInsightsSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de [privacidade para os](iteminsights.md)itens que configuram a visibilidade de insights derivadas do Microsoft Graph, entre usuários e outros itens (como documentos ou sites) no Microsoft 365.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [Get](../api/iteminsightssettings-get.md)| [itemInsightsSettings](iteminsightssettings.md) | Ler as propriedades de um objeto **itemInsightsSettings** . |
| [Update](../api/iteminsightssettings-update.md)| [itemInsightsSettings](iteminsightssettings.md) | Atualize um objeto **itemInsightsSettings** .|


## <a name="properties"></a>Propriedades
| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|isEnabledInOrganization|Boolean| `true` Se o item de organização insights estiver habilitado; `false` se o item de organização insights estiver desabilitado para todos os usuários sem exceções. O padrão é `true`. Opcional.|
|disabledForGroup|Cadeia de caracteres| A ID de um grupo do Azure AD, do qual as insights do item dos membros estão desabilitadas. O padrão é `empty`. Opcional.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso
<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.itemInsightsSettings"
}-->

```json
{
  "isEnabledInOrganization": "Boolean",
  "disabledForGroup": "String"
}
```


