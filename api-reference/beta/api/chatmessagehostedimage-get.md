---
title: Obter chatMessageHostedImage
description: Recupere uma imagem hospedada dentro de um chat.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 41ffef10ce68e4d36399839dbcb8da7dd0eac69c
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/20/2019
ms.locfileid: "35085801"
---
# <a name="get-chatmessagehostedimage"></a><span data-ttu-id="4bb67-103">Obter chatMessageHostedImage</span><span class="sxs-lookup"><span data-stu-id="4bb67-103">Get chatMessageHostedImage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bb67-104">Recupere uma [imagem hospedada](../resources/chatmessagehostedimage.md) em um [chat](../resources/chatmessage.md).</span><span class="sxs-lookup"><span data-stu-id="4bb67-104">Retrieve a [hosted image](../resources/chatmessagehostedimage.md) in a [chatMessage](../resources/chatmessage.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4bb67-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4bb67-105">Permissions</span></span>

<span data-ttu-id="4bb67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bb67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bb67-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4bb67-108">Permission Type</span></span>|<span data-ttu-id="4bb67-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4bb67-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="4bb67-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4bb67-110">Delegated (work or school account)</span></span>|<span data-ttu-id="4bb67-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bb67-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="4bb67-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4bb67-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bb67-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bb67-113">Not supported.</span></span>|
|<span data-ttu-id="4bb67-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bb67-114">Application</span></span>| <span data-ttu-id="4bb67-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bb67-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bb67-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4bb67-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/hostedImages/{id}
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}/hostedImages/{id}
GET /chats/{id}/messages/{id}/hostedImages/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedImages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4bb67-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4bb67-117">Optional query parameters</span></span>

<span data-ttu-id="4bb67-118">Esta operação não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4bb67-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4bb67-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4bb67-119">Request headers</span></span>

| <span data-ttu-id="4bb67-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4bb67-120">Header</span></span>       | <span data-ttu-id="4bb67-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4bb67-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4bb67-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4bb67-122">Authorization</span></span>  | <span data-ttu-id="4bb67-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4bb67-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4bb67-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4bb67-125">Request body</span></span>

<span data-ttu-id="4bb67-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4bb67-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4bb67-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bb67-127">Response</span></span>

<span data-ttu-id="4bb67-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto de [imagem hospedado](../resources/chatmessagehostedimage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bb67-128">If successful, this method returns a `200 OK` response code and a [hosted image](../resources/chatmessagehostedimage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bb67-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4bb67-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4bb67-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bb67-130">Request</span></span>

<span data-ttu-id="4bb67-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bb67-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}
```

##### <a name="response"></a><span data-ttu-id="4bb67-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bb67-132">Response</span></span>

<span data-ttu-id="4bb67-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bb67-133">Here is an example of the response.</span></span> 

><span data-ttu-id="4bb67-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4bb67-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "url": "url-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get chat message image",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chatmessagehostedimage-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
