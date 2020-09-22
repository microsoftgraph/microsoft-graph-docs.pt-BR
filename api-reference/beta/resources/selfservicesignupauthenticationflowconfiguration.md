---
title: Tipo de recurso de configuração de fluxo de autenticação de autoatendimento
description: Representa as configurações relacionadas ao autoatendimento de inscrição.
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 658e27e4fe75424f4bd39cc6c3a76255e70c4d92
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988804"
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


