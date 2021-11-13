---
title: Tipo de recurso itemInsightsSettings
description: Representa configurações de privacidade para itemInsights.
ms.localizationpriority: medium
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 764e47071d0f7554e3bcdd2c5ce4350304bdd6fe
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2021
ms.locfileid: "60891215"
---
# <a name="iteminsightssettings-resource-type"></a>Tipo de recurso itemInsightsSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa configurações de privacidade para [itemInsights](iteminsights.md) e configuração de privacidade para insights [de horário de reunião.](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) Use essa API para desabilitar/habilitar o cálculo e a visibilidade das percepções do item e dos horários de reunião. 

- Insights de item: calcula a relação entre usuários e itens, como documentos ou sites em Microsoft 365.  
- Insights do horário de reunião: calcula o horário de reunião do calendário de uma pessoa com base nas atividades no Word, Excel, PowerPoint, email e Outlook calendário no Microsoft 365.

Use o [recurso userInsightsSettings](userinsightssettings.md) para desabilitar/habilitar o cálculo e a visibilidade das percepções do item e dos insights do horário de reunião de um usuário.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [Get](../api/iteminsightssettings-get.md)| [itemInsightsSettings](iteminsightssettings.md) | Leia as propriedades de um **objeto itemInsightsSettings.** |
| [Atualizar](../api/iteminsightssettings-update.md)| [itemInsightsSettings](iteminsightssettings.md) | Atualizar um **objeto itemInsightsSettings.**|


## <a name="properties"></a>Propriedades
| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|isEnabledInOrganization|Boolean| `true` se as percepções do item da organização estão habilitadas; `false` se as percepções do item da organização estão desabilitadas para todos os usuários sem exceções. O padrão é `true`. Opcional.|
|disabledForGroup|Cadeia de Caracteres| A ID de um grupo do Azure AD, do qual as informações do item dos membros estão desabilitadas. O padrão é `empty`. Opcional.|

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


