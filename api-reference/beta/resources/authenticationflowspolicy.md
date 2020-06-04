---
title: tipo de recurso authenticationFlowsPolicy
description: 'Representa a configuração de política da experiência de inscrição de autoatendimento em um nível de locatário que permite aos usuários externos solicitar a inscrição para aprovação. '
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 263b92c081545fc3ce337d25b4813d85fe034940
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556382"
---
# <a name="authenticationflowspolicy-resource-type"></a>tipo de recurso authenticationFlowsPolicy


Namespace: microsoft.graph

Representa a [configuração de política da experiência de inscrição de autoatendimento](../resources/selfservicesignupauthenticationflowconfiguration.md) em um nível de locatário que permite aos usuários externos solicitar a inscrição para aprovação. Ele contém informações sobre a ID, o nome para exibição e a descrição e indica se a inscrição de autoatendimento está habilitada para a política.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:-------|:---|:----------|
|id|String| Propriedade Inherited. A ID da política de fluxos de autenticação. Opcional. Somente leitura.
|displayName|Cadeia de caracteres| Propriedade Inherited. O nome legível da política. Esta propriedade não é uma chave. Opcional. Somente leitura.|
|description|String|Propriedade Inherited. Uma descrição da política. Esta propriedade não é uma chave. Opcional. Somente leitura.|
|selfServiceSignUp|[selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) |Contém configurações do [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) que transmitem se a inscrição de autoatendimento está habilitada ou desabilitada. Esta propriedade não é uma chave. Opcional. Somente leitura. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationFlowsPolicy",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "selfServiceSignUp": {
    "@odata.type": "#microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
  },
}
```
