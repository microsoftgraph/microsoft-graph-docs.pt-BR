---
title: Tipo de recurso registrationEnforcement
description: Impor o registro no momento da inscrição.
author: mjsantani
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e46661280fac283123dde6c3820f68911658a6a5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019147"
---
# <a name="registrationenforcement-resource-type"></a>Tipo de recurso registrationEnforcement

Namespace: microsoft.graph

Impor o registro no momento da inscrição. Atualmente, isso só pode ser usado para lembrar os usuários de configurar métodos de autenticação direcionada (por exemplo, Microsoft Authenticator) usando `authenticationMethodsRegistrationCampaign` o .

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|authenticationMethodsRegistrationCampaign|[authenticationMethodsRegistrationCampaign](../resources/authenticationmethodsregistrationcampaign.md)|Execute campanhas para lembrar os usuários de configurar métodos de autenticação direcionados.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.registrationEnforcement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.registrationEnforcement",
  "authenticationMethodsRegistrationCampaign": {
    "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaign"
  }
}
```
