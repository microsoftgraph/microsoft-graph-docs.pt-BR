---
title: tipo de recurso authenticationMethodsRegistrationCampaignIncludeTarget
description: Permitir que usuários e grupos de usuários sejam solicitados a configurar métodos de autenticação direcionada.
author: mjsantani
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 51f6e1a9842c05a8fb88a92b38cb0c54fbe0d91e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60994709"
---
# <a name="authenticationmethodsregistrationcampaignincludetarget-resource-type"></a>tipo de recurso authenticationMethodsRegistrationCampaignIncludeTarget

Namespace: microsoft.graph

Representa os usuários e grupos direcionados para campanhas de registro do método de autenticação. Somente usuários e grupos habilitados pela política para configurar o método de autenticação são direcionados.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador de objeto de um Azure Active Directory usuário ou grupo.|
|targetedAuthenticationMethod|Cadeia de caracteres|O método de autenticação solicitado pelo usuário a registrar. O valor deve ser `microsoftAuthenticator` .|
|targetType|authenticationMethodTargetType|O tipo de destino do método de autenticação. Os valores possíveis são: `user`, `group`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaignIncludeTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsRegistrationCampaignIncludeTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "targetedAuthenticationMethod": "String"
}
```
