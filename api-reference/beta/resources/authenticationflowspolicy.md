---
title: Tipo de recurso authenticationFlowsPolicy
description: 'Representa a configuração da política da experiência de inscrição de autoatendimento no nível do locatário que permite aos usuários externos solicitar a inscrição para a aprovação. '
author: linkhp
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1113836041f4faa89a356811e38d2ef3ac70fef4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433156"
---
# <a name="authenticationflowspolicy-resource-type"></a>Tipo de recurso authenticationFlowsPolicy


Namespace: microsoft.graph

Representa a [configuração da política da experiência de inscrição de autoatendimento](../resources/selfservicesignupauthenticationflowconfiguration.md) no nível do locatário que permite aos usuários externos solicitar a inscrição para a aprovação. Ela contém informações sobre a ID, o nome de exibição e a descrição e indica se a inscrição de autoatendimento está habilitada para a política.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:-------|:---|:----------|
|id|Cadeia de caracteres| Propriedade herdada. A ID da política de fluxos de autenticação. Opcional. Somente leitura.
|displayName|Cadeia de caracteres| Propriedade herdada. O nome de política legível. Essa propriedade não é uma chave. Opcional. Somente leitura.|
|description|Cadeia de caracteres|Propriedade herdada. Uma descrição da política. Essa propriedade não é uma chave. Opcional. Somente leitura.|
|selfServiceSignUp|[selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) |Contém configurações [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) que comunicam se a inscrição de autoatendimento está habilitada ou desabilitada. Essa propriedade não é uma chave. Opcional. Somente leitura. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationFlowsPolicy",
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


