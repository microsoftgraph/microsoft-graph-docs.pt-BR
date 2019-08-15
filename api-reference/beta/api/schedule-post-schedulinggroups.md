---
title: Criar schedulingGroup
description: Criar um novo.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 75d464f2f3525841867131855b91580ab97e63d6
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410728"
---
# <a name="create-schedulinggroup"></a><span data-ttu-id="ddfda-103">Criar schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="ddfda-103">Create schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddfda-104">Criar um novo [](../resources/schedulinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="ddfda-104">Create a new [schedulingGroup](../resources/schedulinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ddfda-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ddfda-105">Permissions</span></span>

<span data-ttu-id="ddfda-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddfda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddfda-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddfda-108">Permission type</span></span>      | <span data-ttu-id="ddfda-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ddfda-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddfda-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddfda-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ddfda-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddfda-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ddfda-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddfda-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddfda-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddfda-113">Not supported.</span></span>    |
|<span data-ttu-id="ddfda-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddfda-114">Application</span></span> | <span data-ttu-id="ddfda-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddfda-115">Not supported.</span></span> |

> <span data-ttu-id="ddfda-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="ddfda-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ddfda-117">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="ddfda-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ddfda-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddfda-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="ddfda-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddfda-119">Request headers</span></span>

| <span data-ttu-id="ddfda-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ddfda-120">Header</span></span>       | <span data-ttu-id="ddfda-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ddfda-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ddfda-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddfda-122">Authorization</span></span>  | <span data-ttu-id="ddfda-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddfda-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ddfda-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ddfda-125">Content-Type</span></span>  | <span data-ttu-id="ddfda-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ddfda-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="ddfda-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddfda-127">Response</span></span>

<span data-ttu-id="ddfda-128">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto de forma de [plano](../resources/schedulinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddfda-128">If successful, this method returns a `201 Created` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddfda-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ddfda-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ddfda-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddfda-130">Request</span></span>

<span data-ttu-id="ddfda-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddfda-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ddfda-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddfda-132">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ddfda-133">C#</span><span class="sxs-lookup"><span data-stu-id="ddfda-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ddfda-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddfda-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ddfda-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ddfda-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ddfda-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddfda-136">Response</span></span>

<span data-ttu-id="ddfda-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddfda-137">The following is an example of the response.</span></span> 

><span data-ttu-id="ddfda-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddfda-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
