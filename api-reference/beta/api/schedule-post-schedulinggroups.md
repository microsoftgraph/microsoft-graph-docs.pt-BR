---
title: Criar schedulingGroup
description: Criar um nov schedulingGroup.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b394515e8f69b49f42f9fb517b3077a2fb1d8ee3
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "42453825"
---
# <a name="create-schedulinggroup"></a><span data-ttu-id="f1fe1-103">Criar schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="f1fe1-103">Create schedulingGroup</span></span>

<span data-ttu-id="f1fe1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1fe1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1fe1-105">Criar um nov [schedulingGroup](../resources/schedulinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="f1fe1-105">Create a new [schedulingGroup](../resources/schedulinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f1fe1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1fe1-106">Permissions</span></span>

<span data-ttu-id="f1fe1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1fe1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1fe1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1fe1-109">Permission type</span></span>      | <span data-ttu-id="f1fe1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1fe1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1fe1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1fe1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f1fe1-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1fe1-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f1fe1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1fe1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1fe1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1fe1-114">Not supported.</span></span>    |
|<span data-ttu-id="f1fe1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1fe1-115">Application</span></span> |<span data-ttu-id="f1fe1-116">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="f1fe1-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="f1fe1-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="f1fe1-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="f1fe1-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="f1fe1-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f1fe1-119">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="f1fe1-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f1fe1-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1fe1-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="f1fe1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1fe1-121">Request headers</span></span>

| <span data-ttu-id="f1fe1-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1fe1-122">Header</span></span>       | <span data-ttu-id="f1fe1-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f1fe1-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f1fe1-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1fe1-124">Authorization</span></span>  | <span data-ttu-id="f1fe1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1fe1-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f1fe1-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f1fe1-127">Content-Type</span></span>  | <span data-ttu-id="f1fe1-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1fe1-p104">application/json. Required.</span></span>  |

## <a name="response"></a><span data-ttu-id="f1fe1-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1fe1-130">Response</span></span>

<span data-ttu-id="f1fe1-131">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto de forma de [plano](../resources/schedulinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1fe1-131">If successful, this method returns a `201 Created` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1fe1-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1fe1-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f1fe1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1fe1-133">Request</span></span>

<span data-ttu-id="f1fe1-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1fe1-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f1fe1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1fe1-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f1fe1-136">C#</span><span class="sxs-lookup"><span data-stu-id="f1fe1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1fe1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1fe1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1fe1-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1fe1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f1fe1-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1fe1-139">Response</span></span>

<span data-ttu-id="f1fe1-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f1fe1-140">The following is an example of the response.</span></span> 

><span data-ttu-id="f1fe1-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1fe1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
