---
title: Tipo de recurso cloudAppSecuritySessionControl
description: Controle de sessão usado para impor verificações de segurança de aplicativos na nuvem.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b1eee93b3f80b6d7d916f38d783ca94cef8e81a1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133053"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a>Tipo de recurso cloudAppSecuritySessionControl

Namespace: microsoft.graph

Controle de sessão usado para impor verificações de segurança de aplicativos na nuvem. Inehrits do [Controle de Sessão de Acesso Condicional.](conditionalaccesssessioncontrol.md)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|isEnabled     |Booliano      | Especifica se o controle de sessão está habilitado. |
|cloudAppSecurityType|String| Os valores possíveis são: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`. Para obter mais informações, [consulte Implantar o Controle de Aplicativo de Acesso Condicional para aplicativos em destaque.](/cloud-app-security/proxy-deployment-aad) |

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
