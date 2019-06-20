---
title: 'chatMessageHostedImage: GetBytes'
description: Obtenha a representação binária de uma imagem hospedada dentro de uma mensagem de canal ou de chat.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a661dfe7e51680804faaac7df6e32ee5e680d22b
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/20/2019
ms.locfileid: "35085800"
---
# <a name="chatmessagehostedimage-getbytes"></a><span data-ttu-id="80d58-103">chatMessageHostedImage: GetBytes</span><span class="sxs-lookup"><span data-stu-id="80d58-103">chatMessageHostedImage: getBytes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80d58-104">Obter a representação binária de uma [imagem hospedada](../resources/chatmessagehostedimage.md) em uma [mensagem](../resources/chatmessage.md).</span><span class="sxs-lookup"><span data-stu-id="80d58-104">Get the binary representation of a [hosted image](../resources/chatmessagehostedimage.md) in a [message](../resources/chatmessage.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="80d58-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="80d58-105">Permissions</span></span>

<span data-ttu-id="80d58-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80d58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80d58-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80d58-108">Permission Type</span></span>|<span data-ttu-id="80d58-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="80d58-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="80d58-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80d58-110">Delegated (work or school account)</span></span>|<span data-ttu-id="80d58-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80d58-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="80d58-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80d58-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80d58-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80d58-113">Not supported.</span></span>|
|<span data-ttu-id="80d58-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80d58-114">Application</span></span>| <span data-ttu-id="80d58-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80d58-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="80d58-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80d58-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/hostedImages/{id}/$value
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}/hostedImages/{id}/$value
GET /chats/{id}/messages/{id}/hostedImages/{id}/$value
GET /users/{id}/chats/{id}/messages/{id}/hostedImages/{id}/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="80d58-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="80d58-117">Optional query parameters</span></span>

<span data-ttu-id="80d58-118">Este método não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="80d58-118">This method does not support the [OData Query Parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="80d58-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80d58-119">Request headers</span></span>

| <span data-ttu-id="80d58-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80d58-120">Header</span></span>       | <span data-ttu-id="80d58-121">Valor</span><span class="sxs-lookup"><span data-stu-id="80d58-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="80d58-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="80d58-122">Authorization</span></span>  | <span data-ttu-id="80d58-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80d58-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="80d58-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80d58-125">Request body</span></span>

<span data-ttu-id="80d58-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="80d58-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80d58-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="80d58-127">Response</span></span>

<span data-ttu-id="80d58-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e dados binários da imagem solicitada.</span><span class="sxs-lookup"><span data-stu-id="80d58-128">If successful, this method returns a `200 OK` response code and binary data of the requested image.</span></span>

## <a name="example"></a><span data-ttu-id="80d58-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80d58-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="80d58-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80d58-130">Request</span></span>

<span data-ttu-id="80d58-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80d58-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message"
}-->

```http
GET /teams/{id}/channels/{id}/messages/{id}/hostedImages/{id}/$value
```

##### <a name="response"></a><span data-ttu-id="80d58-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="80d58-132">Response</span></span>

<span data-ttu-id="80d58-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80d58-133">Here is an example of the response.</span></span>

><span data-ttu-id="80d58-134">**Observação:** O objeto de resposta mostrado aqui é encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="80d58-134">**Note:** The response object shown here is shortened for readability.</span></span> <span data-ttu-id="80d58-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80d58-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: image/jpeg
Content-length: 201
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bytes of a hosted image",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chatmessagehostedimage-getbytes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
