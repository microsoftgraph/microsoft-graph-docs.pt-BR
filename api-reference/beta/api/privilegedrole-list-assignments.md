---
title: Lista de atribuições
description: Recupere uma lista de objetos privilegedRoleAssignment que estão associados a função. Cada privilegedRoleAssignment representa uma atribuição de função a um usuário.
localization_priority: Normal
ms.openlocfilehash: f7dd2b94c5d3ac49a6a8c9183373801f76e27964
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508269"
---
# <a name="list-assignments"></a><span data-ttu-id="c6c7b-104">Lista de atribuições</span><span class="sxs-lookup"><span data-stu-id="c6c7b-104">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6c7b-105">Recupere uma lista de objetos [privilegedRoleAssignment](../resources/privilegedroleassignment.md) que estão associados a função.</span><span class="sxs-lookup"><span data-stu-id="c6c7b-105">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects that are associated with the role.</span></span> <span data-ttu-id="c6c7b-106">Cada [privilegedRoleAssignment](../resources/privilegedroleassignment.md) representa uma atribuição de função a um usuário.</span><span class="sxs-lookup"><span data-stu-id="c6c7b-106">Each [privilegedRoleAssignment](../resources/privilegedroleassignment.md) represents a role assignment to a user.</span></span>
## <a name="permissions"></a><span data-ttu-id="c6c7b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c6c7b-107">Permissions</span></span>
<span data-ttu-id="c6c7b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6c7b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c6c7b-110">O solicitante precisa ter uma das seguintes funções: _Leitor de segurança_, _Administrador Global_, _Administrador de segurança_ou _Administrador com privilégios de função_.</span><span class="sxs-lookup"><span data-stu-id="c6c7b-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="c6c7b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6c7b-111">Permission type</span></span>      | <span data-ttu-id="c6c7b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6c7b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6c7b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6c7b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c6c7b-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c6c7b-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c6c7b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6c7b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6c7b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6c7b-116">Not supported.</span></span>    |
|<span data-ttu-id="c6c7b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6c7b-117">Application</span></span> | <span data-ttu-id="c6c7b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6c7b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6c7b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6c7b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/assignments
```

<span data-ttu-id="c6c7b-120">Observe que ``<id>`` é a id de função de destino.</span><span class="sxs-lookup"><span data-stu-id="c6c7b-120">Note that ``<id>`` is the target role id.</span></span>
## <a name="optional-query-parameters"></a><span data-ttu-id="c6c7b-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c6c7b-121">Optional query parameters</span></span>
<span data-ttu-id="c6c7b-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c6c7b-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c6c7b-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6c7b-123">Request headers</span></span>
| <span data-ttu-id="c6c7b-124">Nome</span><span class="sxs-lookup"><span data-stu-id="c6c7b-124">Name</span></span>      |<span data-ttu-id="c6c7b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6c7b-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c6c7b-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6c7b-126">Authorization</span></span>  | <span data-ttu-id="c6c7b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6c7b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6c7b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6c7b-129">Request body</span></span>
<span data-ttu-id="c6c7b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c6c7b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6c7b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6c7b-131">Response</span></span>

<span data-ttu-id="c6c7b-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6c7b-132">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="c6c7b-133">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="c6c7b-133">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c6c7b-134">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="c6c7b-134">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="c6c7b-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6c7b-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6c7b-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6c7b-136">Request</span></span>
<span data-ttu-id="c6c7b-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6c7b-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/assignments
```
##### <a name="response"></a><span data-ttu-id="c6c7b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6c7b-138">Response</span></span>
<span data-ttu-id="c6c7b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6c7b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrole-list-assignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
