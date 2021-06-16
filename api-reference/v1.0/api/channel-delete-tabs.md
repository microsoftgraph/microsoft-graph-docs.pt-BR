---
title: Excluir guia do canal
description: 'Remove (unpins) uma guia do canal especificado dentro de uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e7b2b5404328f659512ff246ed7207be23735583
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971381"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="07ed7-103">Excluir guia do canal</span><span class="sxs-lookup"><span data-stu-id="07ed7-103">Delete tab from channel</span></span>

<span data-ttu-id="07ed7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07ed7-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="07ed7-105">Remove (unpins) uma guia do canal [especificado](../resources/channel.md) dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="07ed7-105">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="07ed7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="07ed7-106">Permissions</span></span>
<span data-ttu-id="07ed7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07ed7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07ed7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07ed7-109">Permission type</span></span>      | <span data-ttu-id="07ed7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07ed7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07ed7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07ed7-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="07ed7-112">TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07ed7-112">TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="07ed7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07ed7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07ed7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07ed7-114">Not supported.</span></span>    |
|<span data-ttu-id="07ed7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07ed7-115">Application</span></span> | <span data-ttu-id="07ed7-116">TeamsTab.Delete.Group *, TeamsTab.ReadWrite.Group*, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07ed7-116">TeamsTab.Delete.Group *, TeamsTab.ReadWrite.Group*, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="07ed7-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="07ed7-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="07ed7-p102">**Observação**: esta API dá suporte a permissões de administrador. Os administradores globais e os administradores de serviços do Microsoft Teams podem acessar equipes das quais não são membros.</span><span class="sxs-lookup"><span data-stu-id="07ed7-p102">**Note**: This API supports admin permissions. Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="07ed7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07ed7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{team-id}/channels/{channel-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="07ed7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07ed7-121">Request headers</span></span>
| <span data-ttu-id="07ed7-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07ed7-122">Header</span></span>       | <span data-ttu-id="07ed7-123">Valor</span><span class="sxs-lookup"><span data-stu-id="07ed7-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="07ed7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="07ed7-124">Authorization</span></span>  | <span data-ttu-id="07ed7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07ed7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="07ed7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07ed7-127">Request body</span></span>
<span data-ttu-id="07ed7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="07ed7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07ed7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="07ed7-129">Response</span></span>

<span data-ttu-id="07ed7-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07ed7-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07ed7-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07ed7-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="07ed7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07ed7-133">Request</span></span>
<span data-ttu-id="07ed7-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="07ed7-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="07ed7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="07ed7-135">Response</span></span>
<span data-ttu-id="07ed7-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="07ed7-136">The following is an example of the response.</span></span> <span data-ttu-id="07ed7-137">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="07ed7-137">Note: The response object shown here might be shortened for readability.</span></span>
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

