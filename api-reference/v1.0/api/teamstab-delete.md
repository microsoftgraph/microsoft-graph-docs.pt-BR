---
title: Excluir o guia de canal
description: 'Remove (unpin) uma guia de canal especificado dentro de uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 672077e4b1ac383ca6e6bb415ff25639fb03dc08
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917430"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="a3846-103">Excluir o guia de canal</span><span class="sxs-lookup"><span data-stu-id="a3846-103">Delete tab from channel</span></span>



<span data-ttu-id="a3846-104">Remove (unpin) uma guia de [canal](../resources/channel.md) especificado dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="a3846-104">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="a3846-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a3846-105">Permissions</span></span>
<span data-ttu-id="a3846-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3846-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3846-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3846-108">Permission type</span></span>      | <span data-ttu-id="a3846-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3846-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3846-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3846-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a3846-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3846-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a3846-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3846-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3846-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3846-113">Not supported.</span></span>    |
|<span data-ttu-id="a3846-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3846-114">Application</span></span> | <span data-ttu-id="a3846-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3846-115">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="a3846-116">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="a3846-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a3846-117">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="a3846-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a3846-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3846-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a3846-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3846-119">Request headers</span></span>
| <span data-ttu-id="a3846-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a3846-120">Header</span></span>       | <span data-ttu-id="a3846-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a3846-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a3846-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3846-122">Authorization</span></span>  | <span data-ttu-id="a3846-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3846-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a3846-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3846-125">Request body</span></span>
<span data-ttu-id="a3846-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a3846-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3846-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3846-127">Response</span></span>

<span data-ttu-id="a3846-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3846-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3846-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3846-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a3846-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3846-131">Request</span></span>
<span data-ttu-id="a3846-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3846-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="a3846-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3846-133">Response</span></span>
<span data-ttu-id="a3846-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a3846-134">The following is an example of the response.</span></span> <span data-ttu-id="a3846-135">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="a3846-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a3846-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3846-136">All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete tab from channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
