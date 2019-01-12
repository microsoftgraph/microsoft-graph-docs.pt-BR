---
title: Excluir o aplicativo da equipe
description: Desinstala um aplicativo da equipe do especificado.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 55e5b1a87c010a0e9a36353d8da82a8433dd3ebd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983573"
---
# <a name="delete-app-from-team"></a><span data-ttu-id="fb28a-103">Excluir o aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="fb28a-103">Delete app from team</span></span>

> <span data-ttu-id="fb28a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fb28a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb28a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fb28a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fb28a-106">Desinstala um [aplicativo](../resources/teamsappinstallation.md) da [equipe](../resources/team.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="fb28a-106">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fb28a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb28a-107">Permissions</span></span>
<span data-ttu-id="fb28a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb28a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb28a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb28a-110">Permission type</span></span>      | <span data-ttu-id="fb28a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb28a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb28a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb28a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fb28a-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb28a-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fb28a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb28a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb28a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb28a-115">Not supported.</span></span>    |
|<span data-ttu-id="fb28a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb28a-116">Application</span></span> | <span data-ttu-id="fb28a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb28a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb28a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb28a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fb28a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb28a-119">Request headers</span></span>
| <span data-ttu-id="fb28a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb28a-120">Header</span></span>       | <span data-ttu-id="fb28a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fb28a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fb28a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb28a-122">Authorization</span></span>  | <span data-ttu-id="fb28a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb28a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fb28a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb28a-125">Request body</span></span>
<span data-ttu-id="fb28a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fb28a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb28a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb28a-127">Response</span></span>

<span data-ttu-id="fb28a-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb28a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb28a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb28a-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fb28a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb28a-131">Request</span></span>
<span data-ttu-id="fb28a-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb28a-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
#### <a name="response"></a><span data-ttu-id="fb28a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb28a-133">Response</span></span>
<span data-ttu-id="fb28a-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fb28a-134">The following is an example of the response.</span></span> <span data-ttu-id="fb28a-135">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="fb28a-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fb28a-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb28a-136">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
