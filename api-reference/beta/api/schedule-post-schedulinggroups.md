---
title: Criar schedulingGroup
description: Criar um novo.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 36e3399a1de4a5792f205331f3aa408a871ca836
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982954"
---
# <a name="create-schedulinggroup"></a><span data-ttu-id="fdbcc-103">Criar schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="fdbcc-103">Create schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdbcc-104">Criar um novo [](../resources/schedulinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="fdbcc-104">Create a new [schedulingGroup](../resources/schedulinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fdbcc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fdbcc-105">Permissions</span></span>

<span data-ttu-id="fdbcc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdbcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdbcc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdbcc-108">Permission type</span></span>      | <span data-ttu-id="fdbcc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fdbcc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdbcc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdbcc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fdbcc-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdbcc-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fdbcc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdbcc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdbcc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdbcc-113">Not supported.</span></span>    |
|<span data-ttu-id="fdbcc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdbcc-114">Application</span></span> | <span data-ttu-id="fdbcc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdbcc-115">Not supported.</span></span> |

> <span data-ttu-id="fdbcc-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="fdbcc-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="fdbcc-117">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="fdbcc-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="fdbcc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdbcc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="fdbcc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdbcc-119">Request headers</span></span>

| <span data-ttu-id="fdbcc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fdbcc-120">Header</span></span>       | <span data-ttu-id="fdbcc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fdbcc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fdbcc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdbcc-122">Authorization</span></span>  | <span data-ttu-id="fdbcc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdbcc-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fdbcc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fdbcc-125">Content-Type</span></span>  | <span data-ttu-id="fdbcc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fdbcc-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="fdbcc-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdbcc-127">Response</span></span>

<span data-ttu-id="fdbcc-128">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto de forma de [plano](../resources/schedulinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdbcc-128">If successful, this method returns a `201 Created` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdbcc-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdbcc-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fdbcc-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdbcc-130">Request</span></span>

<span data-ttu-id="fdbcc-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdbcc-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fdbcc-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="fdbcc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-post-schedulinggroups"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups
Content-type: application/json

{
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fdbcc-133">C#</span><span class="sxs-lookup"><span data-stu-id="fdbcc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fdbcc-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="fdbcc-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fdbcc-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fdbcc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fdbcc-136">Java</span><span class="sxs-lookup"><span data-stu-id="fdbcc-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-post-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fdbcc-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdbcc-137">Response</span></span>

<span data-ttu-id="fdbcc-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fdbcc-138">The following is an example of the response.</span></span> 

><span data-ttu-id="fdbcc-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fdbcc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates a new schedulingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
