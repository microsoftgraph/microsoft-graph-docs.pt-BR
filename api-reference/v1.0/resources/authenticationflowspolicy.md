---
title: Tipo de recurso authenticationFlowsPolicy
description: 'Representa a configuração da política da experiência de inscrição de autoatendimento no nível do locatário que permite aos usuários externos solicitar a inscrição para a aprovação. '
author: linkhp
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 369ad06f9d653054c6b165b0ebc2daa3e8d402c6
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231253"
---
# <a name="authenticationflowspolicy-resource-type"></a>Tipo de recurso authenticationFlowsPolicy

Namespace: microsoft.graph

Representa a [configuração da política da experiência de inscrição de autoatendimento](../resources/selfservicesignupauthenticationflowconfiguration.md) no nível do locatário que permite aos usuários externos solicitar a inscrição para a aprovação. Ela contém informações sobre a ID, o nome de exibição e a descrição e indica se a inscrição de autoatendimento está habilitada para a política.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter política de fluxos de autenticação](../api/authenticationflowspolicy-get.md)|authenticationFlowsPolicy|Obter a configuração da política de fluxos de autenticação.|
|[Atualizar a política de fluxos de autenticação](../api/authenticationflowspolicy-update.md)|authenticationFlowsPolicy|Atualizar a configuração de política de fluxos de autenticação.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:-------|:---|:----------|
|id|Cadeia de caracteres| Propriedade herdada. A ID da política de fluxos de autenticação. Opcional. Somente leitura.
|displayName|Cadeia de caracteres| Propriedade herdada. O nome de política legível. Opcional. Somente leitura.|
|description|Cadeia de caracteres|Propriedade herdada. Uma descrição da política. Opcional. Somente leitura.|
|selfServiceSignUp|[selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) |Contém configurações [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) que comunicam se a inscrição de autoatendimento está habilitada ou desabilitada. Opcional. Somente leitura. |

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
