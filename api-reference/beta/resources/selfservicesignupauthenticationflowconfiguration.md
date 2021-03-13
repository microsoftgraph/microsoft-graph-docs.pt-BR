---
title: Tipo de recurso de configuração de fluxo de autenticação de autoatendimento
description: Representa as configurações relacionadas ao autoatendimento de inscrição.
author: linkhp
localization_priority: Priority
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 93b99ffc6698da60a995bdd8da8f97855dd04b1c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761062"
---
# <a name="selfservicesignupauthenticationflowconfiguration-resource-type"></a>Tipo de recurso de configuração de fluxo de autenticação de autoatendimento


Namespace: Microsoft Graph

Representa as configurações relacionadas ao autoatendimento de registro.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:-------|:---|:----------|
|isEnabled|Booliano|Indica se o fluxo de autoatendimento de inscrição está ativado ou desativado. O valor padrão é `false`. Esta propriedade não é uma chave. Obrigatório. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
}
-->

``` json
{
  "isEnabled": "Boolean"
}
```


