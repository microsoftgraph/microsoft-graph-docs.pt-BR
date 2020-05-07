---
title: Criar schedulingGroup
description: Criar um novo.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 92218b38d07c83acbd0e32893dce96fe9cf31286
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154458"
---
# <a name="create-schedulinggroup"></a><span data-ttu-id="bdc8a-103">Criar schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="bdc8a-103">Create schedulingGroup</span></span>

<span data-ttu-id="bdc8a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdc8a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bdc8a-105">Criar [um novo.](../resources/schedulinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="bdc8a-105">Create a new [schedulingGroup](../resources/schedulinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bdc8a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bdc8a-106">Permissions</span></span>

<span data-ttu-id="bdc8a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdc8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdc8a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdc8a-109">Permission type</span></span>      | <span data-ttu-id="bdc8a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bdc8a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdc8a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdc8a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bdc8a-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bdc8a-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bdc8a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdc8a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdc8a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdc8a-114">Not supported.</span></span>    |
|<span data-ttu-id="bdc8a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdc8a-115">Application</span></span> |<span data-ttu-id="bdc8a-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdc8a-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="bdc8a-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="bdc8a-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="bdc8a-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="bdc8a-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="bdc8a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdc8a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="bdc8a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdc8a-120">Request headers</span></span>

| <span data-ttu-id="bdc8a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bdc8a-121">Header</span></span>       | <span data-ttu-id="bdc8a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bdc8a-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bdc8a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bdc8a-123">Authorization</span></span>  | <span data-ttu-id="bdc8a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdc8a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bdc8a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bdc8a-126">Content-Type</span></span>  | <span data-ttu-id="bdc8a-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdc8a-p104">application/json. Required.</span></span>  |

## <a name="response"></a><span data-ttu-id="bdc8a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdc8a-129">Response</span></span>

<span data-ttu-id="bdc8a-130">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto de forma de [plano](../resources/schedulinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdc8a-130">If successful, this method returns a `201 Created` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdc8a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bdc8a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bdc8a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdc8a-132">Request</span></span>

<span data-ttu-id="bdc8a-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdc8a-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "schedule-post-schedulinggroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups
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
---


### <a name="response"></a><span data-ttu-id="bdc8a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdc8a-134">Response</span></span>

<span data-ttu-id="bdc8a-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bdc8a-135">The following is an example of the response.</span></span> 

><span data-ttu-id="bdc8a-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bdc8a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
