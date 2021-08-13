---
title: Tipo de recurso conditionalAccessSessionControls
description: Representa um tipo complexo de controles de sessão que é imposto após a assinatura.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9d48684205582dbb59b80fd5fa7b92eee5e425871afe3a6eed32a913795513fd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229350"
---
# <a name="conditionalaccesssessioncontrols-resource-type"></a>Tipo de recurso conditionalAccessSessionControls

Namespace: microsoft.graph

Representa os controles de sessão que são imposto após a assinatura.
Todos os controles de sessão herdam [de conditionalAccessSessionControl](conditionalaccesssessioncontrol.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|applicationEnforcedRestrictions|[applicationEnforcedRestrictionsSessionControl](applicationenforcedrestrictionssessioncontrol.md)| Controle de sessão para impor restrições de aplicativo. Somente Exchange Online e o Sharepoint Online suportam esse controle de sessão. |
|cloudAppSecurity|[cloudAppSecuritySessionControl](cloudappsecuritysessioncontrol.md)| Controle de sessão para aplicar a segurança do aplicativo na nuvem.|
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
    "signInFrequency"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessSessionControls",
  "baseType": null
}-->

```json
{
  "applicationEnforcedRestrictions": {"@odata.type": "microsoft.graph.applicationEnforcedRestrictionsSessionControl"},
  "cloudAppSecurity": {"@odata.type": "microsoft.graph.cloudAppSecuritySessionControl"},
  "persistentBrowser": {"@odata.type": "microsoft.graph.persistentBrowserSessionControl"},
  "signInFrequency": {"@odata.type": "microsoft.graph.signInFrequencySessionControl"}
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

