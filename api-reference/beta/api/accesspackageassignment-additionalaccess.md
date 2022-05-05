---
title: 'accessPackageAssignment: additionalAccess'
description: Recupere uma lista de objetos accessPackageAssignment indicando possíveis conflitos de separação de tarefas ou acesso a pacotes de acesso incompatíveis.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6aac3e2ac4ecb3c539a24bf8fa730641e2fa09e1
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203775"
---
# <a name="accesspackageassignment-additionalaccess"></a>accessPackageAssignment: additionalAccess
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure AD Gerenciamento](../resources/entitlementmanagement-overview.md) de Direitos, recupere uma coleção de objetos [accessPackageAssignment](../resources/accesspackageassignment.md) que indicam que um usuário de destino tem uma atribuição a um pacote de acesso especificado e também uma atribuição a outro pacote de acesso potencialmente incompatível.  Isso pode ser usado para se preparar para configurar os pacotes de acesso incompatíveis para um pacote de acesso específico.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackageAssignments/additionalAccess(accessPackageId='parameterValue',incompatibleAccessPackageId='parameterValue')
```

## <a name="function-parameters"></a>Parâmetros de função
A tabela a seguir mostra os parâmetros que devem ser fornecidos com essa função.  As duas IDs de pacote de acesso devem ser distintas.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
| accessPackageId | Cadeia de Caracteres |  Indica a ID de um pacote de acesso para o qual o chamador gostaria de recuperar as atribuições. Obrigatório. |
| incompatibleAccessPackageId | Cadeia de Caracteres | O pacote de acesso incompatível específico para o qual o chamador gostaria de recuperar apenas as atribuições em que o usuário também tem uma atribuição a esse pacote de acesso incompatível. Obrigatório. |

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método dá suporte aos `$select`parâmetros de consulta , `$filter`e `$expand` OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de [objetos accessPackageAssignment](../resources/accesspackageassignment.md) no corpo da resposta.

Quando um conjunto de resultados abrange várias páginas, o Microsoft Graph `@odata.nextLink` retorna essa página com uma propriedade na resposta que contém uma URL para a próxima página de resultados. Se essa propriedade estiver presente, continue fazendo solicitações `@odata.nextLink` adicionais com a URL em cada resposta, até que todos os resultados sejam retornados. Para obter mais informações, [consulte paginação de dados Graph Microsoft em seu aplicativo](/graph/paging).

## <a name="examples"></a>Exemplos

O exemplo a seguir obtém as atribuições de pacote de acesso para usuários que têm atribuições para ambos os pacotes de acesso.

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accesspackageassignment_additionalaccess"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments/additionalAccess(accessPackageId='2506aef1-3929-4d24-a61e-7c8b83d95e6f',incompatibleAccessPackageId='d5d99728-8c0b-4ede-83d2-cf9b0e8dabfb')?$expand=target
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accesspackageassignment-additionalaccess-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accesspackageassignment-additionalaccess-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accesspackageassignment-additionalaccess-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accesspackageassignment-additionalaccess-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/accesspackageassignment-additionalaccess-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/accesspackageassignment-additionalaccess-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
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
            "@odata.type": "#microsoft.graph.accessPackageAssignment",
            "id": "a61f7889-ae61-4e97-a4dc-e4fa525f5b33",
            "catalogId": "beedadfe-01d5-4025-910b-84abb9369997",
            "accessPackageId": "2506aef1-3929-4d24-a61e-7c8b83d95e6f",
            "assignmentPolicyId": "07c7c99d-6cf3-4527-bd05-5fc2ac8e96e7",
            "targetId": "cdbdf152-82ce-479c-b5b8-df90f561d5c7",
            "target": {
                "id": "ebaf071e-c647-42c6-b86f-fbe3625b4b63",
                "objectId": "cdbdf152-82ce-479c-b5b8-df90f561d5c7",
                "displayName": "user1"
            }
        },
        {
            "@odata.type": "#microsoft.graph.accessPackageAssignment",
            "id": "a7284263-8233-44de-8095-0ee3ff5a1716",
            "catalogId": "beedadfe-01d5-4025-910b-84abb9369997",
            "accessPackageId": "2506aef1-3929-4d24-a61e-7c8b83d95e6f",
            "assignmentPolicyId": "07c7c99d-6cf3-4527-bd05-5fc2ac8e96e7",
            "targetId": "79a8f0b6-61dc-41db-b49e-470c278e05b6",
            "target": {
                "id": "9865b0f8-868f-42c6-a49b-3067eb4b2da1",
                "objectId": "79a8f0b6-61dc-41db-b49e-470c278e05b6",
                "displayName": "user2"
            }
        }
  ]
}

```

