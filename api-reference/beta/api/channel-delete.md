---
title: Excluir um canal
description: Exclua o canal.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 2ff974205c20ea8a50778f04c741dc3f7e39a7e1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833422"
---
# <a name="delete-channel"></a><span data-ttu-id="aff7f-103">Excluir um canal</span><span class="sxs-lookup"><span data-stu-id="aff7f-103">Delete channel</span></span>

> <span data-ttu-id="aff7f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="aff7f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aff7f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="aff7f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aff7f-106">Exclua o [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="aff7f-106">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="aff7f-107">**Observação**: não há um problema conhecido com permissões de aplicativo e essa API.</span><span class="sxs-lookup"><span data-stu-id="aff7f-107">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="aff7f-108">Para obter detalhes, consulte a [lista de problemas conhecidos do](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="aff7f-108">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="aff7f-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="aff7f-109">Permissions</span></span>
<span data-ttu-id="aff7f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aff7f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aff7f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aff7f-112">Permission type</span></span>      | <span data-ttu-id="aff7f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aff7f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aff7f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aff7f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="aff7f-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aff7f-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="aff7f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aff7f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aff7f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aff7f-117">Not supported.</span></span>    |
|<span data-ttu-id="aff7f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aff7f-118">Application</span></span> | <span data-ttu-id="aff7f-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aff7f-119">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="aff7f-120">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="aff7f-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="aff7f-121">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="aff7f-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="aff7f-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aff7f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="aff7f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aff7f-123">Request headers</span></span>
| <span data-ttu-id="aff7f-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aff7f-124">Header</span></span>       | <span data-ttu-id="aff7f-125">Valor</span><span class="sxs-lookup"><span data-stu-id="aff7f-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aff7f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="aff7f-126">Authorization</span></span>  | <span data-ttu-id="aff7f-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aff7f-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aff7f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aff7f-129">Request body</span></span>
<span data-ttu-id="aff7f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aff7f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aff7f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="aff7f-131">Response</span></span>

<span data-ttu-id="aff7f-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aff7f-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aff7f-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aff7f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aff7f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aff7f-135">Request</span></span>
<span data-ttu-id="aff7f-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aff7f-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="aff7f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="aff7f-137">Response</span></span>

<span data-ttu-id="aff7f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aff7f-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
