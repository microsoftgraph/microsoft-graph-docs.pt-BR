---
title: 'group: assignLicense'
description: Adicione ou remova licenças no grupo. As licenças atribuídas ao grupo serão atribuídas a todos os usuários do grupo.
ms.localizationpriority: medium
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 240750f8747a3ec2a17e151e3772a69f73f478bd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984748"
---
# <a name="group-assignlicense"></a>group: assignLicense

Namespace: microsoft.graph

Adicione ou remova licenças no grupo. As licenças atribuídas ao grupo serão atribuídas a todos os usuários do grupo. Para saber mais sobre o licenciamento baseado em grupo, consulte O que é licenciamento baseado em [grupo em Azure Active Directory](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).

Para obter as assinaturas disponíveis no diretório, execute uma [solicitação GET subscribedSkus](../resources/subscribedsku.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Group.ReadWrite.All, Directory.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Group.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/assignLicense
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|addLicenses|Coleção [assignedLicense](../resources/assignedlicense.md)|Uma coleção de objetos [assignedLicense](../resources/assignedlicense.md) que especifica as licenças a adicionar. Você pode desabilitar servicePlans associado a uma licença definindo a propriedade **disabledPlans** em [um objeto assignedLicense.](../resources/assignedlicense.md)|
|removeLicenses|Coleção GUID|Uma coleção de skuIds que identificam as licenças a remover.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `202 Accepted` um código de resposta e um objeto [de](../resources/group.md) grupo de destino no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-add-licenses-to-the-group"></a>Exemplo 1: Adicionar licenças ao grupo
O exemplo a seguir adiciona licenças ao grupo.
#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_assignlicense"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/1132b215-826f-42a9-8cfe-1643d19d17fd/assignLicense
Content-type: application/json

{
  "addLicenses": [
    {
      "disabledPlans": [
        "113feb6c-3fe4-4440-bddc-54d774bf0318",
        "14ab5db5-e6c4-4b20-b4bc-13e36fd2227f"
      ],
      "skuId": "b05e124f-c7cc-45a0-a6aa-8cf78c946968"
    },
    {
      "disabledPlans": [
        "a413a9ff-720c-4822-98ef-2f37c2a21f4c"
      ],
      "skuId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
    }
  ],
  "removeLicenses": []
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-assignlicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/group-assignlicense-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

A resposta é o objeto de grupo atualizado.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 202 Accepted
Content-type: application/json
location: https://graph.microsoft.com/v2/e8e96c2a-d787-4eb1-98d7-9e57c965f1de/directoryObjects/1132b215-826f-42a9-8cfe-1643d19d17fd/Microsoft.DirectoryServices.Group

{
  "id": "1132b215-826f-42a9-8cfe-1643d19d17fd",
  "createdDateTime": "2021-03-12T11:15:03Z",
  "groupTypes": [],
  "securityEnabled": true,
}
```

### <a name="example-2-remove-licenses-from-the-group"></a>Exemplo 2: Remover licenças do grupo
O exemplo a seguir remove licenças do grupo.

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_removelicense"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/1132b215-826f-42a9-8cfe-1643d19d17fd/assignLicense
Content-type: application/json

{
  "addLicenses": [],
  "removeLicenses": [
    "c7df2760-2c81-4ef7-b578-5b5392b571df",
    "b05e124f-c7cc-45a0-a6aa-8cf78c946968"
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removelicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removelicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-removelicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-removelicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/group-removelicense-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

A resposta é o objeto de grupo atualizado.

>**Observação:** O objeto de resposta mostrado aqui pode ser reduzido para a capacidade de leitura..
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 202 Accepted
Content-type: application/json
location: https://graph.microsoft.com/v2/d056d009-17b3-4106-8173-cd3978ada898/directoryObjects/1ad75eeb-7e5a-4367-a493-9214d90d54d0/Microsoft.DirectoryServices.Group


{
  "id": "1ad75eeb-7e5a-4367-a493-9214d90d54d0",
  "deletedDateTime": null,
  "classification": null,
  "createdDateTime": "2018-04-18T22:05:03Z",
  "securityEnabled": true,

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

