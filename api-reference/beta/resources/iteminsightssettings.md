---
title: tipo de recurso itemInsightsSettings
description: Representa as configurações de privacidade de informações.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c84b2397c938997a3285d16612d090ae22444580
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522712"
---
# <a name="iteminsightssettings-resource-type"></a>tipo de recurso itemInsightsSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de privacidade para as [idéias](iteminsights.md) e a configuração de privacidade para as ideias de horário de reunião. Use esta API para desabilitar/habilitar o cálculo e a visibilidade de insights de itens e de horas de reunião. 

- Insights de item: calcula a relação entre usuários e itens, como documentos ou sites no Microsoft 365.  
- Observações de horário de reunião: calcula as horas de reunião de calendário de uma pessoa com base nas atividades no Word, Excel, PowerPoint, email e calendário do Outlook no Microsoft 365.

> [!NOTE]
> Horas de reunião as ideias estão implantando para clientes que começam de novembro de 2020. 

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [Get](../api/iteminsightssettings-get.md)| [itemInsightsSettings](iteminsightssettings.md) | Ler as propriedades de um objeto **itemInsightsSettings** . |
| [Update](../api/iteminsightssettings-update.md)| [itemInsightsSettings](iteminsightssettings.md) | Atualize um objeto **itemInsightsSettings** .|


## <a name="properties"></a>Propriedades
| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|isEnabledInOrganization|Boolean| `true` Se o item de organização insights estiver habilitado; `false` se o item de organização insights estiver desabilitado para todos os usuários sem exceções. O padrão é `true`. Opcional.|
|disabledForGroup|String| A ID de um grupo do Azure AD, do qual as insights do item dos membros estão desabilitadas. O padrão é `empty`. Opcional.|

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


