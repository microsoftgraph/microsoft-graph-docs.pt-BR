---
title: tipo de recurso authenticationMethodsRegistrationCampaign
description: Representa as configurações usadas para executar campanhas para pressionar os usuários a configurar métodos de autenticação direcionada.
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: be989bc86e5e708a89cd33c700e57edce42d9e50
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682863"
---
# <a name="authenticationmethodsregistrationcampaign-resource-type"></a>tipo de recurso authenticationMethodsRegistrationCampaign

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações usadas para executar campanhas para pressionar os usuários a configurar métodos de autenticação direcionada. Os usuários são solicitados a configurar o método de autenticação após concluirem com êxito um desafio de MFA. Disponível apenas para o aplicativo Microsoft Authenticator para MFA.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|excludeTargets|[Coleção excludeTarget](../resources/excludetarget.md)|Usuários e grupos de usuários excluídos de serem solicitados a configurar o método de autenticação.|
|includeTargets|[coleção authenticationMethodsRegistrationCampaignIncludeTarget](../resources/authenticationmethodsregistrationcampaignincludetarget.md)|Usuários e grupos de usuários solicitados a configurar o método de autenticação.|
|snoozeDurationInDays|Int32|Especifica o número de dias em que o usuário vê um prompt novamente se ele selecionar "Não agora" e esnome o prompt. Mínimo de 0 dias. Máximo: 14 dias. Se o valor for "0" – o usuário será solicitado durante cada tentativa de MFA.|
|state|advancedConfigState|Habilitar ou desabilitar o recurso. Os valores possíveis são: `default`, `enabled`, `disabled`, `unknownFutureValue`. O valor é usado quando a configuração não foi definida explicitamente e usa o comportamento padrão do `default` Azure AD para a configuração. O valor padrão é `disabled`.|

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
  "snoozeDurationInDays": "Integer",
  "state": "String"
}
```
