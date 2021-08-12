---
title: Tipo de recurso cloudAppSecuritySessionControl
description: Controle de sessão usado para impor verificações de segurança do aplicativo na nuvem.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7ba9d84a10ac25275abffd6c922286c010f02a042c5377f3f43b9f26e55be71a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54243613"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a>Tipo de recurso cloudAppSecuritySessionControl

Namespace: microsoft.graph

Controle de sessão usado para impor verificações de segurança do aplicativo na nuvem. Inehrits do Controle de Sessão [de Acesso Condicional](conditionalaccesssessioncontrol.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|isEnabled     |Booliano      | Especifica se o controle de sessão está habilitado. |
|cloudAppSecurityType|cloudAppSecuritySessionControlType| Os valores possíveis são: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`. Para obter mais informações, [consulte Deploy Conditional Access App Control for featured apps](/cloud-app-security/proxy-deployment-aad). |

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
