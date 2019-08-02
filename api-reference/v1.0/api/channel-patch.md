---
title: Canal de patch
description: Atualiza as propriedades do canal especificado.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 39410cc591f658ca77ec05f433727a6b82b04cee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003872"
---
# <a name="patch-channel"></a><span data-ttu-id="d8fef-103">Canal de patch</span><span class="sxs-lookup"><span data-stu-id="d8fef-103">Patch channel</span></span>



<span data-ttu-id="d8fef-104">Atualiza as propriedades do [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="d8fef-104">Update the properties of the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="d8fef-105">**Observação**: Há um problema conhecido com as permissões do aplicativo e este API.</span><span class="sxs-lookup"><span data-stu-id="d8fef-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="d8fef-106">Para saber mais, confira a [lista de problemas conhecidos](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="d8fef-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="d8fef-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8fef-107">Permissions</span></span>
<span data-ttu-id="d8fef-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8fef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8fef-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8fef-110">Permission type</span></span>      | <span data-ttu-id="d8fef-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8fef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8fef-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8fef-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d8fef-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8fef-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d8fef-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8fef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8fef-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8fef-115">Not supported.</span></span>    |
|<span data-ttu-id="d8fef-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8fef-116">Application</span></span> | <span data-ttu-id="d8fef-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8fef-117">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="d8fef-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="d8fef-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d8fef-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="d8fef-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d8fef-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8fef-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d8fef-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8fef-121">Request headers</span></span>
| <span data-ttu-id="d8fef-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8fef-122">Header</span></span>       | <span data-ttu-id="d8fef-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d8fef-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d8fef-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8fef-124">Authorization</span></span>  | <span data-ttu-id="d8fef-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8fef-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d8fef-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d8fef-127">Content-Type</span></span>  | <span data-ttu-id="d8fef-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d8fef-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d8fef-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8fef-129">Request body</span></span>
<span data-ttu-id="d8fef-130">No corpo da solicitação, fornça uma representação JSON do objeto [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="d8fef-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d8fef-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8fef-131">Response</span></span>

<span data-ttu-id="d8fef-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d8fef-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d8fef-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8fef-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8fef-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8fef-134">Request</span></span>
<span data-ttu-id="d8fef-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8fef-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d8fef-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8fef-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d8fef-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d8fef-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d8fef-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8fef-138">Response</span></span>
<span data-ttu-id="d8fef-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8fef-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
