---
title: Tipo de recurso emailAuthenticationMethod
description: Uma representação de um endereço de email registrado para um usuário. O email é um método de autenticação disponível apenas para redefinição de senha de autoatendados (SSPR)
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a24a67fdb4bcc054036de26ba235bf4bac0f2da2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440364"
---
# <a name="emailauthenticationmethod-resource-type"></a>Tipo de recurso emailAuthenticationMethod

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma representação de um endereço de email registrado para um usuário. O email é um método de autenticação disponível apenas para redefinição de senha de autoatendados (SSPR). Os usuários podem ter apenas um método de autenticação de email.


## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[List](../api/emailauthenticationmethod-list.md)|[Coleção emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|Recupere uma lista de emailsauthenticationMethods de um usuário. Os usuários podem ter apenas um método de autenticação de email.|
|[Create](../api/emailauthenticationmethod-post.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|Criar o objeto emailMethods de um usuário.|
|[Get](../api/emailauthenticationmethod-get.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|Recupere as propriedades do objeto emailAuthenticationMethod do usuário.|
|[Atualização](../api/emailauthenticationmethod-update.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|Atualize as propriedades do objeto emailMethods de um usuário.|
|[Delete](../api/emailauthenticationmethod-delete.md)|Nenhum(a)|Exclua o objeto emailAuthenticationMethod de um usuário.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador do endereço de email registrado para esse usuário.|
|emailAddress|String|O endereço de email registrado para esse usuário.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethod",
  "id": "String (identifier)",
  "emailAddress": "String"
}
```

