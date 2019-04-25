---
title: Criar schedulingGroup
description: Criar um novo.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: da8d93f955fcac0530d093a33d9018930767e710
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537733"
---
# <a name="create-schedulinggroup"></a><span data-ttu-id="dc03c-103">Criar schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="dc03c-103">Create schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc03c-104">Criar um novo [](../resources/schedulinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="dc03c-104">Create a new [schedulingGroup](../resources/schedulinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dc03c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dc03c-105">Permissions</span></span>

<span data-ttu-id="dc03c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc03c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc03c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc03c-108">Permission type</span></span>      | <span data-ttu-id="dc03c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc03c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc03c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc03c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dc03c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc03c-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dc03c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc03c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc03c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc03c-113">Not supported.</span></span>    |
|<span data-ttu-id="dc03c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc03c-114">Application</span></span> | <span data-ttu-id="dc03c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc03c-115">Not supported.</span></span> |

> <span data-ttu-id="dc03c-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="dc03c-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="dc03c-117">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="dc03c-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="dc03c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc03c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="dc03c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc03c-119">Request headers</span></span>

| <span data-ttu-id="dc03c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc03c-120">Header</span></span>       | <span data-ttu-id="dc03c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dc03c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dc03c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc03c-122">Authorization</span></span>  | <span data-ttu-id="dc03c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc03c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dc03c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dc03c-125">Content-Type</span></span>  | <span data-ttu-id="dc03c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc03c-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="dc03c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc03c-127">Response</span></span>

<span data-ttu-id="dc03c-128">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto de forma de [plano](../resources/schedulinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc03c-128">If successful, this method returns a `201 Created` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc03c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc03c-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="dc03c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc03c-130">Request</span></span>

<span data-ttu-id="dc03c-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc03c-131">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="dc03c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc03c-132">Response</span></span>

<span data-ttu-id="dc03c-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dc03c-133">The following is an example of the response.</span></span> 

><span data-ttu-id="dc03c-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc03c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/schedule-post-schedulinggroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
