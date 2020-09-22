---
title: tipo de recurso passwordAuthenticationMethod
description: Uma representação de uma senha registrada para um usuário.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c61367520f9dccb47fe238a92366cefd41748865
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998226"
---
# <a name="passwordauthenticationmethod-resource-type"></a>tipo de recurso passwordAuthenticationMethod

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma representação da senha de um usuário. Por segurança, a senha em si nunca será retornada no objeto, mas é possível executar a ação para redefinir uma senha.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
|[Listar passwordAuthenticationMethods](../api/authentication-list-passwordmethods.md) | coleção [passwordAuthenticationMethod](passwordauthenticationmethod.md) | Leia as propriedades e as relações de todos os objetos **passwordAuthenticationMethod** deste usuário. |
|[Obter passwordAuthenticationMethod](../api/passwordauthenticationmethod-get.md) | [passwordAuthenticationMethod](passwordauthenticationmethod.md) | Leia as propriedades e os relacionamentos de um objeto **passwordAuthenticationMethod** . |
|[Redefinir senha](../api/passwordauthenticationmethod-resetpassword.md)|Nenhum|Redefinir a senha de um usuário na nuvem e, se sincronizada, no local.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|creationDatetime|DateTimeOffset|A data e a hora da última atualização da senha. Esta propriedade não está preenchida no momento. Somente leitura. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id|String| O identificador dessa senha registrado para este usuário. Somente leitura.|
|password|String|Por segurança, a senha é sempre retornada como NULL de uma lista ou uma operação GET.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod",
  "baseType": "",
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


