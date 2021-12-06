---
title: Criar plannerRosterMember
description: Crie um novo objeto plannerRosterMember.
author: tarkansevilmis
ms.localizationpriority: medium
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: a1688a176c192b660e3d63da3d20a473a91b8662
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990054"
---
# <a name="create-plannerrostermember"></a>Criar plannerRosterMember
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Adicione um membro ao [objeto plannerRoster.](../resources/plannerrostermember.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Tasks.ReadWrite|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /planner/rosters/{plannerRosterId}/members
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto plannerRosterMember.](../resources/plannerrostermember.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o plannerRosterMember](../resources/plannerrostermember.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|userId|Cadeia de caracteres|Identificador do .|
|tenantId|String|Identificador do locatário ao que o usuário pertence. Opcional. Atualmente, os membros da lista não podem ser de locatários diferentes.|
|funções|Coleção de cadeias de caracteres|Funções adicionais atribuídas ao usuário. Opcional. Atualmente, não há funções adicionais disponíveis para os usuários.|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto plannerRosterMember](../resources/plannerrostermember.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerrostermember_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/planner/rosters/6519868f-868f-6519-8f86-19658f861965/members
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.plannerRosterMember",
  "userId": "String"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerrostermember-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerrostermember-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerrostermember-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerrostermember-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-plannerrostermember-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerRosterMember"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.plannerRosterMember",
  "id": "670095cd-95cd-6700-cd95-0067cd950067",
  "userId": "5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38",
  "roles": [
  ]
}
```

