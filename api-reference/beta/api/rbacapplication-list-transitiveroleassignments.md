---
title: Listar transitiveRoleAssignment
description: Listar atribuições de função diretas e transitivas para uma entidade de segurança específica.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b29fe74cae67dab5731ba7098f2fc7cf3591ddda
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338098"
---
# <a name="list-transitiveroleassignment"></a>Listar transitiveRoleAssignment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter a lista de objetos [unifiedRoleAssignment diretos e transitivos](../resources/unifiedroleassignment.md) para uma entidade principal específica. Por exemplo, se um usuário receber uma função do Azure AD por meio da associação ao grupo, a atribuição de função será transitiva e essa solicitação lista a ID do grupo como a **principalId**. Os resultados também podem ser filtrados pela **funçãoDefinitionId** e **directoryScopeId**. Suportado apenas para provedor de diretório (Azure AD).

Para obter mais informações, [consulte Usar grupos do Azure AD para gerenciar atribuições de função](/azure/active-directory/roles/groups-concept).

> [!NOTE]
> Essa solicitação pode ter atrasos de replicação para atribuições de função que foram criadas, atualizadas ou excluídas recentemente.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

Para listar atribuições de função transitiva para um provedor de diretórios:

<!-- {
  "blockType": "ignored"
}
-->
```http
GET /roleManagement/directory/transitiveRoleAssignments?$filter=principalId eq '{principalId}'
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte aos `$count`parâmetros de consulta , `$filter` (`eq`) `$select` e OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters). Você pode filtrar pelo **principalId**, **roleDefinitionId** e **directoryScopeId** para recuperar atribuições de função diretas e transitivas para uma entidade principal.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | Portador {token} Obrigatório. |
| ConsistencyLevel | eventualmente. Este header e `$count`são `$filter` obrigatórios. Para obter mais informações sobre o uso **de ConsistencyLevel** e `$count`, `$filter`consulte Recursos avançados de consulta em objetos de diretório [do Azure AD](/graph/aad-advanced-queries). |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de [objetos unifiedRoleAssignment](../resources/unifiedroleassignment.md) no corpo da resposta.

## <a name="examples"></a>Exemplos
Para os exemplos nesta seção, considere o seguinte cenário de atribuição de função. Um usuário chamado Alice tem atribuições de função diretas e transitivas da seguinte forma:

| Usuário | Group | Função | Escopo | ID de atribuição de função |
| :---: | :---: | :---: | :---: | :---: |
| Alice<br/>`2c7936bc-3517-40f3-8eda-4806637b6516` |  | Administrador do usuário<br/>`fe930be7-5e62-47db-91af-98c3a49a38b1` | Tenant | RA1<br/>`857708a7-b5e0-44f9-bfd7-53531d72a739` |
|  | G1<br/>`ae2fc327-4c71-48ed-b6ca-f48632186510`<br/>(Alice é membro) | Administrador do usuário<br/>`fe930be7-5e62-47db-91af-98c3a49a38b1` | Tenant | RA2<br/>`8a021d5f-7351-4713-aab4-b088504d476e` |
|  | G2<br/>`6ffb34b8-5e6d-4727-a7f9-93245e7f6ea8`<br/>(Alice é membro) | Administrador da Assistência Técnica<br/>`729827e3-9c14-49f7-bb1b-9608f156bbb8` | Unidade administrativa (AU1)<br/>`26e79164-0c5c-4281-8c5b-be7bc7809fb2` | RA3<br/>`6cc86637-13c8-473f-afdc-e0e65c9734d2` |

+ Alice recebe a função administrador do usuário diretamente no escopo do locatário com a atribuição de função RA1. 
+ Alice é membro de um grupo G1 e G1 recebe a função de Administrador de Usuário no escopo do locatário com a atribuição de função RA2.
+ Alice também é membro do grupo G2 e G2 é atribuída a função administrador do Helpdesk em um escopo de unidade administrativa AU1 com atribuição de função RA3.

### <a name="example-1--get-direct-and-transitive-role-assignments-of-a-principal"></a>Exemplo 1 : Obter atribuições de função diretas e transitivas de uma entidade

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. Essa solicitação requer o header **ConsistencyLevel** definido como `eventual` e os `$count=true` parâmetros `$filter` de consulta e. Para obter mais informações sobre o uso **de ConsistencyLevel** e `$count`, `$filter`consulte Recursos avançados de consulta em objetos de diretório [do Azure AD](/graph/aad-advanced-queries).


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_all"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/transitiveRoleAssignments?$count=true&$filter=principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516'
ConsistencyLevel: eventual
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-all-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-all-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-all-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-all-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-unifiedroleassignment-all-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "isCollection": true
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/transitiveRoleAssignments",
    "value": [
        {
            "id": "857708a7-b5e0-44f9-bfd7-53531d72a739",
            "principalId": "2c7936bc-3517-40f3-8eda-4806637b6516",
            "directoryScopeId": "/",
            "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1"
        },
        {
            "id": "8a021d5f-7351-4713-aab4-b088504d476e",
            "principalId": "ae2fc327-4c71-48ed-b6ca-f48632186510",
            "directoryScopeId": "/",
            "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1"
        },
        {
            "id": "6cc86637-13c8-473f-afdc-e0e65c9734d2",
            "principalId": "6ffb34b8-5e6d-4727-a7f9-93245e7f6ea8",
            "directoryScopeId": "/administrativeUnits/26e79164-0c5c-4281-8c5b-be7bc7809fb2",
            "roleDefinitionId": "729827e3-9c14-49f7-bb1b-9608f156bbb8"
        }
    ]
}
```

