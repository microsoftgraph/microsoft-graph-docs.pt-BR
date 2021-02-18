---
title: Criar responsabilidades
description: Crie um novo objeto de responsabilidades.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f46a7ba7e7e2d0a6b0d51d16059b78d286fe8e5a
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292340"
---
# <a name="create-personresponsibility"></a>Criar personResponsibility
Namespace: microsoft.graph

Crie um novo [objeto personResponsibility](../resources/personresponsibility.md) no perfil de um [usuário.](../resources/profile.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | User.ReadWrite, User.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | User.ReadWrite, User.ReadWrite.All |
| Aplicativo                            | User.ReadWrite.All                            |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/responsibilities
POST /users/{id | userPrincipalName}/responsibilities
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto personResponsibility.](../resources/personresponsibility.md)

A tabela a seguir mostra as propriedades que são possíveis definir em um novo [objeto personResponsibility](../resources/personresponsibility.md) no perfil de um [usuário.](../resources/profile.md)

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|String|As audiências que podem ver os valores contidos na entidade. Herdado de [itemFacet](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|collaborationTags|Coleção de cadeias de caracteres|Contém marcas de cenário de experiência que um usuário associou ao interesse. Os valores permitidos na coleção são: `askMeAbout` , `ableToMentor` , `wantsToLearn` `wantsToImprove` .|
|description|String|Descrição da responsabilidade.|
|displayName|String|Contém um nome amigável para a responsabilidade. |
|inferência|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pela criação ou modificação do aplicativo. Herdado de [itemFacet](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores se originaram se sincronizados de outro serviço. Herdado de [itemFacet](../resources/itemfacet.md).|
|webUrl|String|Contém um link para uma página da Web ou um recurso sobre a responsabilidade.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta e um `201 Created` [objeto personResponsibility](../resources/personannotation.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

<!-- {
  "blockType": "request",
  "name": "create_personresponsibility_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/responsibilities
Content-Type: application/json
Content-length: 413

{
  "description": "Member of the Microsoft API Council",
  "displayName": "API Council",
  "collaborationTags": [
    "askMeAbout"
  ]
}
```

### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personResponsibility"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "organization",
  "inference": null,
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "source": null,
  "description": "Member of the Microsoft API Council",
  "displayName": "API Council",
  "webUrl": null,
  "collaborationTags": [
    "askMeAbout"
  ]
}
```


