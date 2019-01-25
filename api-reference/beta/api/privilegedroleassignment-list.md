---
title: Lista privilegedRoleAssignments
description: Recupere uma lista dos objetos de privilegedRoleAssignment, que correspondem a todas as atribuições de função para a organização.
localization_priority: Normal
ms.openlocfilehash: c576e0d9c0a278e02159e02cea94ddd927561e08
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516585"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="7721e-103">Lista privilegedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="7721e-103">List privilegedRoleAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7721e-104">Recupere uma lista dos objetos de [privilegedRoleAssignment](../resources/privilegedroleassignment.md) , que correspondem a todas as atribuições de função para a organização.</span><span class="sxs-lookup"><span data-stu-id="7721e-104">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="7721e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7721e-105">Permissions</span></span>
<span data-ttu-id="7721e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7721e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7721e-108">O solicitante precisa ter uma das seguintes funções: _Leitor de segurança_, _Administrador Global_, _Administrador de segurança_ou _Administrador com privilégios de função_.</span><span class="sxs-lookup"><span data-stu-id="7721e-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="7721e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7721e-109">Permission type</span></span>      | <span data-ttu-id="7721e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7721e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7721e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7721e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7721e-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7721e-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7721e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7721e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7721e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7721e-114">Not supported.</span></span>    |
|<span data-ttu-id="7721e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7721e-115">Application</span></span> | <span data-ttu-id="7721e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7721e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7721e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7721e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7721e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7721e-118">Optional query parameters</span></span>
<span data-ttu-id="7721e-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7721e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7721e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7721e-120">Request headers</span></span>
| <span data-ttu-id="7721e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7721e-121">Name</span></span>      |<span data-ttu-id="7721e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7721e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7721e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7721e-123">Authorization</span></span>  | <span data-ttu-id="7721e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7721e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7721e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7721e-126">Request body</span></span>
<span data-ttu-id="7721e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7721e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7721e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7721e-128">Response</span></span>

<span data-ttu-id="7721e-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7721e-129">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="7721e-130">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="7721e-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="7721e-131">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="7721e-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="7721e-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7721e-132">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="7721e-133">Obtenha todas as atribuições de função</span><span class="sxs-lookup"><span data-stu-id="7721e-133">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="7721e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7721e-134">Request</span></span>
<span data-ttu-id="7721e-135">O exemplo a seguir mostra uma solicitação para obter todas as atribuições de função:</span><span class="sxs-lookup"><span data-stu-id="7721e-135">The following example shows a request to get all role assignments:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
##### <a name="response"></a><span data-ttu-id="7721e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7721e-136">Response</span></span>
<span data-ttu-id="7721e-137">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="7721e-137">The following example shows the response.</span></span> <span data-ttu-id="7721e-138">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="7721e-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7721e-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7721e-139">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-active-role-assignments"></a><span data-ttu-id="7721e-140">Obtenha as atribuições de função ativo</span><span class="sxs-lookup"><span data-stu-id="7721e-140">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="7721e-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7721e-141">Request</span></span> 
<span data-ttu-id="7721e-142">O exemplo a seguir mostra uma solicitação para atribuições de função ativo de consulta:</span><span class="sxs-lookup"><span data-stu-id="7721e-142">The following example shows a request to query active role assignments:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
##### <a name="response"></a><span data-ttu-id="7721e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7721e-143">Response</span></span>
<span data-ttu-id="7721e-144">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="7721e-144">The following example shows the response.</span></span> <span data-ttu-id="7721e-145">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="7721e-145">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7721e-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7721e-146">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="7721e-147">Obtenha as atribuições de função permanente</span><span class="sxs-lookup"><span data-stu-id="7721e-147">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="7721e-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7721e-148">Request</span></span> 
<span data-ttu-id="7721e-149">O exemplo a seguir mostra uma solicitação para atribuições de função permanente de consulta, onde ``expirationDateTime`` valor é ``null``:</span><span class="sxs-lookup"><span data-stu-id="7721e-149">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
##### <a name="response"></a><span data-ttu-id="7721e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="7721e-150">Response</span></span>
<span data-ttu-id="7721e-151">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="7721e-151">The following example shows the response.</span></span> <span data-ttu-id="7721e-152">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="7721e-152">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7721e-153">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7721e-153">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="7721e-154">Obtenha as atribuições de função elegíveis</span><span class="sxs-lookup"><span data-stu-id="7721e-154">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="7721e-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7721e-155">Request</span></span> 
<span data-ttu-id="7721e-156">O exemplo a seguir mostra uma solicitação para atribuições de função elegíveis de consulta, incluindo aqueles ativas e não estiver ativo:</span><span class="sxs-lookup"><span data-stu-id="7721e-156">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
##### <a name="response"></a><span data-ttu-id="7721e-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="7721e-157">Response</span></span> 
<span data-ttu-id="7721e-158">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="7721e-158">The following example shows the response.</span></span> <span data-ttu-id="7721e-159">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="7721e-159">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7721e-160">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7721e-160">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/privilegedroleassignment-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
