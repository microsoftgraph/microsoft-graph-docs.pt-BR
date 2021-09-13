---
title: Tipo de recurso de configuração de fluxo de autenticação de autoatendimento
description: Representa as configurações relacionadas ao autoatendimento de inscrição.
author: linkhp
ms.localizationpriority: high
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 735803c579f79e9f27f81c53fd9e3fd5ce94e84a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067014"
---
# <a name="selfservicesignupauthenticationflowconfiguration-resource-type"></a>Tipo de recurso de configuração de fluxo de autenticação de autoatendimento

Namespace: Microsoft Graph

Representa as configurações relacionadas a inscrição de autoatendimento.

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
