---
title: Listar privilegedRoleAssignments
description: Recupere uma lista de objetos privilegedRoleAssignment, que correspondem a todas as atribuições de função da organização.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 31bbf6221c4d8b9fc021aabd8678acb7c64b74a2
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412726"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="db66b-103">Listar privilegedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="db66b-103">List privilegedRoleAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db66b-104">Recupere uma lista de objetos [privilegedRoleAssignment](../resources/privilegedroleassignment.md) , que correspondem a todas as atribuições de função da organização.</span><span class="sxs-lookup"><span data-stu-id="db66b-104">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="db66b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="db66b-105">Permissions</span></span>
<span data-ttu-id="db66b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db66b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="db66b-108">O solicitante precisa ter uma das seguintes funções: administrador de _função privilegiada_, _administrador global_, _administrador de segurança_ou _leitor de segurança_.</span><span class="sxs-lookup"><span data-stu-id="db66b-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="db66b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db66b-109">Permission type</span></span>      | <span data-ttu-id="db66b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db66b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db66b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db66b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="db66b-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="db66b-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="db66b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db66b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db66b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db66b-114">Not supported.</span></span>    |
|<span data-ttu-id="db66b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db66b-115">Application</span></span> | <span data-ttu-id="db66b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db66b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="db66b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db66b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="db66b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="db66b-118">Optional query parameters</span></span>
<span data-ttu-id="db66b-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="db66b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="db66b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db66b-120">Request headers</span></span>
| <span data-ttu-id="db66b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="db66b-121">Name</span></span>      |<span data-ttu-id="db66b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="db66b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="db66b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="db66b-123">Authorization</span></span>  | <span data-ttu-id="db66b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db66b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db66b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db66b-126">Request body</span></span>
<span data-ttu-id="db66b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="db66b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db66b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="db66b-128">Response</span></span>

<span data-ttu-id="db66b-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db66b-129">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="db66b-130">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="db66b-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="db66b-131">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="db66b-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="db66b-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="db66b-132">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="db66b-133">Obter todas as atribuições de função</span><span class="sxs-lookup"><span data-stu-id="db66b-133">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="db66b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db66b-134">Request</span></span>
<span data-ttu-id="db66b-135">O exemplo a seguir mostra uma solicitação para obter todas as atribuições de função:</span><span class="sxs-lookup"><span data-stu-id="db66b-135">The following example shows a request to get all role assignments:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="db66b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="db66b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db66b-137">C#</span><span class="sxs-lookup"><span data-stu-id="db66b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db66b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db66b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db66b-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="db66b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="db66b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="db66b-140">Response</span></span>
<span data-ttu-id="db66b-141">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="db66b-141">The following example shows the response.</span></span> <span data-ttu-id="db66b-142">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="db66b-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="db66b-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db66b-143">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-active-role-assignments"></a><span data-ttu-id="db66b-144">Obter atribuições de função ativas</span><span class="sxs-lookup"><span data-stu-id="db66b-144">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="db66b-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db66b-145">Request</span></span> 
<span data-ttu-id="db66b-146">O exemplo a seguir mostra uma solicitação para consultar as atribuições de função ativas:</span><span class="sxs-lookup"><span data-stu-id="db66b-146">The following example shows a request to query active role assignments:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="db66b-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="db66b-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db66b-148">C#</span><span class="sxs-lookup"><span data-stu-id="db66b-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db66b-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db66b-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db66b-150">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="db66b-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="db66b-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="db66b-151">Response</span></span>
<span data-ttu-id="db66b-152">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="db66b-152">The following example shows the response.</span></span> <span data-ttu-id="db66b-153">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="db66b-153">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="db66b-154">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db66b-154">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="db66b-155">Obter atribuições de função permanentes</span><span class="sxs-lookup"><span data-stu-id="db66b-155">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="db66b-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db66b-156">Request</span></span> 
<span data-ttu-id="db66b-157">O exemplo a seguir mostra uma solicitação para consultar atribuições de função ``expirationDateTime`` permanentes ``null``, onde Value é:</span><span class="sxs-lookup"><span data-stu-id="db66b-157">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="db66b-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="db66b-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db66b-159">C#</span><span class="sxs-lookup"><span data-stu-id="db66b-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db66b-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db66b-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db66b-161">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="db66b-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="db66b-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="db66b-162">Response</span></span>
<span data-ttu-id="db66b-163">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="db66b-163">The following example shows the response.</span></span> <span data-ttu-id="db66b-164">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="db66b-164">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="db66b-165">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db66b-165">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="db66b-166">Obter atribuições de função qualificadas</span><span class="sxs-lookup"><span data-stu-id="db66b-166">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="db66b-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db66b-167">Request</span></span> 
<span data-ttu-id="db66b-168">O exemplo a seguir mostra uma solicitação para consultar atribuições de função qualificadas, incluindo as que são ativas e não ativas:</span><span class="sxs-lookup"><span data-stu-id="db66b-168">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="db66b-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="db66b-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db66b-170">C#</span><span class="sxs-lookup"><span data-stu-id="db66b-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db66b-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db66b-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db66b-172">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="db66b-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="db66b-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="db66b-173">Response</span></span> 
<span data-ttu-id="db66b-174">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="db66b-174">The following example shows the response.</span></span> <span data-ttu-id="db66b-175">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="db66b-175">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="db66b-176">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db66b-176">All of the properties will be returned from an actual call.</span></span>
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
