---
title: 'directoryObject: getByIds'
description: Retorna os objetos de diretório especificados em uma lista de IDs.
author: keylimesoda
localization_priority: Priority
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d86b10766b0a735e482fd0d09d19a0682d7099d6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448587"
---
# <a name="directoryobject-getbyids"></a>directoryObject: getByIds

Namespace: microsoft.graph

Retorne os objetos de diretório especificados em uma lista de IDs.

>[!NOTE]
>Essa API tem um [problema conhecido](/graph/known-issues#incomplete-objects-when-using-getbyids-request). Nem todos os objetos de diretório retornados são os objetos completos que contêm todas as propriedades.

Alguns usos comuns dessa função são:

* Resolva as IDs retornadas por funções (que retornam coleções de IDs) como [getMemberObjects](directoryobject-getmemberobjects.md) ou [getMemberGroups](directoryobject-getmembergroups.md) para seus objetos de diretório de suporte.
* Resolva IDs que persistem em um repositório externo pelo aplicativo para seus objetos de diretório de suporte.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.Read.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Directory.Read.All |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Content-type  | string | application/json. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro   | Tipo |Descrição|
|:---------------|:--------|:----------|
|ids|Coleção de cadeias de caracteres| Uma coleção de IDs para a qual retornar objetos.  As IDs são GUIDs, representadas como cadeias de caracteres.  Você pode especificar até 1000 IDs. |
|tipos|Coleção de cadeias de caracteres| Uma coleção de tipos de recursos que especifica o conjunto de coleções de recursos para pesquisar. Se não estiver especificado, o padrão será [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), que contém todos os tipos de recursos definidos no diretório. Qualquer objeto deriva do [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) pode ser especificado na coleção. Por exemplo: [usuário](/graph/api/resources/user?view=graph-rest-v1.0), [grupo](/graph/api/resources/group?view=graph-rest-v1.0), [dispositivo](/graph/api/resources/device?view=graph-rest-v1.0) e assim por diante. Para procurar referências para uma organização parceira do [Provedor de soluções de nuvem](https://partner.microsoft.com/cloud-solution-provider) especifique [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0). Se não for especificado, o padrão é [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0),  que contém todos os tipos de recursos definidos no diretório, exceto referências a uma organização parceira do [Provedor de soluções de nuvem](https://partner.microsoft.com/cloud-solution-provider). Os valores não diferenciam maiúsculas de minúsculas.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto da coleção de cadeias de caracteres no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/v1.0/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893874940a3-97b7-68513b600544","5d6059b6368d-45f8-91e18e07d485f1d0"],
    "types":["user"]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
    "value": [
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Trevor Jones"
      },
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Billy Smith"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

