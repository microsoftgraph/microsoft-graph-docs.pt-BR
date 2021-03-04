---
title: Listar privilegedRoleAssignments
description: Recupere uma lista de objetos privilegedRoleAssignment, que correspondem a todas as atribuições de função para a organização.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: a7dc26effcc7d43348e05f57dc54e1f908ea79c7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441225"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="fec2b-103">Listar privilegedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="fec2b-103">List privilegedRoleAssignments</span></span>

<span data-ttu-id="fec2b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fec2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fec2b-105">Recupere uma lista de [objetos privilegedRoleAssignment,](../resources/privilegedroleassignment.md) que correspondem a todas as atribuições de função para a organização.</span><span class="sxs-lookup"><span data-stu-id="fec2b-105">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="fec2b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fec2b-106">Permissions</span></span>
<span data-ttu-id="fec2b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fec2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="fec2b-109">O solicitante precisa ter uma das seguintes funções: Administrador de Função _Privilegiada,_ _Administrador Global,_ Administrador de Segurança _ou_ Leitor de _Segurança._</span><span class="sxs-lookup"><span data-stu-id="fec2b-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="fec2b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fec2b-110">Permission type</span></span>      | <span data-ttu-id="fec2b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fec2b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fec2b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fec2b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fec2b-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fec2b-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fec2b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fec2b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fec2b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fec2b-115">Not supported.</span></span>    |
|<span data-ttu-id="fec2b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fec2b-116">Application</span></span> | <span data-ttu-id="fec2b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fec2b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fec2b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fec2b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fec2b-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fec2b-119">Optional query parameters</span></span>
<span data-ttu-id="fec2b-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fec2b-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fec2b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fec2b-121">Request headers</span></span>
| <span data-ttu-id="fec2b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="fec2b-122">Name</span></span>      |<span data-ttu-id="fec2b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fec2b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fec2b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fec2b-124">Authorization</span></span>  | <span data-ttu-id="fec2b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fec2b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fec2b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fec2b-127">Request body</span></span>
<span data-ttu-id="fec2b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fec2b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fec2b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fec2b-129">Response</span></span>

<span data-ttu-id="fec2b-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fec2b-130">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="fec2b-131">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="fec2b-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="fec2b-132">Caso contrário, o código de status HTTP 403 Forbidden será retornado.</span><span class="sxs-lookup"><span data-stu-id="fec2b-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="fec2b-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fec2b-133">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="fec2b-134">Obter todas as atribuições de função</span><span class="sxs-lookup"><span data-stu-id="fec2b-134">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="fec2b-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fec2b-135">Request</span></span>
<span data-ttu-id="fec2b-136">O exemplo a seguir mostra uma solicitação para obter todas as atribuições de função:</span><span class="sxs-lookup"><span data-stu-id="fec2b-136">The following example shows a request to get all role assignments:</span></span>

# <a name="http"></a>[<span data-ttu-id="fec2b-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="fec2b-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="fec2b-138">C#</span><span class="sxs-lookup"><span data-stu-id="fec2b-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fec2b-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fec2b-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fec2b-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fec2b-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fec2b-141">Java</span><span class="sxs-lookup"><span data-stu-id="fec2b-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fec2b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="fec2b-142">Response</span></span>
<span data-ttu-id="fec2b-143">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="fec2b-143">The following example shows the response.</span></span> <span data-ttu-id="fec2b-144">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="fec2b-144">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fec2b-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fec2b-145">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-active-role-assignments"></a><span data-ttu-id="fec2b-146">Obter atribuições de função ativa</span><span class="sxs-lookup"><span data-stu-id="fec2b-146">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="fec2b-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fec2b-147">Request</span></span> 
<span data-ttu-id="fec2b-148">O exemplo a seguir mostra uma solicitação para consultar atribuições de função ativa:</span><span class="sxs-lookup"><span data-stu-id="fec2b-148">The following example shows a request to query active role assignments:</span></span>

# <a name="http"></a>[<span data-ttu-id="fec2b-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="fec2b-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
# <a name="c"></a>[<span data-ttu-id="fec2b-150">C#</span><span class="sxs-lookup"><span data-stu-id="fec2b-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fec2b-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fec2b-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fec2b-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fec2b-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fec2b-153">Java</span><span class="sxs-lookup"><span data-stu-id="fec2b-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fec2b-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="fec2b-154">Response</span></span>
<span data-ttu-id="fec2b-155">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="fec2b-155">The following example shows the response.</span></span> <span data-ttu-id="fec2b-156">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="fec2b-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fec2b-157">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fec2b-157">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="fec2b-158">Obter atribuições de função permanente</span><span class="sxs-lookup"><span data-stu-id="fec2b-158">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="fec2b-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fec2b-159">Request</span></span> 
<span data-ttu-id="fec2b-160">O exemplo a seguir mostra uma solicitação para consultar atribuições de função permanente, onde ``expirationDateTime`` o valor é ``null`` :</span><span class="sxs-lookup"><span data-stu-id="fec2b-160">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>

# <a name="http"></a>[<span data-ttu-id="fec2b-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="fec2b-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
# <a name="c"></a>[<span data-ttu-id="fec2b-162">C#</span><span class="sxs-lookup"><span data-stu-id="fec2b-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fec2b-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fec2b-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fec2b-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fec2b-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fec2b-165">Java</span><span class="sxs-lookup"><span data-stu-id="fec2b-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fec2b-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="fec2b-166">Response</span></span>
<span data-ttu-id="fec2b-167">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="fec2b-167">The following example shows the response.</span></span> <span data-ttu-id="fec2b-168">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="fec2b-168">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fec2b-169">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fec2b-169">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="fec2b-170">Obter atribuições de função qualificadas</span><span class="sxs-lookup"><span data-stu-id="fec2b-170">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="fec2b-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fec2b-171">Request</span></span> 
<span data-ttu-id="fec2b-172">O exemplo a seguir mostra uma solicitação para consultar atribuições de função qualificadas, incluindo as ativas e não ativas:</span><span class="sxs-lookup"><span data-stu-id="fec2b-172">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>

# <a name="http"></a>[<span data-ttu-id="fec2b-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="fec2b-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
# <a name="c"></a>[<span data-ttu-id="fec2b-174">C#</span><span class="sxs-lookup"><span data-stu-id="fec2b-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fec2b-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fec2b-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fec2b-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fec2b-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fec2b-177">Java</span><span class="sxs-lookup"><span data-stu-id="fec2b-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fec2b-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="fec2b-178">Response</span></span> 
<span data-ttu-id="fec2b-179">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="fec2b-179">The following example shows the response.</span></span> <span data-ttu-id="fec2b-180">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="fec2b-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fec2b-181">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fec2b-181">All of the properties will be returned from an actual call.</span></span>
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
