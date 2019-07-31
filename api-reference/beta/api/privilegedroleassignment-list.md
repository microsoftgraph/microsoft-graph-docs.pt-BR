---
title: Listar privilegedRoleAssignments
description: Recupere uma lista de objetos privilegedRoleAssignment, que correspondem a todas as atribuições de função da organização.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4a55d33bf6c9bcecc8a1c643176a630648f7e379
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983373"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="0a7b6-103">Listar privilegedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="0a7b6-103">List privilegedRoleAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a7b6-104">Recupere uma lista de objetos [privilegedRoleAssignment](../resources/privilegedroleassignment.md) , que correspondem a todas as atribuições de função da organização.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-104">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="0a7b6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0a7b6-105">Permissions</span></span>
<span data-ttu-id="0a7b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a7b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0a7b6-108">O solicitante precisa ter uma das seguintes funções: administrador de _função privilegiada_, _administrador global_, _administrador de segurança_ou _leitor de segurança_.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="0a7b6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a7b6-109">Permission type</span></span>      | <span data-ttu-id="0a7b6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0a7b6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a7b6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a7b6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0a7b6-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0a7b6-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0a7b6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a7b6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a7b6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-114">Not supported.</span></span>    |
|<span data-ttu-id="0a7b6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a7b6-115">Application</span></span> | <span data-ttu-id="0a7b6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a7b6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a7b6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0a7b6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0a7b6-118">Optional query parameters</span></span>
<span data-ttu-id="0a7b6-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a7b6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a7b6-120">Request headers</span></span>
| <span data-ttu-id="0a7b6-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0a7b6-121">Name</span></span>      |<span data-ttu-id="0a7b6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a7b6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0a7b6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a7b6-123">Authorization</span></span>  | <span data-ttu-id="0a7b6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a7b6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a7b6-126">Request body</span></span>
<span data-ttu-id="0a7b6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a7b6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a7b6-128">Response</span></span>

<span data-ttu-id="0a7b6-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-129">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="0a7b6-130">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="0a7b6-131">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="0a7b6-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0a7b6-132">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="0a7b6-133">Obter todas as atribuições de função</span><span class="sxs-lookup"><span data-stu-id="0a7b6-133">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="0a7b6-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a7b6-134">Request</span></span>
<span data-ttu-id="0a7b6-135">O exemplo a seguir mostra uma solicitação para obter todas as atribuições de função:</span><span class="sxs-lookup"><span data-stu-id="0a7b6-135">The following example shows a request to get all role assignments:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0a7b6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a7b6-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0a7b6-137">C#</span><span class="sxs-lookup"><span data-stu-id="0a7b6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a7b6-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="0a7b6-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0a7b6-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0a7b6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0a7b6-140">Java</span><span class="sxs-lookup"><span data-stu-id="0a7b6-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0a7b6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a7b6-141">Response</span></span>
<span data-ttu-id="0a7b6-142">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-142">The following example shows the response.</span></span> <span data-ttu-id="0a7b6-143">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0a7b6-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-144">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-active-role-assignments"></a><span data-ttu-id="0a7b6-145">Obter atribuições de função ativas</span><span class="sxs-lookup"><span data-stu-id="0a7b6-145">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="0a7b6-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a7b6-146">Request</span></span> 
<span data-ttu-id="0a7b6-147">O exemplo a seguir mostra uma solicitação para consultar as atribuições de função ativas:</span><span class="sxs-lookup"><span data-stu-id="0a7b6-147">The following example shows a request to query active role assignments:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0a7b6-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a7b6-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0a7b6-149">C#</span><span class="sxs-lookup"><span data-stu-id="0a7b6-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a7b6-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="0a7b6-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0a7b6-151">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0a7b6-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0a7b6-152">Java</span><span class="sxs-lookup"><span data-stu-id="0a7b6-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0a7b6-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a7b6-153">Response</span></span>
<span data-ttu-id="0a7b6-154">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-154">The following example shows the response.</span></span> <span data-ttu-id="0a7b6-155">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-155">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0a7b6-156">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-156">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="0a7b6-157">Obter atribuições de função permanentes</span><span class="sxs-lookup"><span data-stu-id="0a7b6-157">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="0a7b6-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a7b6-158">Request</span></span> 
<span data-ttu-id="0a7b6-159">O exemplo a seguir mostra uma solicitação para consultar atribuições de função ``expirationDateTime`` permanentes ``null``, onde Value é:</span><span class="sxs-lookup"><span data-stu-id="0a7b6-159">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0a7b6-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a7b6-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0a7b6-161">C#</span><span class="sxs-lookup"><span data-stu-id="0a7b6-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a7b6-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="0a7b6-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0a7b6-163">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0a7b6-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0a7b6-164">Java</span><span class="sxs-lookup"><span data-stu-id="0a7b6-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0a7b6-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a7b6-165">Response</span></span>
<span data-ttu-id="0a7b6-166">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-166">The following example shows the response.</span></span> <span data-ttu-id="0a7b6-167">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-167">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0a7b6-168">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-168">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="0a7b6-169">Obter atribuições de função qualificadas</span><span class="sxs-lookup"><span data-stu-id="0a7b6-169">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="0a7b6-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a7b6-170">Request</span></span> 
<span data-ttu-id="0a7b6-171">O exemplo a seguir mostra uma solicitação para consultar atribuições de função qualificadas, incluindo as que são ativas e não ativas:</span><span class="sxs-lookup"><span data-stu-id="0a7b6-171">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0a7b6-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a7b6-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0a7b6-173">C#</span><span class="sxs-lookup"><span data-stu-id="0a7b6-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a7b6-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="0a7b6-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0a7b6-175">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0a7b6-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0a7b6-176">Java</span><span class="sxs-lookup"><span data-stu-id="0a7b6-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0a7b6-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a7b6-177">Response</span></span> 
<span data-ttu-id="0a7b6-178">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-178">The following example shows the response.</span></span> <span data-ttu-id="0a7b6-179">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-179">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0a7b6-180">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a7b6-180">All of the properties will be returned from an actual call.</span></span>
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
