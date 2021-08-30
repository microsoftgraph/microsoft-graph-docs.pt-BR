---
title: Tipo de recurso authenticationFlowsPolicy
description: 'Representa a configuração da política da experiência de inscrição de autoatendimento no nível do locatário que permite aos usuários externos solicitar a inscrição para a aprovação. '
author: linkhp
ms.localizationpriority: high
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 195f317785d9a0a3ee85c6bb58872d4c47cc8483
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696327"
---
# <a name="authenticationflowspolicy-resource-type"></a>Tipo de recurso authenticationFlowsPolicy


Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
   "id":"String (identifier)",
   "displayName":"String",
   "description":"String",
   "selfServiceSignUp":{
      "@odata.type":"#microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
   }
}
```


