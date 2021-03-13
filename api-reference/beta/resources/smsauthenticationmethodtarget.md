---
title: Tipo de recurso smsAuthenticationMethodTarget
description: Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação de Mensagem de Texto.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4309316adfeff126f845dd362d5ffb8899a77e60
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761027"
---
# <a name="smsauthenticationmethodtarget-resource-type"></a>Tipo de recurso smsAuthenticationMethodTarget
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação de Mensagem [de](../resources/smsAuthenticationMethodConfiguration.md) Texto no Azure AD.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID do objeto de um usuário ou grupo do Azure AD.|
|isRegistrationRequired|Boolean|Determina se o usuário é imposto a registrar o método de autenticação. **Não há suporte para**.|
|isUsableForSignIn|Boolean|Determina se os usuários ou grupos podem usar esse método de autenticação para entrar no Azure AD. O valor é sempre `true` .|
|targetType|authenticationMethodTargetType| Os valores possíveis são: `user`, `group`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.smsAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.smsAuthenticationMethodTarget",
  "targetType": "String",
  "id": "String (identifier)",
  "isRegistrationRequired": "Boolean",
  "isUsableForSignIn": "Boolean"
}
```
