---
title: Excluir o guia de canal
description: 'Remove (unpin) uma guia de canal especificado dentro de uma equipe. '
author: nkramer
ms.openlocfilehash: 7d8465f650d63f22625c1da2c56b3de4e065374b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349284"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="b8046-103">Excluir o guia de canal</span><span class="sxs-lookup"><span data-stu-id="b8046-103">Delete tab from channel</span></span>

> <span data-ttu-id="b8046-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b8046-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8046-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b8046-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b8046-106">Remove (unpin) uma guia de [canal](../resources/channel.md) especificado dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="b8046-106">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="b8046-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8046-107">Permissions</span></span>
<span data-ttu-id="b8046-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8046-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8046-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8046-110">Permission type</span></span>      | <span data-ttu-id="b8046-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8046-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8046-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8046-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b8046-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8046-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b8046-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8046-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8046-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8046-115">Not supported.</span></span>    |
|<span data-ttu-id="b8046-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8046-116">Application</span></span> | <span data-ttu-id="b8046-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8046-117">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="b8046-118">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="b8046-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b8046-119">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="b8046-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b8046-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8046-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b8046-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8046-121">Request headers</span></span>
| <span data-ttu-id="b8046-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8046-122">Header</span></span>       | <span data-ttu-id="b8046-123">Valor</span><span class="sxs-lookup"><span data-stu-id="b8046-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b8046-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8046-124">Authorization</span></span>  | <span data-ttu-id="b8046-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8046-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b8046-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8046-127">Request body</span></span>
<span data-ttu-id="b8046-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8046-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8046-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8046-129">Response</span></span>

<span data-ttu-id="b8046-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8046-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8046-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8046-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b8046-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8046-133">Request</span></span>
<span data-ttu-id="b8046-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8046-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="b8046-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8046-135">Response</span></span>
<span data-ttu-id="b8046-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b8046-136">The following is an example of the response.</span></span> <span data-ttu-id="b8046-137">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="b8046-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b8046-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8046-138">All of the properties will be returned from an actual call.</span></span>
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
