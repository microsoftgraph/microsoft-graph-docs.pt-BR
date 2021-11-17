---
title: tipo de recurso authenticationMethodsRegistrationCampaign
description: Representa as configurações usadas para executar campanhas para pressionar os usuários a configurar métodos de autenticação direcionada.
author: mjsantani
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 71de25c16e357ade6aca9f2bb7fd5100cf8af7cd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019151"
---
# <a name="authenticationmethodsregistrationcampaign-resource-type"></a>tipo de recurso authenticationMethodsRegistrationCampaign

Namespace: microsoft.graph

Representa as configurações usadas para executar campanhas para pressionar os usuários a configurar métodos de autenticação direcionada. Os usuários são solicitados a configurar o método de autenticação após concluirem com êxito um desafio de MFA. Disponível apenas para o aplicativo Microsoft Authenticator para MFA.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|excludeTargets|[Coleção excludeTarget](../resources/excludetarget.md)|Usuários e grupos de usuários excluídos de serem solicitados a configurar o método de autenticação.|
|includeTargets|[coleção authenticationMethodsRegistrationCampaignIncludeTarget](../resources/authenticationmethodsregistrationcampaignincludetarget.md)|Usuários e grupos de usuários solicitados a configurar o método de autenticação.|
|snoozeDurationInDays|Int32|Especifica o número de dias em que o usuário vê um prompt novamente se ele selecionar "Não agora" e esnome o prompt. Mínimo: 0 dias. Máximo: 14 dias. Se o valor for "0", o usuário será solicitado durante cada tentativa de MFA.|
|estado|advancedConfigState|Habilitar ou desabilitar o recurso. Os valores possíveis são: `default`, `enabled`, `disabled`, `unknownFutureValue`. O valor é usado quando a configuração não foi definida explicitamente e usa o comportamento padrão de Azure Active Directory `default` para a configuração. O valor padrão é `disabled`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaign"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsRegistrationCampaign",
  "excludeTargets": [
    {
      "@odata.type": "microsoft.graph.excludeTarget"
    }
  ],
  "includeTargets": [
    {
      "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaignIncludeTarget"
    }
  ],
  "snoozeDurationInDays": "Int32",
  "state": "String"
}
```
