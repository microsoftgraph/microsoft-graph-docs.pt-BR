---
title: Excluir guia do canal
description: 'Remove (unpins) uma guia do canal especificado dentro de uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 06f91b864ecb4a5fdf02dfab115f2f818a0ea34d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039906"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="a4b48-103">Excluir guia do canal</span><span class="sxs-lookup"><span data-stu-id="a4b48-103">Delete tab from channel</span></span>

<span data-ttu-id="a4b48-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4b48-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="a4b48-105">Remove (unpins) uma guia do canal [especificado](../resources/channel.md) dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="a4b48-105">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="a4b48-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a4b48-106">Permissions</span></span>
<span data-ttu-id="a4b48-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4b48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4b48-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4b48-109">Permission type</span></span>      | <span data-ttu-id="a4b48-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4b48-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4b48-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4b48-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="a4b48-112">TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4b48-112">TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="a4b48-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4b48-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4b48-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4b48-114">Not supported.</span></span>    |
|<span data-ttu-id="a4b48-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4b48-115">Application</span></span> | <span data-ttu-id="a4b48-116">TeamsTab.Delete.Group\*, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4b48-116">TeamsTab.Delete.Group\*, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="a4b48-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="a4b48-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="a4b48-p102">**Observação**: esta API dá suporte a permissões de administrador. Os administradores globais e os administradores de serviços do Microsoft Teams podem acessar equipes das quais não são membros.</span><span class="sxs-lookup"><span data-stu-id="a4b48-p102">**Note**: This API supports admin permissions. Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a4b48-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4b48-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{team-id}/channels/{channel-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="a4b48-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4b48-121">Request headers</span></span>
| <span data-ttu-id="a4b48-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a4b48-122">Header</span></span>       | <span data-ttu-id="a4b48-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a4b48-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a4b48-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4b48-124">Authorization</span></span>  | <span data-ttu-id="a4b48-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4b48-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a4b48-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4b48-127">Request body</span></span>
<span data-ttu-id="a4b48-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a4b48-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4b48-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4b48-129">Response</span></span>

<span data-ttu-id="a4b48-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4b48-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4b48-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4b48-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a4b48-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4b48-133">Request</span></span>
<span data-ttu-id="a4b48-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4b48-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="a4b48-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4b48-135">Response</span></span>
<span data-ttu-id="a4b48-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a4b48-136">The following is an example of the response.</span></span> <span data-ttu-id="a4b48-137">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a4b48-137">Note: The response object shown here might be shortened for readability.</span></span>
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete tab from channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->

