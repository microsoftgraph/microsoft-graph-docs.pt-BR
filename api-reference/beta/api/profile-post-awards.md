---
title: Criar prêmios
description: Criar um novo objeto de prêmios.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 07f4478350e00184616a719f40c3c21a014a6331
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812855"
---
# <a name="create-personaward"></a>Criar personAward

Namespace: microsoft.graph

Criar um novo objeto [personAward](../resources/personaward.md) no [perfil](../resources/profile.md)de um usuário.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | User. ReadWrite, User. ReadWrite. All |
| Delegada (conta pessoal da Microsoft) | User. ReadWrite, User. ReadWrite. All |
| Aplicativo                            | User.ReadWrite.All                            |
## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/awards
POST /users/{id | userPrincipalName}/profile/awards
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [personAward](../resources/personaward.md) .

A tabela a seguir mostra as propriedades que são possíveis de definir ao criar um novo objeto [personAward](../resources/personaward.md) no [perfil](../resources/profile.md)de um usuário.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|String|As audiências que podem ver os valores contidos na entidade. Herdado de [MyFace](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|description|String|Descpription do prêmio ou honra. |
|displayName|String|Nome do prêmio ou honra. |
|fracassa|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [MyFace](../resources/itemfacet.md).|
|issuedDate|Data|A data em que o prêmio ou honra foi concedido. |
|issuingAuthority|String|Autoridade que concedeu o prêmio ou honra.  |
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores são originados se forem sincronizados a partir de outro serviço. Herdado de [MyFace](../resources/itemfacet.md).|
|thumbnailUrl|String|URL que faz referência a uma miniatura do prêmio ou honra.  |
|webUrl|String|URL que faz referência ao prêmio ou honra. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [personAward](../resources/personaward.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personaward_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/awards
Content-Type: application/json
Content-length: 497

{
  "description": "Lifetime Achievement award from the International Association of Branding Managers",
  "displayName": "Lifetime Achievement Award For Excellence in Branding",
  "issuedDate": "Date",
  "issuingAuthority": "International Association of Branding Management",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAward"
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
  "description": "Lifetime Achievement award from the International Association of Branding Managers",
  "displayName": "Lifetime Achievement Award For Excellence in Branding",
  "issuedDate": "Date",
  "issuingAuthority": "International Association of Branding Management",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```
