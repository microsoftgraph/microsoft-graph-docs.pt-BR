---
title: Tipo de recurso userInsightsSettings
description: Representa as configurações de privacidade do usuário para insights de item e informações de horários de reunião.
ms.localizationpriority: medium
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 723f1ca8d0a56116039ae3f85eb0d534c3525972
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780888"
---
# <a name="userinsightssettings-resource-type"></a>Tipo de recurso userInsightsSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de privacidade do usuário [para o itemInsights](iteminsights.md) e informações sobre horários [de reunião.](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) Use esse recurso para desabilitar/habilitar o cálculo e a visibilidade das percepções do item e dos horários de reunião de um usuário. 

- Insights de item: calcula a relação entre usuários e itens, como documentos ou sites em Microsoft 365.  
- Insights do horário de reunião: calcula o horário de reunião do calendário de uma pessoa com base nas atividades no Word, Excel, PowerPoint, email e Outlook calendário no Microsoft 365.

Use o [recurso insightsSettings](insightssettings.md) para desabilitar/habilitar o cálculo e a visibilidade de insights de itens, insights de horas de reunião ou informações de pessoas em um nível de organização.

## <a name="methods"></a>Métodos

| Método                                                 | Tipo de retorno                                                   | Descrição                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [Get](../api/userinsightssettings-get.md)       | [userInsightsSettings](userinsightssettings.md) | Leia as propriedades de **um objeto userinsightssettings.**  |
| [Atualizar](../api/userinsightssettings-update.md) | [userInsightsSettings](userinsightssettings.md) | Atualize as propriedades de **um objeto userinsightssettings.** |

## <a name="properties"></a>Propriedades
| Propriedade                   | Tipo                                                  | Descrição                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| isEnabled     | Booliano  |  `true` se os insights **de item do usuárioInsights** e de horas de reunião estão habilitados; `false` se o item do **usuárioInights** e as percepções do horário de reunião estão desabilitados. O padrão é `true`. Opcional.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.userInsightsSettings"
}-->

```json
{
  "isEnabled": "Boolean"
}
```


