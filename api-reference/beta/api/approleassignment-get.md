---
title: Obter appRoleAssignment
description: Recupere as propriedades e relações do objeto approleassignment.
localization_priority: Priority
ms.openlocfilehash: 465ef0365bee8c1dd002fa423232cc615fc45635
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809657"
---
# <a name="get-approleassignment"></a><span data-ttu-id="e3224-103">Obter appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e3224-103">Get appRoleAssignment</span></span>

> <span data-ttu-id="e3224-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e3224-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3224-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e3224-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e3224-106">Recupere as propriedades e relações do objeto approleassignment.</span><span class="sxs-lookup"><span data-stu-id="e3224-106">Retrieve the properties and relationships of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e3224-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="e3224-107">Permissions</span></span>
<span data-ttu-id="e3224-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3224-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3224-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3224-110">Permission type</span></span>      | <span data-ttu-id="e3224-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3224-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3224-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3224-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e3224-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e3224-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e3224-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3224-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3224-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3224-115">Not supported.</span></span>    |
|<span data-ttu-id="e3224-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3224-116">Application</span></span> | <span data-ttu-id="e3224-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3224-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3224-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3224-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/appRoleAssignments/{id}
GET /servicePrincipals/{id}/appRoleAssignedTo
GET /groups/{id}/appRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e3224-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e3224-119">Optional query parameters</span></span>
<span data-ttu-id="e3224-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e3224-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3224-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3224-121">Request headers</span></span>
| <span data-ttu-id="e3224-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e3224-122">Name</span></span>       | <span data-ttu-id="e3224-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3224-123">Type</span></span> | <span data-ttu-id="e3224-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3224-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e3224-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3224-125">Authorization</span></span>  | <span data-ttu-id="e3224-126">string</span><span class="sxs-lookup"><span data-stu-id="e3224-126">string</span></span>  | <span data-ttu-id="e3224-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3224-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3224-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3224-129">Request body</span></span>
<span data-ttu-id="e3224-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e3224-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3224-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3224-131">Response</span></span>

<span data-ttu-id="e3224-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3224-132">If successful, this method returns a `200 OK` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e3224-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3224-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3224-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3224-134">Request</span></span>
<span data-ttu-id="e3224-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3224-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_approleassignment"
}-->
```http
GET https://graph.microsoft.com/beta/appRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="e3224-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3224-136">Response</span></span>
<span data-ttu-id="e3224-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3224-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approleassignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
