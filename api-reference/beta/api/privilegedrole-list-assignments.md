---
title: Lista de atribuições
description: Recupere uma lista de objetos privilegedRoleAssignment que estão associados a função. Cada privilegedRoleAssignment representa uma atribuição de função a um usuário.
ms.openlocfilehash: 52cc720381baa6b7c82fe3b5c88d469081da3b81
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037863"
---
# <a name="list-assignments"></a><span data-ttu-id="9ae91-104">Lista de atribuições</span><span class="sxs-lookup"><span data-stu-id="9ae91-104">List assignments</span></span>

> <span data-ttu-id="9ae91-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9ae91-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ae91-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9ae91-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9ae91-107">Recupere uma lista de objetos [privilegedRoleAssignment](../resources/privilegedroleassignment.md) que estão associados a função.</span><span class="sxs-lookup"><span data-stu-id="9ae91-107">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects that are associated with the role.</span></span> <span data-ttu-id="9ae91-108">Cada [privilegedRoleAssignment](../resources/privilegedroleassignment.md) representa uma atribuição de função a um usuário.</span><span class="sxs-lookup"><span data-stu-id="9ae91-108">Each [privilegedRoleAssignment](../resources/privilegedroleassignment.md) represents a role assignment to a user.</span></span>
## <a name="permissions"></a><span data-ttu-id="9ae91-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="9ae91-109">Permissions</span></span>
<span data-ttu-id="9ae91-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ae91-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9ae91-112">O solicitante precisa ter uma das seguintes funções: _Leitor de segurança_, _Administrador Global_, _Administrador de segurança_ou _Administrador com privilégios de função_.</span><span class="sxs-lookup"><span data-stu-id="9ae91-112">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="9ae91-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ae91-113">Permission type</span></span>      | <span data-ttu-id="9ae91-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ae91-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ae91-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ae91-115">Delegated (work or school account)</span></span> | <span data-ttu-id="9ae91-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9ae91-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9ae91-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ae91-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ae91-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ae91-118">Not supported.</span></span>    |
|<span data-ttu-id="9ae91-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ae91-119">Application</span></span> | <span data-ttu-id="9ae91-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ae91-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ae91-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ae91-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/assignments
```

<span data-ttu-id="9ae91-122">Observe que ``<id>`` é a id de função de destino.</span><span class="sxs-lookup"><span data-stu-id="9ae91-122">Note that ``<id>`` is the target role id.</span></span>
## <a name="optional-query-parameters"></a><span data-ttu-id="9ae91-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9ae91-123">Optional query parameters</span></span>
<span data-ttu-id="9ae91-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9ae91-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ae91-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ae91-125">Request headers</span></span>
| <span data-ttu-id="9ae91-126">Nome</span><span class="sxs-lookup"><span data-stu-id="9ae91-126">Name</span></span>      |<span data-ttu-id="9ae91-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ae91-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9ae91-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ae91-128">Authorization</span></span>  | <span data-ttu-id="9ae91-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ae91-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ae91-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ae91-131">Request body</span></span>
<span data-ttu-id="9ae91-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ae91-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ae91-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ae91-133">Response</span></span>

<span data-ttu-id="9ae91-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ae91-134">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="9ae91-135">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="9ae91-135">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="9ae91-136">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="9ae91-136">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="9ae91-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ae91-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ae91-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ae91-138">Request</span></span>
<span data-ttu-id="9ae91-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ae91-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/assignments
```
##### <a name="response"></a><span data-ttu-id="9ae91-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ae91-140">Response</span></span>
<span data-ttu-id="9ae91-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ae91-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
