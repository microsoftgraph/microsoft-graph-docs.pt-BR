---
title: Tipo de recurso de configuração de fluxo de autenticação de autoatendimento
description: Representa as configurações relacionadas ao autoatendimento de inscrição.
author: linkhp
ms.localizationpriority: high
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3bab808249ee7417d721e68dbd2a172c71daf593
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696880"
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


