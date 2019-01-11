---
title: Criar appRoleAssignment
description: Use essa API para criar um novo appRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: ce498312f294ff11b97f12b136a6f48ebb4d3791
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886979"
---
# <a name="create-approleassignment"></a><span data-ttu-id="563b9-103">Criar appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="563b9-103">Create appRoleAssignment</span></span>

> <span data-ttu-id="563b9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="563b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="563b9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="563b9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="563b9-106">Use essa API para criar um novo appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="563b9-106">Use this API to create a new appRoleAssignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="563b9-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="563b9-107">Permissions</span></span>
<span data-ttu-id="563b9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="563b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="563b9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="563b9-110">Permission type</span></span>      | <span data-ttu-id="563b9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="563b9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="563b9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="563b9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="563b9-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="563b9-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="563b9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="563b9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="563b9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="563b9-115">Not supported.</span></span>    |
|<span data-ttu-id="563b9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="563b9-116">Application</span></span> | <span data-ttu-id="563b9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="563b9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="563b9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="563b9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments

```
## <a name="request-headers"></a><span data-ttu-id="563b9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="563b9-119">Request headers</span></span>
| <span data-ttu-id="563b9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="563b9-120">Name</span></span>       | <span data-ttu-id="563b9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="563b9-121">Type</span></span> | <span data-ttu-id="563b9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="563b9-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="563b9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="563b9-123">Authorization</span></span>  | <span data-ttu-id="563b9-124">string</span><span class="sxs-lookup"><span data-stu-id="563b9-124">string</span></span>  | <span data-ttu-id="563b9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="563b9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="563b9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="563b9-127">Request body</span></span>
<span data-ttu-id="563b9-128">No corpo da solicitação, fornece uma representação JSON do objeto [appRoleAssignment](../resources/approleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="563b9-128">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="563b9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="563b9-129">Response</span></span>

<span data-ttu-id="563b9-130">Se tiver êxito, este método retornará `201 Created` objeto response de código e [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="563b9-130">If successful, this method returns `201 Created` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="563b9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="563b9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="563b9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="563b9-132">Request</span></span>
<span data-ttu-id="563b9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="563b9-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_approleassignment_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
Content-type: application/json
Content-length: 233

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```
<span data-ttu-id="563b9-134">No corpo da solicitação, fornece uma representação JSON do objeto [appRoleAssignment](../resources/approleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="563b9-134">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="563b9-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="563b9-135">Response</span></span>
<span data-ttu-id="563b9-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="563b9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
