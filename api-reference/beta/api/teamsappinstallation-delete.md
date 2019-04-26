---
title: Excluir aplicativo da equipe
description: Desinstala um aplicativo da equipe especificada.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8f744083bcde7fd682620fe4cb289d34c4aa07c8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330358"
---
# <a name="delete-app-from-team"></a><span data-ttu-id="3c307-103">Excluir aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="3c307-103">Delete app from team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c307-104">Desinstala um [aplicativo](../resources/teamsappinstallation.md) da [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="3c307-104">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3c307-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c307-105">Permissions</span></span>
<span data-ttu-id="3c307-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c307-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c307-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c307-108">Permission type</span></span>      | <span data-ttu-id="3c307-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c307-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c307-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c307-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3c307-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c307-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3c307-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c307-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c307-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c307-113">Not supported.</span></span>    |
|<span data-ttu-id="3c307-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c307-114">Application</span></span> | <span data-ttu-id="3c307-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c307-115">Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3c307-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c307-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3c307-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c307-117">Request headers</span></span>
| <span data-ttu-id="3c307-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c307-118">Header</span></span>       | <span data-ttu-id="3c307-119">Valor</span><span class="sxs-lookup"><span data-stu-id="3c307-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3c307-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c307-120">Authorization</span></span>  | <span data-ttu-id="3c307-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c307-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3c307-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c307-123">Request body</span></span>
<span data-ttu-id="3c307-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c307-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c307-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c307-125">Response</span></span>

<span data-ttu-id="3c307-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c307-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c307-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c307-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3c307-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c307-129">Request</span></span>
<span data-ttu-id="3c307-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c307-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
#### <a name="response"></a><span data-ttu-id="3c307-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c307-131">Response</span></span>
<span data-ttu-id="3c307-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3c307-132">The following is an example of the response.</span></span> <span data-ttu-id="3c307-133">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="3c307-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3c307-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c307-134">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
