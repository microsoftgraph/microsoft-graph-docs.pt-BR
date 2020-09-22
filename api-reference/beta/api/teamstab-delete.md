---
title: Excluir Guia do canal
description: 'Remove (desafixa) uma guia do canal especificado de uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5d3a3512637f7352b532b682c494818984277ff6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999038"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="a430a-103">Excluir Guia do canal</span><span class="sxs-lookup"><span data-stu-id="a430a-103">Delete tab from channel</span></span>

<span data-ttu-id="a430a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a430a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a430a-105">Remove (desafixa) uma guia do [canal](../resources/channel.md) especificado de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="a430a-105">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="a430a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a430a-106">Permissions</span></span>
<span data-ttu-id="a430a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a430a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a430a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a430a-109">Permission type</span></span>      | <span data-ttu-id="a430a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a430a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a430a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a430a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a430a-112">TeamsTab. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a430a-112">TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="a430a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a430a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a430a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a430a-114">Not supported.</span></span>    |
|<span data-ttu-id="a430a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a430a-115">Application</span></span> | <span data-ttu-id="a430a-116">TeamsTab. Delete. Group \*, TeamsTab. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a430a-116">TeamsTab.Delete.Group\*, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="a430a-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="a430a-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="a430a-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="a430a-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a430a-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="a430a-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a430a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a430a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a430a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a430a-121">Request headers</span></span>
| <span data-ttu-id="a430a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a430a-122">Header</span></span>       | <span data-ttu-id="a430a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a430a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a430a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a430a-124">Authorization</span></span>  | <span data-ttu-id="a430a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a430a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a430a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a430a-127">Request body</span></span>
<span data-ttu-id="a430a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a430a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a430a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a430a-129">Response</span></span>

<span data-ttu-id="a430a-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a430a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a430a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a430a-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a430a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a430a-133">Request</span></span>
<span data-ttu-id="a430a-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a430a-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="a430a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a430a-135">Response</span></span>
<span data-ttu-id="a430a-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a430a-136">The following is an example of the response.</span></span> <span data-ttu-id="a430a-137">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="a430a-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a430a-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a430a-138">All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": []
}
-->


