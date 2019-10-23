---
title: tipo de recurso conditionalAccessSessionControls
description: Representa um tipo complexo de controles de sessão que é aplicado após a entrada.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 317120eb7c4138d955bf8a35030375180d5a1631
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638544"
---
# <a name="conditionalaccesssessioncontrols-resource-type"></a>tipo de recurso conditionalAccessSessionControls

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os controles de sessão que são aplicados após a entrada.
Todos os controles de sessão herdam de [conditionalAccessSessionControl](conditionalaccesssessioncontrol.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|applicationEnforcedRestrictions|[applicationEnforcedRestrictionsSessionControl](applicationenforcedrestrictionssessioncontrol.md)| Controle de sessão para impor restrições de aplicativo. Somente o Exchange Online e o SharePoint Online dão suporte a esse controle de sessão. |
|cloudAppSecurity|[cloudAppSecuritySessionControl](cloudappsecuritysessioncontrol.md)| Controle de sessão para aplicar o Cloud app Security.|
|persistentBrowser|[persistentBrowserSessionControl](persistentbrowsersessioncontrol.md)| Controle de sessão para definir se deseja persistir cookies ou não. Todos os aplicativos devem ser selecionados para que esse controle de sessão funcione corretamente. |
|signInFrequency|[signInFrequencySessionControl](signinfrequencysessioncontrol.md)| Controle de sessão para impor a frequência de entrada.|

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