---
title: Tipo de recurso insightsSettings
description: Representa as configurações de privacidade para informações.
ms.localizationpriority: medium
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 61625b4d9309ca203d1d523f1fcdb4f0fe6c583f
ms.sourcegitcommit: 0fa7148e0b776663eaca3e79e72b85046d4b8b1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/15/2022
ms.locfileid: "63500886"
---
# <a name="insightssettings-resource-type"></a>Tipo de recurso insightsSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa _configurações para_ calcular e gerenciar o retorno de exibição ou programática de um tipo específico de insights em uma organização. As percepções podem ser insights de item, insights de horas de reunião ou percepções de pessoas. 

Insights de itens [e informações de horas](https://support.microsoft.com/office/suggested-meeting-hours-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) de reunião representam relações entre usuários e itens, como documentos, sites e outros tipos de conteúdo em Microsoft 365. Programaticamente, eles são representados pelo [recurso itemInsights](iteminsights.md) . Você pode obter documentos [compartilhados com](../api/insights-list-shared.md) um usuário, [com tendências](../api/insights-list-trending.md) ao redor de um usuário ou [usados](../api/insights-list-used.md) por um usuário. Você pode usar **insightsSettings** para personalizar as configurações de privacidade para calcular [, exibir ou retornar insights de item em uma organização](/graph/insights-customize-item-insights-privacy).

As percepções de pessoas representam conexões de pessoas que são relevantes ou trabalham umas com as outras com base em suas relações públicas. Programaticamente, as pessoas individuais são representadas pelo [recurso pessoa](person.md) . Você pode [usar a API de pessoas para obter informações das pessoas](/graph/people-example). Você pode usar **insightsSettings** para personalizar [as configurações de privacidade para exibir ou retornar informações de pessoas](/graph/insights-customize-people-insights-privacy).

Por outro lado, para insights de item e de horas de [reunião, você](https://support.microsoft.com/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) também pode gerenciar o cálculo _e a_ visibilidade em um nível de usuário usando o [recurso userInsightsSettings](userinsightssettings.md) .

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Item de listaInsights](../api/organizationsettings-list-iteminsights.md) | [insightsSettings](insightssettings.md) | Obter as _configurações em_ um [objeto insightsSettings](insightssettings.md) para exibir insights de item em uma organização. |
| [Listar peopleInsights](../api/organizationsettings-list-peopleinsights.md) | [insightsSettings](insightssettings.md) | Obter as _configurações em_ um [objeto insightsSettings](insightssettings.md) para exibir informações de pessoas em uma organização. |
| [Atualizar insightsSettings](../api/insightssettings-update.md) | [insightsSettings](insightssettings.md) | Atualize as propriedades de um **recurso insightsSettings** para gerenciar a exibição ou o retorno do tipo especificado de insights, que podem ser insights de item ou informações de pessoas. |


## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|isEnabledInOrganization|Booliano| `true` se o tipo especificado de insights estiver habilitado para a organização; `false` se o tipo especificado de insights estiver desabilitado para todos os usuários sem exceções. O padrão é `true`. Opcional.|
|disabledForGroup|Cadeia de caracteres| A ID de um grupo Azure Active Directory, do qual o tipo especificado de insights está desabilitado para seus membros. O padrão é `empty`. Opcional.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.insightsSettings"
}-->

```json
{
  "disabledForGroup": "String",
  "isEnabledInOrganization": "Boolean"
}
```





