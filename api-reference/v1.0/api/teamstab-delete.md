---
title: Excluir o guia de canal
description: 'Remove (unpin) uma guia de canal especificado dentro de uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9b66bf69645c9a76ea11375984cf8c56e0dff6bd
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016692"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="278ae-103">Excluir o guia de canal</span><span class="sxs-lookup"><span data-stu-id="278ae-103">Delete tab from channel</span></span>



<span data-ttu-id="278ae-104">Remove (unpin) uma guia de [canal](../resources/channel.md) especificado dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="278ae-104">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="278ae-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="278ae-105">Permissions</span></span>
<span data-ttu-id="278ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="278ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="278ae-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="278ae-108">Permission type</span></span>      | <span data-ttu-id="278ae-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="278ae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="278ae-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="278ae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="278ae-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="278ae-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="278ae-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="278ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="278ae-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="278ae-113">Not supported.</span></span>    |
|<span data-ttu-id="278ae-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="278ae-114">Application</span></span> | <span data-ttu-id="278ae-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="278ae-115">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="278ae-116">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="278ae-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="278ae-117">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="278ae-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="278ae-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="278ae-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="278ae-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="278ae-119">Request headers</span></span>
| <span data-ttu-id="278ae-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="278ae-120">Header</span></span>       | <span data-ttu-id="278ae-121">Valor</span><span class="sxs-lookup"><span data-stu-id="278ae-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="278ae-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="278ae-122">Authorization</span></span>  | <span data-ttu-id="278ae-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="278ae-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="278ae-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="278ae-125">Request body</span></span>
<span data-ttu-id="278ae-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="278ae-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="278ae-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="278ae-127">Response</span></span>

<span data-ttu-id="278ae-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="278ae-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="278ae-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="278ae-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="278ae-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="278ae-131">Request</span></span>
<span data-ttu-id="278ae-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="278ae-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="278ae-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="278ae-133">Response</span></span>
<span data-ttu-id="278ae-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="278ae-134">The following is an example of the response.</span></span> <span data-ttu-id="278ae-135">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="278ae-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="278ae-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="278ae-136">All of the properties will be returned from an actual call.</span></span>
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
