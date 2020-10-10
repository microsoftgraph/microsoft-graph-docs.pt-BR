---
title: tipo de recurso emailAuthenticationMethod
description: Uma representação de um endereço de email registrado para um usuário. O email é um método de autenticação disponível somente para redefinição de senha de autoatendimento (SSPR)
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6dde3c9a859f2527241b66c0172d6b5dd877aac4
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418193"
---
# <a name="emailauthenticationmethod-resource-type"></a>tipo de recurso emailAuthenticationMethod

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma representação de um endereço de email registrado para um usuário. O email é um método de autenticação disponível somente para redefinição de senha de autoatendimento (SSPR). Os usuários podem ter apenas um método de autenticação de email.


## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[List](../api/emailauthenticationmethod-list.md)|coleção [emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|Recupere uma lista de emailAuthenticationMethods de um usuário. Os usuários podem ter apenas um método de autenticação de email.|
|[Criar](../api/emailauthenticationmethod-post.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|Criar um objeto emailMethods de um usuário.|
|[Obter](../api/emailauthenticationmethod-get.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|Recupere as propriedades do objeto emailAuthenticationMethod do usuário.|
|[Atualizar](../api/emailauthenticationmethod-update.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|Atualiza as propriedades do objeto emailMethods de um usuário.|
|[Excluir](../api/emailauthenticationmethod-delete.md)|Nenhum|Exclua o objeto emailAuthenticationMethod de um usuário.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador do endereço de email registrado para este usuário.|
|emailAddress|String|O endereço de email registrado para este usuário.|

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

