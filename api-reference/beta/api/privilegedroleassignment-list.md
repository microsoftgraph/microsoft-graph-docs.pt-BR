---
title: Listar privilegedRoleAssignments
description: Recupere uma lista de objetos privilegedRoleAssignment, que correspondem a todas as atribuições de função da organização.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: d6c99aa96fb8b2bec47f57fdc32abe5e008aac12
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035049"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="9e683-103">Listar privilegedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="9e683-103">List privilegedRoleAssignments</span></span>

<span data-ttu-id="9e683-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e683-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e683-105">Recupere uma lista de objetos [privilegedRoleAssignment](../resources/privilegedroleassignment.md) , que correspondem a todas as atribuições de função da organização.</span><span class="sxs-lookup"><span data-stu-id="9e683-105">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="9e683-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9e683-106">Permissions</span></span>
<span data-ttu-id="9e683-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e683-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9e683-109">O solicitante precisa ter uma das seguintes funções: administrador de _função privilegiada_, _administrador global_, _administrador de segurança_ou _leitor de segurança_.</span><span class="sxs-lookup"><span data-stu-id="9e683-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="9e683-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e683-110">Permission type</span></span>      | <span data-ttu-id="9e683-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e683-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e683-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e683-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9e683-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9e683-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9e683-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e683-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e683-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e683-115">Not supported.</span></span>    |
|<span data-ttu-id="9e683-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e683-116">Application</span></span> | <span data-ttu-id="9e683-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e683-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e683-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e683-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9e683-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9e683-119">Optional query parameters</span></span>
<span data-ttu-id="9e683-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9e683-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e683-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e683-121">Request headers</span></span>
| <span data-ttu-id="9e683-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9e683-122">Name</span></span>      |<span data-ttu-id="9e683-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e683-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9e683-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e683-124">Authorization</span></span>  | <span data-ttu-id="9e683-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e683-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e683-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e683-127">Request body</span></span>
<span data-ttu-id="9e683-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e683-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e683-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e683-129">Response</span></span>

<span data-ttu-id="9e683-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e683-130">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="9e683-131">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="9e683-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="9e683-132">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="9e683-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="9e683-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9e683-133">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="9e683-134">Obter todas as atribuições de função</span><span class="sxs-lookup"><span data-stu-id="9e683-134">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="9e683-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e683-135">Request</span></span>
<span data-ttu-id="9e683-136">O exemplo a seguir mostra uma solicitação para obter todas as atribuições de função:</span><span class="sxs-lookup"><span data-stu-id="9e683-136">The following example shows a request to get all role assignments:</span></span>

# <a name="http"></a>[<span data-ttu-id="9e683-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e683-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="9e683-138">C#</span><span class="sxs-lookup"><span data-stu-id="9e683-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e683-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e683-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e683-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e683-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9e683-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e683-141">Response</span></span>
<span data-ttu-id="9e683-142">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="9e683-142">The following example shows the response.</span></span> <span data-ttu-id="9e683-143">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="9e683-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9e683-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e683-144">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-active-role-assignments"></a><span data-ttu-id="9e683-145">Obter atribuições de função ativas</span><span class="sxs-lookup"><span data-stu-id="9e683-145">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="9e683-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e683-146">Request</span></span> 
<span data-ttu-id="9e683-147">O exemplo a seguir mostra uma solicitação para consultar as atribuições de função ativas:</span><span class="sxs-lookup"><span data-stu-id="9e683-147">The following example shows a request to query active role assignments:</span></span>

# <a name="http"></a>[<span data-ttu-id="9e683-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e683-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
# <a name="c"></a>[<span data-ttu-id="9e683-149">C#</span><span class="sxs-lookup"><span data-stu-id="9e683-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e683-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e683-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e683-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e683-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9e683-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e683-152">Response</span></span>
<span data-ttu-id="9e683-153">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="9e683-153">The following example shows the response.</span></span> <span data-ttu-id="9e683-154">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="9e683-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9e683-155">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e683-155">All of the properties will be returned from an actual call.</span></span>
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
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_62e90394-69f5-4237-9190-012177145e10",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "62e90394-69f5-4237-9190-012177145e10",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": true,
            "expirationDateTime": "2017-07-25T17:38:49.563Z",
            "resultMessage": null
        }
  ]
}
```
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="9e683-156">Obter atribuições de função permanentes</span><span class="sxs-lookup"><span data-stu-id="9e683-156">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="9e683-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e683-157">Request</span></span> 
<span data-ttu-id="9e683-158">O exemplo a seguir mostra uma solicitação para consultar atribuições de função permanentes, onde ``expirationDateTime`` Value é ``null`` :</span><span class="sxs-lookup"><span data-stu-id="9e683-158">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>

# <a name="http"></a>[<span data-ttu-id="9e683-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e683-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
# <a name="c"></a>[<span data-ttu-id="9e683-160">C#</span><span class="sxs-lookup"><span data-stu-id="9e683-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e683-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e683-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e683-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e683-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9e683-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e683-163">Response</span></span>
<span data-ttu-id="9e683-164">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="9e683-164">The following example shows the response.</span></span> <span data-ttu-id="9e683-165">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="9e683-165">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9e683-166">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e683-166">All of the properties will be returned from an actual call.</span></span>
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
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_194ae4cb-b126-40b2-bd5b-6091b380977d",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "194ae4cb-b126-40b2-bd5b-6091b380977d",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_44367163-eba1-44c3-98af-f5787879f96a",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "44367163-eba1-44c3-98af-f5787879f96a",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        }
  ]
}
```
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="9e683-167">Obter atribuições de função qualificadas</span><span class="sxs-lookup"><span data-stu-id="9e683-167">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="9e683-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e683-168">Request</span></span> 
<span data-ttu-id="9e683-169">O exemplo a seguir mostra uma solicitação para consultar atribuições de função qualificadas, incluindo as que são ativas e não ativas:</span><span class="sxs-lookup"><span data-stu-id="9e683-169">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>

# <a name="http"></a>[<span data-ttu-id="9e683-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e683-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
# <a name="c"></a>[<span data-ttu-id="9e683-171">C#</span><span class="sxs-lookup"><span data-stu-id="9e683-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e683-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e683-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e683-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e683-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9e683-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e683-174">Response</span></span> 
<span data-ttu-id="9e683-175">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="9e683-175">The following example shows the response.</span></span> <span data-ttu-id="9e683-176">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="9e683-176">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9e683-177">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e683-177">All of the properties will be returned from an actual call.</span></span>
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
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": true,
            "expirationDateTime": "2017-07-25T18:42:26.823Z",
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_194ae4cb-b126-40b2-bd5b-6091b380977d",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "194ae4cb-b126-40b2-bd5b-6091b380977d",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_9360feb5-f418-4baa-8175-e2a00bac4301",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "9360feb5-f418-4baa-8175-e2a00bac4301",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


