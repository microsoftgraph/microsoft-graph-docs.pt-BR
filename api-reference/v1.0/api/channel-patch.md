---
title: Canal do patch
description: Atualize as propriedades do canal especificado.
ms.openlocfilehash: 981de62dcedb42b98016aa99ccaaa8b5cd27ba9c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007539"
---
# <a name="patch-channel"></a><span data-ttu-id="ff194-103">Canal do patch</span><span class="sxs-lookup"><span data-stu-id="ff194-103">Patch channel</span></span>



<span data-ttu-id="ff194-104">Atualize as propriedades do [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="ff194-104">Update the properties of the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="ff194-105">**Observação**: não há um problema conhecido com permissões de aplicativo e essa API.</span><span class="sxs-lookup"><span data-stu-id="ff194-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="ff194-106">Para obter detalhes, consulte a [lista de problemas conhecidos do](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="ff194-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="ff194-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="ff194-107">Permissions</span></span>
<span data-ttu-id="ff194-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff194-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff194-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff194-110">Permission type</span></span>      | <span data-ttu-id="ff194-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff194-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff194-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff194-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ff194-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff194-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ff194-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff194-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff194-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff194-115">Not supported.</span></span>    |
|<span data-ttu-id="ff194-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff194-116">Application</span></span> | <span data-ttu-id="ff194-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff194-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff194-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff194-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ff194-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff194-119">Request headers</span></span>
| <span data-ttu-id="ff194-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff194-120">Header</span></span>       | <span data-ttu-id="ff194-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ff194-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ff194-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff194-122">Authorization</span></span>  | <span data-ttu-id="ff194-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff194-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ff194-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ff194-125">Content-Type</span></span>  | <span data-ttu-id="ff194-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff194-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ff194-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff194-127">Request body</span></span>
<span data-ttu-id="ff194-128">No corpo da solicitação, fornece uma representação JSON do objeto de [canal](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="ff194-128">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ff194-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff194-129">Response</span></span>

<span data-ttu-id="ff194-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ff194-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ff194-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff194-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff194-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff194-132">Request</span></span>
<span data-ttu-id="ff194-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff194-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="ff194-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff194-134">Response</span></span>
<span data-ttu-id="ff194-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff194-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
