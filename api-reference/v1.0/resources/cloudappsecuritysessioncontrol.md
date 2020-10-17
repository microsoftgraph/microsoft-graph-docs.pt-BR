---
title: tipo de recurso cloudAppSecuritySessionControl
description: Controle de sessão usado para impor verificações de segurança do aplicativo na nuvem.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 114e788e12ab8f633bc6350b08140f9d5e4fe8a3
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581264"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a>tipo de recurso cloudAppSecuritySessionControl

Namespace: microsoft.graph

Controle de sessão usado para impor verificações de segurança do aplicativo na nuvem. Inehrits do [controle de sessão de acesso condicional](conditionalaccesssessioncontrol.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|isEnabled     |Booliano      | Especifica se o controle de sessão está habilitado. |
|cloudAppSecurityType|String| Os valores possíveis são: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`. Para obter mais informações, consulte [Deploy Conditional Access app Control for refeatured apps](/cloud-app-security/proxy-deployment-aad). |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecuritySessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "cloudAppSecurityType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecuritySessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->