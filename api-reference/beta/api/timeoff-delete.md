---
title: Excluir timeOff
description: Excluir uma instância do timeOff de um agendamento.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fe3fdbe8445b11c9d1c0f176bccdc794e3a80480
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544411"
---
# <a name="delete-timeoff"></a><span data-ttu-id="cc89d-103">Excluir timeOff</span><span class="sxs-lookup"><span data-stu-id="cc89d-103">Delete timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc89d-104">Excluir uma instância do [timeOff](../resources/timeoff.md) de um [agendamento](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="cc89d-104">Delete a [timeOff](../resources/timeoff.md) instance from a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cc89d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc89d-105">Permissions</span></span>

<span data-ttu-id="cc89d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc89d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc89d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc89d-108">Permission type</span></span>      | <span data-ttu-id="cc89d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc89d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc89d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc89d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cc89d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc89d-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cc89d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc89d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc89d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc89d-113">Not supported.</span></span>    |
|<span data-ttu-id="cc89d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc89d-114">Application</span></span> | <span data-ttu-id="cc89d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc89d-115">Not supported.</span></span> |

> <span data-ttu-id="cc89d-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="cc89d-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="cc89d-117">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="cc89d-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="cc89d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc89d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="cc89d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc89d-119">Request headers</span></span>

| <span data-ttu-id="cc89d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cc89d-120">Header</span></span>       | <span data-ttu-id="cc89d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cc89d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc89d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc89d-122">Authorization</span></span>  | <span data-ttu-id="cc89d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc89d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cc89d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc89d-125">Content-Type</span></span>  | <span data-ttu-id="cc89d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cc89d-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc89d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc89d-127">Request body</span></span>
<span data-ttu-id="cc89d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cc89d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc89d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc89d-129">Response</span></span>

<span data-ttu-id="cc89d-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc89d-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc89d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc89d-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cc89d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc89d-133">Request</span></span>

<span data-ttu-id="cc89d-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc89d-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoff-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```

#### <a name="response"></a><span data-ttu-id="cc89d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc89d-135">Response</span></span>

<span data-ttu-id="cc89d-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cc89d-136">The following is an example of the response.</span></span> 

><span data-ttu-id="cc89d-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cc89d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Deletes a timeOff from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoff-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
