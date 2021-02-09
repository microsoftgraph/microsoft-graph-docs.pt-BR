---
title: Tipo de recurso passwordAuthenticationMethod
description: Uma representação de uma senha registrada para um usuário.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 92e135b74bc68662749376298b4be44155b577b2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156690"
---
# <a name="passwordauthenticationmethod-resource-type"></a>Tipo de recurso passwordAuthenticationMethod

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma representação da senha de um usuário. Por segurança, a senha em si nunca será retornada no objeto, mas é possível fazer uma ação para redefinir uma senha.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
|[Listar passwordAuthenticationMethods](../api/authentication-list-passwordmethods.md) | [Coleção passwordAuthenticationMethod](passwordauthenticationmethod.md) | Leia as propriedades e os relacionamentos de todos os objetos **passwordAuthenticationMethod** desse usuário. |
|[Obter passwordAuthenticationMethod](../api/passwordauthenticationmethod-get.md) | [passwordAuthenticationMethod](passwordauthenticationmethod.md) | Leia as propriedades e os relacionamentos de um **objeto passwordAuthenticationMethod.** |
|[Redefinir senha](../api/passwordauthenticationmethod-resetpassword.md)|Nenhum(a)|Redefinir a senha de um usuário na nuvem e, se sincronizado, no local.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|creationDateTime|DateTimeOffset|A data e a hora em que essa senha foi atualizada pela última vez. No momento, essa propriedade não está preenchida. Somente leitura. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id|String| O identificador dessa senha registrado para esse usuário. Somente leitura.|
|password|String|Para segurança, a senha sempre é retornada como nula de uma operação LIST ou GET.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod",
  "keyProperty": "id"
}-->

```json
{
  "creationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "password": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordAuthenticationMethod resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


