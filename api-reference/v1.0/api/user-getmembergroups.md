---
title: 'usuário: getMemberGroups'
description: Retorne todos os grupos dos quais o usuário é membro. A verificação foi transitiva, ao contrário de leitura a
localization_priority: Priority
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 8ebbbe1aeca0e20af40b19cf72ef1baa4ce0689d
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51870041"
---
# <a name="user-getmembergroups"></a>usuário: getMemberGroups

Namespace: microsoft.graph

Retorne todos os grupos dos quais o usuário é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação [member](../api/user-list-memberof.md), que retorna somente os grupos dos quais o usuário é membro direto.

Esta função é compatível com o Microsoft 365 e outros tipos de grupos provisionados no Azure AD. O número máximo de grupos que cada solicitação pode retornar é 2046. Observe que os grupos do Microsoft 365 não podem conter grupos. Portanto, associações em um grupo do Microsoft 365 sempre são diretas.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                                                                                          |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| Delegada (conta corporativa ou de estudante)     | User.ReadBasic.All, User.Read, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                                                                                                                                       |
| Application                            |  User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/getMemberGroups
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor                     |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |
| Content-Type  | application/json          |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro           | Tipo    | Descrição                                                                                                                                                                                                                                                                         |
| :------------------ | :------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| securityEnabledOnly | Booliano | **true** para especificar que somente grupos de segurança dos quais o usuário é membro devem ser retornados; **false** para especificar que todos os grupos dos quais o usuário é membro devem ser retornados. Observação: Definir esse parâmetro como **true** é suportado apenas ao chamar este método em um usuário. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o usuário é membro.

## <a name="example"></a>Exemplo

Eis um exemplo de como chamar esta API.

##### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "user: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

