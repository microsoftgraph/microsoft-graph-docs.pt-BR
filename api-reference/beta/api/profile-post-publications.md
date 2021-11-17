---
title: Criar publicações
description: Crie um novo objeto publications.
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 801d330884d310ab6c101ad98215004c62e65d10
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019329"
---
# <a name="create-itempublication"></a>Criar itemPublication
Namespace: microsoft.graph

Criar um novo [objeto itemPublication](../resources/itempublication.md) no perfil de um [usuário.](../resources/profile.md)

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
POST /me/profile/publications
POST /users/{id | userPrincipalName}/profile/publications
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto itemPublication.](../resources/itempublication.md)

A tabela a seguir mostra as propriedades que são possíveis de definir ao criar um novo [objeto itemPublication](../resources/itempublication.md) no perfil de um [usuário](../resources/profile.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedAudiences|Cadeia de caracteres|As audiências que são capazes de ver os valores contidos na entidade. Herdado [do itemFacet](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado [do itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece a dataTimeOffset para quando a entidade foi criada. Herdado [do itemFacet](../resources/itemfacet.md).|
|description    |Cadeia de caracteres      |Descrição da publicação.                   |
|displayName    |Cadeia de caracteres      |Título da publicação.                         |
|id|String|Identificador usado para endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|inferência|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado [do itemFacet](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado [do itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece a dataTimeOffset para quando a entidade foi criada. Herdado [do itemFacet](../resources/itemfacet.md).|
|publishedDate  |Data        |A data em que a publicação foi publicada.      |
|publicador      |String      |Publicação ou Publisher para a publicação.     |
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores se originaram se sincronizados de outro serviço. Herdado [do itemFacet](../resources/itemfacet.md).|
|thumbnailUrl   |String      |URL fazendo referência a uma miniatura da publicação.   |
|webUrl         |String      |URL fazendo referência à publicação.                  |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [itemPublication](../resources/itempublication.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itemPublication_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/publications
Content-Type: application/json

{
  "description": "One persons journey to the top of the branding management field.",
  "displayName": "Got Brands? The story of Innocenty Popov and his journey to the top.",
  "publishedDate": "Date",
  "publisher": "International Association of Branding Management Publishing",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itempublication-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itempublication-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itempublication-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-itempublication-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-itempublication-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPublication"
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
  "description": "One persons journey to the top of the branding management field.",
  "displayName": "Got Brands? The story of Innocenty Popov and his journey to the top.",
  "publishedDate": "Date",
  "publisher": "International Association of Branding Management Publishing",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```


