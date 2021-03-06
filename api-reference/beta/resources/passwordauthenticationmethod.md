---
title: tipo de recurso passwordAuthenticationMethod
description: Uma representação de uma senha registrada para um usuário.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f902d47d0d06857537a07541456596c3a6204bc3
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720565"
---
# <a name="passwordauthenticationmethod-resource-type"></a>tipo de recurso passwordAuthenticationMethod

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma representação da senha de um usuário. Por segurança, a senha em si nunca será retornada no objeto, mas pode ser tomada uma ação para redefinir uma senha.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
|[Listar passwordAuthenticationMethods](../api/authentication-list-passwordmethods.md) | [coleção passwordAuthenticationMethod](passwordauthenticationmethod.md) | Leia as propriedades e as relações de todos os objetos **passwordAuthenticationMethod** deste usuário. |
|[Obter passwordAuthenticationMethod](../api/passwordauthenticationmethod-get.md) | [passwordAuthenticationMethod](passwordauthenticationmethod.md) | Leia as propriedades e as relações de um **objeto PasswordAuthenticationMethod.** |
|[Redefinir senha](../api/passwordauthenticationmethod-resetpassword.md)|Nenhum(a)|Redefinir a senha de um usuário na nuvem e, se sincronizado, no local.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|creationDateTime|DateTimeOffset|A data e a hora em que essa senha foi atualizada pela última vez. No momento, essa propriedade não está preenchida. Somente leitura. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|id|Cadeia de caracteres| O identificador dessa senha registrado para esse usuário. Somente leitura.|
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


