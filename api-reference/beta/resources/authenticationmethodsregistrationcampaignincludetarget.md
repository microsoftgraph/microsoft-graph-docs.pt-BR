---
title: tipo de recurso authenticationMethodsRegistrationCampaignIncludeTarget
description: Permitir que usuários e grupos de usuários sejam solicitados a configurar métodos de autenticação direcionada.
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 04dc753dd1a574bbf0b30d29b4b80375e7ab9a2c
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682862"
---
# <a name="authenticationmethodsregistrationcampaignincludetarget-resource-type"></a>tipo de recurso authenticationMethodsRegistrationCampaignIncludeTarget

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os usuários e grupos direcionados para campanhas de registro do método de autenticação. Somente usuários e grupos habilitados pela política para configurar o método de autenticação são direcionados.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador de objeto de um usuário ou grupo do Azure AD.|
|targetedAuthenticationMethod|String|O método de autenticação solicitado pelo usuário a registrar. O valor deve ser `microsoftAuthenticator` .|
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
