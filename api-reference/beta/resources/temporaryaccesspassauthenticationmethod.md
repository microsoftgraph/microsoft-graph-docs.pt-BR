---
title: tipo de recurso temporaryAccessPassAuthenticationMethod
description: Representa um Passe de Acesso Temporário registrado para um usuário.
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1bd5bd1ab118d7ec5c7443c47bda1ea614f31bf0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442800"
---
# <a name="temporaryaccesspassauthenticationmethod-resource-type"></a>tipo de recurso temporaryAccessPassAuthenticationMethod

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um Passe de Acesso Temporário registrado para um usuário. Um Passe de Acesso Temporário é uma senha limitada por tempo que serve como uma credencial forte e permite a integração de credenciais sem senha.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[List](../api/temporaryaccesspassauthenticationmethod-list.md)|[coleção temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Recupere uma lista dos objetos **temporaryAccessPassAuthenticationMethod** de um usuário e suas propriedades. Os usuários só podem ter um método de autenticação de Passagem de Acesso Temporário.|
|[Create](../api/temporaryaccesspassauthenticationmethod-post.md)|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Crie um objeto **temporaryAccessPassAuthenticationMethod de um** usuário.|
|[Get](../api/temporaryaccesspassauthenticationmethod-get.md)|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Recupere as propriedades do objeto **temporaryAccessPassAuthenticationMethod do** usuário.||
|[Delete](../api/temporaryaccesspassauthenticationmethod-delete.md)|Nenhum(a)|Exclua o **objeto temporaryAccessPassAuthenticationMethod de um** usuário.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador do Passe de Acesso Temporário registrado para esse usuário.|
|temporaryAccessPass|String|O temporaryAccessPass usado para autenticar. Retornado somente na criação de um novo temporaryAccessPass; retornado como NULL com GET.|
|createdDateTime|DateTimeOffset|A data e a hora em que o temporaryAccessPass foi criado.|
|startDateTime|DateTimeOffset|A data e a hora em que o temporaryAccessPass fica disponível para uso.|
|lifetimeInMinutes|Int32|O tempo de vida do temporaryAccessPass em minutos começando em startDateTime. Mínimo 10, Máximo 43200 (equivalente a 30 dias).|
|isUsableOnce|Booliano|Determina se a passagem está limitada a um uso único. If , the pass can be used once; if , the pass can be `true` used multiple times within the `false` temporaryAccessPass lifetime.|
|isUsable|Booliano|O estado do método de autenticação que indica se ele pode ser usado no momento pelo usuário.|
|methodUsabilityReason|String|Detalhes sobre o estado de usabilidade (isUsable). Os motivos podem incluir: `enabledByPolicy` , , , , `disabledByPolicy` `expired` `notYetValid` `oneTimeUsed` .|


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
  "id": "String (identifier)",
  "temporaryAccessPass": "String",
  "createdDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "lifetimeInMinutes": "Integer",
  "isUsableOnce": "Boolean",
  "isUsable": "Boolean",
  "methodUsabilityReason": "String"
}
```
