---
title: Tipo de recurso temporaryAccessPassAuthenticationMethod
description: Representa uma Passagem de Acesso Temporária registrada para um usuário.
author: tilarso
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: aacb033a858255fe69a44a530ad37ee394fbbfc3
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095080"
---
# <a name="temporaryaccesspassauthenticationmethod-resource-type"></a>Tipo de recurso temporaryAccessPassAuthenticationMethod

Namespace: microsoft.graph

Representa uma Passagem de Acesso Temporária registrada para um usuário. Uma Passagem de Acesso Temporária é uma senha com tempo limitado que serve como uma credencial forte e permite a integração de credenciais sem senha. A disponibilidade e as configurações que podem ser [definidas](temporaryaccesspassauthenticationmethodconfiguration.md) para **temporaryAccessPassAuthenticationMethod** dependem da política de métodos de Passagem de Acesso Temporário.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar](../api/authentication-list-temporaryaccesspassmethods.md)|[Coleção temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Recupere uma lista dos objetos **temporaryAccessPassAuthenticationMethod** de um usuário e suas propriedades. Os usuários só podem ter um método de autenticação de Passagem de Acesso Temporário.|
|[Criar](../api/authentication-post-temporaryaccesspassmethods.md)|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Crie o objeto **temporaryAccessPassAuthenticationMethod de um** usuário.|
|[Get](../api/temporaryaccesspassauthenticationmethod-get.md)|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Recupere as propriedades do objeto **temporaryAccessPassAuthenticationMethod do** usuário.|
|[Excluir](../api/temporaryaccesspassauthenticationmethod-delete.md)|Nenhum|Exclua o **objeto temporaryAccessPassAuthenticationMethod de um** usuário.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|A data e a hora em que a Passagem de Acesso Temporário foi criada.|
|id|Cadeia de caracteres|O identificador da Passagem de Acesso Temporário registrada para esse usuário. Herdado da [entidade](../resources/entity.md).|
|isUsableOnce|Booliano|Determina se a passagem está limitada a um uso único. If `true`, the pass can be used once; if `false`, the pass can be used multiple times within the Temporary Access Pass lifetime.|
|isUsable|Boolean|O estado do método de autenticação que indica se ele pode ser usado no momento pelo usuário.|
|lifetimeInMinutes|Int32|O tempo de vida da Passagem de Acesso Temporário em minutos, começando em **startDateTime**. Deve estar entre 10 e 43200 inclusive (equivalente a 30 dias).|
|methodUsabilityReason|String|Detalhes sobre o estado de usabilidade (**isUsable**). Os motivos podem incluir: `EnabledByPolicy`, `DisabledByPolicy`, `Expired`, `NotYetValid`, `OneTimeUsed`.|
|startDateTime|DateTimeOffset|A data e a hora em que a Passagem de Acesso Temporário fica disponível para uso e quando **isUsable** é `true` imposta.|
|temporaryAccessPass|Cadeia de caracteres|A Passagem de Acesso Temporária usada para autenticar. Retornado somente na criação de um novo **objeto temporaryAccessPassAuthenticationMethod** ; Oculto em operações de leitura subsequentes e retornado como `null` com GET.|

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