### <a name="example-2-get-direct-and-transitive-assignments-of-a-principal-but-only-specific-role-definitions"></a>Exemplo 2: Obter atribuições diretas e transitivas de uma entidade principal, mas apenas definições de função específicas

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. Essa solicitação requer o header **ConsistencyLevel** definido como `eventual` e os `$count=true` parâmetros `$filter` de consulta e. Para obter mais informações sobre o uso **de ConsistencyLevel** e `$count`, `$filter`consulte Recursos avançados de consulta em objetos de diretório [do Azure AD](/graph/aad-advanced-queries).


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_transitive"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/transitiveRoleAssignments?$count=true&$filter=principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516' and roleDefinitionId eq 'fe930be7-5e62-47db-91af-98c3a49a38b1'
ConsistencyLevel: eventual
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-transitive-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-transitive-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-transitive-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-transitive-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-unifiedroleassignment-transitive-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "isCollection": true
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/transitiveRoleAssignments",
    "value": [
        {
            "id": "857708a7-b5e0-44f9-bfd7-53531d72a739",
            "principalId": "2c7936bc-3517-40f3-8eda-4806637b6516",
            "directoryScopeId": "/",
            "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1"
        },
        {
            "id": "8a021d5f-7351-4713-aab4-b088504d476e",
            "principalId": "6ffb34b8-5e6d-4727-a7f9-93245e7f6ea8",
            "directoryScopeId": "/",
            "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1"
        }
    ]
}
```

### <a name="example-3-get-direct-and-transitive-role-assignments-of-a-principal-but-only-administrative-unit-scoped"></a>Exemplo 3: Obter atribuições de função diretas e transitivas de uma entidade principal, mas apenas unidade administrativa com escopo

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. Essa solicitação requer o header **ConsistencyLevel** definido como `eventual` e os `$count=true` parâmetros `$filter` de consulta e. Para obter mais informações sobre o uso **de ConsistencyLevel** e `$count`, `$filter`consulte Recursos avançados de consulta em objetos de diretório [do Azure AD](/graph/aad-advanced-queries).


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_tenantscoped"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/transitiveRoleAssignments?$count=true&$filter=principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516' and directoryScopeId eq '/administrativeUnits/26e79164-0c5c-4281-8c5b-be7bc7809fb2'
ConsistencyLevel: eventual
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-tenantscoped-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-tenantscoped-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-tenantscoped-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-tenantscoped-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-unifiedroleassignment-tenantscoped-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "isCollection": true
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/transitiveRoleAssignments",
    "value": [
        {
            "id": "6cc86637-13c8-473f-afdc-e0e65c9734d2",
            "principalId": "6ffb34b8-5e6d-4727-a7f9-93245e7f6ea8",
            "directoryScopeId": "/administrativeUnits/26e79164-0c5c-4281-8c5b-be7bc7809fb2",
            "roleDefinitionId": "729827e3-9c14-49f7-bb1b-9608f156bbb8"
        }
    ]
}
```
