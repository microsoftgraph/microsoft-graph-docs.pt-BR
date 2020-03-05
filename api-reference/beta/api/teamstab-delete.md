---
title: Excluir Guia do canal
description: 'Remove (desafixa) uma guia do canal especificado de uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 04162d76710746ea41382c808acea940bc947866
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452418"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="1f23d-103">Excluir Guia do canal</span><span class="sxs-lookup"><span data-stu-id="1f23d-103">Delete tab from channel</span></span>

<span data-ttu-id="1f23d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1f23d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f23d-105">Remove (desafixa) uma guia do [canal](../resources/channel.md) especificado de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="1f23d-105">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="1f23d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1f23d-106">Permissions</span></span>
<span data-ttu-id="1f23d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f23d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f23d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f23d-109">Permission type</span></span>      | <span data-ttu-id="1f23d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f23d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f23d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f23d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1f23d-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f23d-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1f23d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f23d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f23d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f23d-114">Not supported.</span></span>    |
|<span data-ttu-id="1f23d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f23d-115">Application</span></span> | <span data-ttu-id="1f23d-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f23d-116">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="1f23d-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="1f23d-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1f23d-118">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="1f23d-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1f23d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f23d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1f23d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f23d-120">Request headers</span></span>
| <span data-ttu-id="1f23d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1f23d-121">Header</span></span>       | <span data-ttu-id="1f23d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1f23d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1f23d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f23d-123">Authorization</span></span>  | <span data-ttu-id="1f23d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f23d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1f23d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f23d-126">Request body</span></span>
<span data-ttu-id="1f23d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1f23d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f23d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f23d-128">Response</span></span>

<span data-ttu-id="1f23d-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f23d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f23d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f23d-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1f23d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f23d-132">Request</span></span>
<span data-ttu-id="1f23d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f23d-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="1f23d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f23d-134">Response</span></span>
<span data-ttu-id="1f23d-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1f23d-135">The following is an example of the response.</span></span> <span data-ttu-id="1f23d-136">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="1f23d-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1f23d-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f23d-137">All of the properties will be returned from an actual call.</span></span>
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
