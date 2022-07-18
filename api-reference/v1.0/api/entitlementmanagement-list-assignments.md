---
title: Listar accessPackageAssignments
description: Recupere uma lista de objetos accesspackageassignment.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f0fe67076195ea044e2dd8bca822192c31664f69
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100973"
---
# <a name="list-assignments"></a>Listar tarefas

Namespace: microsoft.graph

No gerenciamento de direitos do [Azure AD,](../resources/entitlementmanagement-overview.md)recupere uma lista de [objetos accessPackageAssignment.](../resources/accesspackageassignment.md)

Para administradores de todo o diretório, a lista resultante inclui todas as atribuições, atuais e bem como expiradas, que o chamador tem acesso para ler, em todos os catálogos e pacotes de acesso.  Se o chamador estiver em nome de um usuário delegado atribuído apenas a funções administrativas delegadas específicas do catálogo, a solicitação deverá fornecer um filtro para indicar um pacote de acesso específico, como: `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'` .


## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/assignments
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte `$select` aos `$filter` parâmetros de consulta , e OData para ajudar a personalizar `$expand` a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

### <a name="example-scenarios-for-using-query-parameters"></a>Cenários de exemplo para o uso de parâmetros de consulta

- Se o chamador estiver em nome de um usuário delegado atribuído apenas a funções administrativas delegadas específicas do catálogo, a solicitação deverá fornecer um filtro para indicar um pacote de acesso específico, como: `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'` .
- Para retornar o assunto de destino e o pacote de acesso, inclua `$expand=target,accessPackage` .
- Para recuperar apenas atribuições entregues, você pode incluir uma consulta `$filter=assignmentState eq 'Delivered'` .
- Para recuperar apenas atribuições para um usuário específico, você pode incluir uma consulta com atribuições voltadas para a ID do objeto desse usuário: `$expand=target&$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'` .
- Para recuperar apenas atribuições para um determinado usuário e um pacote de acesso específico, você pode incluir uma consulta com atribuições voltadas para esse pacote de acesso e a ID do objeto desse usuário: `$expand=accessPackage,target&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea' and target/objectid eq '7deff43e-1f17-44ef-9e5f-d516b0ba11d4'` .


## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessPackageAssignment](../resources/accesspackageassignment.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accesspackageassignment"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignments
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accesspackageassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accesspackageassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accesspackageassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accesspackageassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-accesspackageassignment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-accesspackageassignment-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "2a353749-3749-2a35-4937-352a4937352a",
      "state": "delivered",
      "status": "Delivered",
      "expiredDateTime": "2019-04-25T23:45:40.42Z",
      "schedule": {
        "@odata.type": "microsoft.graph.entitlementManagementSchedule"
      }
    }
  ]
}
```



