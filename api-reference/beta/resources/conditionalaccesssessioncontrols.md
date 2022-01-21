---
title: Tipo de recurso conditionalAccessSessionControls
description: Representa um tipo complexo de controles de sessão que é imposto após a assinatura.
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c60d87cfab617bea22df27e8a289e90fb889b78a
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161618"
---
# <a name="conditionalaccesssessioncontrols-resource-type"></a>Tipo de recurso conditionalAccessSessionControls

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os controles de sessão que são imposto após a assinatura.
Todos os controles de sessão herdam [de conditionalAccessSessionControl](conditionalaccesssessioncontrol.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|applicationEnforcedRestrictions|[applicationEnforcedRestrictionsSessionControl](applicationenforcedrestrictionssessioncontrol.md)| Controle de sessão para impor restrições de aplicativo. Somente Exchange Online e o Sharepoint Online suportam esse controle de sessão. |
|cloudAppSecurity|[cloudAppSecuritySessionControl](cloudappsecuritysessioncontrol.md)| Controle de sessão para aplicar a segurança do aplicativo na nuvem.|
|continuousAccessEvaluation|[continuousAccessEvaluationSessionControl](../resources/continuousaccessevaluationsessioncontrol.md)|Controle de sessão para configurações de avaliação de acesso contínuo.|
|disableResilienceDefaults|Booliano| Controle de sessão que determina se é aceitável para o Azure AD estender sessões existentes com base nas informações coletadas antes de uma paralisação ou não.|
|persistentBrowser|[persistentBrowserSessionControl](persistentbrowsersessioncontrol.md)| Controle de sessão para definir se os cookies serão persistentes ou não. Todos os aplicativos devem ser selecionados para que esse controle de sessão funcione corretamente. |
|signInFrequency|[signInFrequencySessionControl](signinfrequencysessioncontrol.md)| Controle de sessão para impor a frequência de signin.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "applicationEnforcedRestrictions",
    "persistentBrowser",
    "cloudAppSecurity",
    "signInFrequency",
    "continuousAccessEvaluation",
    "disableResilienceDefaults"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessSessionControls",
  "baseType": null
}-->

```json
{
  "applicationEnforcedRestrictions": {"@odata.type": "microsoft.graph.applicationEnforcedRestrictionsSessionControl"},
  "cloudAppSecurity": {"@odata.type": "microsoft.graph.cloudAppSecuritySessionControl"},
  "continuousAccessEvaluation": {"@odata.type": "microsoft.graph.continuousAccessEvaluationSessionControl"},
  "persistentBrowser": {"@odata.type": "microsoft.graph.persistentBrowserSessionControl"},
  "signInFrequency": {"@odata.type": "microsoft.graph.signInFrequencySessionControl"},
  "disableResilienceDefaults": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessSessionControls resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

