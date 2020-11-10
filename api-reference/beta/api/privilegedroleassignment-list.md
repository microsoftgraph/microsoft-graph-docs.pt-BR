---
title: Listar privilegedRoleAssignments
description: Recupere uma lista de objetos privilegedRoleAssignment, que correspondem a todas as atribuições de função da organização.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 529fb8f5d43d9fe4c60ccc9161edf3466680a7f8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971610"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="af0ef-103">Listar privilegedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="af0ef-103">List privilegedRoleAssignments</span></span>

<span data-ttu-id="af0ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af0ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af0ef-105">Recupere uma lista de objetos [privilegedRoleAssignment](../resources/privilegedroleassignment.md) , que correspondem a todas as atribuições de função da organização.</span><span class="sxs-lookup"><span data-stu-id="af0ef-105">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="af0ef-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="af0ef-106">Permissions</span></span>
<span data-ttu-id="af0ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af0ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="af0ef-109">O solicitante precisa ter uma das seguintes funções: administrador de _função privilegiada_ , _administrador global_ , _administrador de segurança_ ou _leitor de segurança_.</span><span class="sxs-lookup"><span data-stu-id="af0ef-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_ , _Global Administrator_ , _Security Administrator_ , or _Security Reader_.</span></span> 

|<span data-ttu-id="af0ef-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af0ef-110">Permission type</span></span>      | <span data-ttu-id="af0ef-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af0ef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af0ef-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af0ef-112">Delegated (work or school account)</span></span> | <span data-ttu-id="af0ef-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="af0ef-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="af0ef-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af0ef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af0ef-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af0ef-115">Not supported.</span></span>    |
|<span data-ttu-id="af0ef-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af0ef-116">Application</span></span> | <span data-ttu-id="af0ef-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af0ef-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="af0ef-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af0ef-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="af0ef-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="af0ef-119">Optional query parameters</span></span>
<span data-ttu-id="af0ef-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="af0ef-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="af0ef-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af0ef-121">Request headers</span></span>
| <span data-ttu-id="af0ef-122">Nome</span><span class="sxs-lookup"><span data-stu-id="af0ef-122">Name</span></span>      |<span data-ttu-id="af0ef-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="af0ef-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="af0ef-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="af0ef-124">Authorization</span></span>  | <span data-ttu-id="af0ef-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af0ef-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af0ef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af0ef-127">Request body</span></span>
<span data-ttu-id="af0ef-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="af0ef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af0ef-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="af0ef-129">Response</span></span>

<span data-ttu-id="af0ef-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af0ef-130">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="af0ef-131">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="af0ef-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="af0ef-132">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="af0ef-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="af0ef-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="af0ef-133">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="af0ef-134">Obter todas as atribuições de função</span><span class="sxs-lookup"><span data-stu-id="af0ef-134">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="af0ef-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af0ef-135">Request</span></span>
<span data-ttu-id="af0ef-136">O exemplo a seguir mostra uma solicitação para obter todas as atribuições de função:</span><span class="sxs-lookup"><span data-stu-id="af0ef-136">The following example shows a request to get all role assignments:</span></span>

# <a name="http"></a>[<span data-ttu-id="af0ef-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="af0ef-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="af0ef-138">C#</span><span class="sxs-lookup"><span data-stu-id="af0ef-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af0ef-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af0ef-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af0ef-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af0ef-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="af0ef-141">Java</span><span class="sxs-lookup"><span data-stu-id="af0ef-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="af0ef-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="af0ef-142">Response</span></span>
<span data-ttu-id="af0ef-143">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="af0ef-143">The following example shows the response.</span></span> <span data-ttu-id="af0ef-144">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="af0ef-144">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="af0ef-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af0ef-145">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-active-role-assignments"></a><span data-ttu-id="af0ef-146">Obter atribuições de função ativas</span><span class="sxs-lookup"><span data-stu-id="af0ef-146">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="af0ef-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af0ef-147">Request</span></span> 
<span data-ttu-id="af0ef-148">O exemplo a seguir mostra uma solicitação para consultar as atribuições de função ativas:</span><span class="sxs-lookup"><span data-stu-id="af0ef-148">The following example shows a request to query active role assignments:</span></span>

# <a name="http"></a>[<span data-ttu-id="af0ef-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="af0ef-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
# <a name="c"></a>[<span data-ttu-id="af0ef-150">C#</span><span class="sxs-lookup"><span data-stu-id="af0ef-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af0ef-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af0ef-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af0ef-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af0ef-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="af0ef-153">Java</span><span class="sxs-lookup"><span data-stu-id="af0ef-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="af0ef-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="af0ef-154">Response</span></span>
<span data-ttu-id="af0ef-155">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="af0ef-155">The following example shows the response.</span></span> <span data-ttu-id="af0ef-156">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="af0ef-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="af0ef-157">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af0ef-157">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="af0ef-158">Obter atribuições de função permanentes</span><span class="sxs-lookup"><span data-stu-id="af0ef-158">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="af0ef-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af0ef-159">Request</span></span> 
<span data-ttu-id="af0ef-160">O exemplo a seguir mostra uma solicitação para consultar atribuições de função permanentes, onde ``expirationDateTime`` Value é ``null`` :</span><span class="sxs-lookup"><span data-stu-id="af0ef-160">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>

# <a name="http"></a>[<span data-ttu-id="af0ef-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="af0ef-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
# <a name="c"></a>[<span data-ttu-id="af0ef-162">C#</span><span class="sxs-lookup"><span data-stu-id="af0ef-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af0ef-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af0ef-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af0ef-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af0ef-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="af0ef-165">Java</span><span class="sxs-lookup"><span data-stu-id="af0ef-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="af0ef-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="af0ef-166">Response</span></span>
<span data-ttu-id="af0ef-167">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="af0ef-167">The following example shows the response.</span></span> <span data-ttu-id="af0ef-168">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="af0ef-168">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="af0ef-169">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af0ef-169">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="af0ef-170">Obter atribuições de função qualificadas</span><span class="sxs-lookup"><span data-stu-id="af0ef-170">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="af0ef-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af0ef-171">Request</span></span> 
<span data-ttu-id="af0ef-172">O exemplo a seguir mostra uma solicitação para consultar atribuições de função qualificadas, incluindo as que são ativas e não ativas:</span><span class="sxs-lookup"><span data-stu-id="af0ef-172">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>

# <a name="http"></a>[<span data-ttu-id="af0ef-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="af0ef-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
# <a name="c"></a>[<span data-ttu-id="af0ef-174">C#</span><span class="sxs-lookup"><span data-stu-id="af0ef-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af0ef-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af0ef-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af0ef-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af0ef-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="af0ef-177">Java</span><span class="sxs-lookup"><span data-stu-id="af0ef-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="af0ef-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="af0ef-178">Response</span></span> 
<span data-ttu-id="af0ef-179">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="af0ef-179">The following example shows the response.</span></span> <span data-ttu-id="af0ef-180">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="af0ef-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="af0ef-181">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af0ef-181">All of the properties will be returned from an actual call.</span></span>
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
