---
title: Lista privilegedRoleAssignments
description: Recupere uma lista dos objetos de privilegedRoleAssignment, que correspondem a todas as atribuições de função para a organização.
localization_priority: Normal
ms.openlocfilehash: ee6fac823e4d05eb13ada0a3ad1082ba1a78a7e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838658"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="14878-103">Lista privilegedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="14878-103">List privilegedRoleAssignments</span></span>

> <span data-ttu-id="14878-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="14878-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14878-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="14878-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="14878-106">Recupere uma lista dos objetos de [privilegedRoleAssignment](../resources/privilegedroleassignment.md) , que correspondem a todas as atribuições de função para a organização.</span><span class="sxs-lookup"><span data-stu-id="14878-106">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="14878-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="14878-107">Permissions</span></span>
<span data-ttu-id="14878-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14878-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="14878-110">O solicitante precisa ter uma das seguintes funções: _Leitor de segurança_, _Administrador Global_, _Administrador de segurança_ou _Administrador com privilégios de função_.</span><span class="sxs-lookup"><span data-stu-id="14878-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="14878-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14878-111">Permission type</span></span>      | <span data-ttu-id="14878-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="14878-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14878-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14878-113">Delegated (work or school account)</span></span> | <span data-ttu-id="14878-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="14878-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="14878-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14878-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14878-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14878-116">Not supported.</span></span>    |
|<span data-ttu-id="14878-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14878-117">Application</span></span> | <span data-ttu-id="14878-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14878-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="14878-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14878-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="14878-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="14878-120">Optional query parameters</span></span>
<span data-ttu-id="14878-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="14878-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="14878-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14878-122">Request headers</span></span>
| <span data-ttu-id="14878-123">Nome</span><span class="sxs-lookup"><span data-stu-id="14878-123">Name</span></span>      |<span data-ttu-id="14878-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="14878-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="14878-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="14878-125">Authorization</span></span>  | <span data-ttu-id="14878-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14878-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14878-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14878-128">Request body</span></span>
<span data-ttu-id="14878-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="14878-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14878-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="14878-130">Response</span></span>

<span data-ttu-id="14878-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14878-131">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="14878-132">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="14878-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="14878-133">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="14878-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="14878-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="14878-134">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="14878-135">Obtenha todas as atribuições de função</span><span class="sxs-lookup"><span data-stu-id="14878-135">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="14878-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14878-136">Request</span></span>
<span data-ttu-id="14878-137">O exemplo a seguir mostra uma solicitação para obter todas as atribuições de função:</span><span class="sxs-lookup"><span data-stu-id="14878-137">The following example shows a request to get all role assignments:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
##### <a name="response"></a><span data-ttu-id="14878-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="14878-138">Response</span></span>
<span data-ttu-id="14878-139">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="14878-139">The following example shows the response.</span></span> <span data-ttu-id="14878-140">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="14878-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="14878-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14878-141">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-active-role-assignments"></a><span data-ttu-id="14878-142">Obtenha as atribuições de função ativo</span><span class="sxs-lookup"><span data-stu-id="14878-142">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="14878-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14878-143">Request</span></span> 
<span data-ttu-id="14878-144">O exemplo a seguir mostra uma solicitação para atribuições de função ativo de consulta:</span><span class="sxs-lookup"><span data-stu-id="14878-144">The following example shows a request to query active role assignments:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
##### <a name="response"></a><span data-ttu-id="14878-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="14878-145">Response</span></span>
<span data-ttu-id="14878-146">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="14878-146">The following example shows the response.</span></span> <span data-ttu-id="14878-147">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="14878-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="14878-148">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14878-148">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="14878-149">Obtenha as atribuições de função permanente</span><span class="sxs-lookup"><span data-stu-id="14878-149">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="14878-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14878-150">Request</span></span> 
<span data-ttu-id="14878-151">O exemplo a seguir mostra uma solicitação para atribuições de função permanente de consulta, onde ``expirationDateTime`` valor é ``null``:</span><span class="sxs-lookup"><span data-stu-id="14878-151">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
##### <a name="response"></a><span data-ttu-id="14878-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="14878-152">Response</span></span>
<span data-ttu-id="14878-153">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="14878-153">The following example shows the response.</span></span> <span data-ttu-id="14878-154">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="14878-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="14878-155">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14878-155">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="14878-156">Obtenha as atribuições de função elegíveis</span><span class="sxs-lookup"><span data-stu-id="14878-156">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="14878-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14878-157">Request</span></span> 
<span data-ttu-id="14878-158">O exemplo a seguir mostra uma solicitação para atribuições de função elegíveis de consulta, incluindo aqueles ativas e não estiver ativo:</span><span class="sxs-lookup"><span data-stu-id="14878-158">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
##### <a name="response"></a><span data-ttu-id="14878-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="14878-159">Response</span></span> 
<span data-ttu-id="14878-160">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="14878-160">The following example shows the response.</span></span> <span data-ttu-id="14878-161">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="14878-161">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="14878-162">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14878-162">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
