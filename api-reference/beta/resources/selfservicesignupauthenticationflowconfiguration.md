---
title: Tipo de recurso de configuração de fluxo de autenticação de autoatendimento
description: Representa as configurações relacionadas ao autoatendimento de inscrição.
author: linkhp
localization_priority: Priority
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: f194c626fceab840f2312200cd824cdbbf63c913345410a6274778d3475bb97b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54212917"
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


