---
title: Listar hatMessageHostedImages em uma chatmessage
description: Listar todas as imagens hospedadas em uma chatMessage.
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 351e473e0d97ec23c1a4b859d637c40a3e49b7ab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943551"
---
# <a name="list-chatmessagehostedimages-in-a-chatmessage"></a><span data-ttu-id="0fe46-103">Listar chatMessageHostedImages em uma chatMessage</span><span class="sxs-lookup"><span data-stu-id="0fe46-103">List chatMessageHostedImages in a chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fe46-104">Listar todas as [imagens hospedadas](../resources/chatmessagehostedimage.md) em uma [chatMessage](../resources/chatmessage.md).</span><span class="sxs-lookup"><span data-stu-id="0fe46-104">List all [hosted images](../resources/chatmessagehostedimage.md) in a [chatMessage](../resources/chatmessage.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0fe46-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0fe46-105">Permissions</span></span>

<span data-ttu-id="0fe46-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fe46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fe46-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fe46-108">Permission Type</span></span>|<span data-ttu-id="0fe46-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0fe46-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="0fe46-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fe46-110">Delegated (work or school account)</span></span>|<span data-ttu-id="0fe46-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fe46-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="0fe46-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fe46-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fe46-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0fe46-113">Not supported</span></span>|
|<span data-ttu-id="0fe46-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fe46-114">Application</span></span>| <span data-ttu-id="0fe46-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fe46-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fe46-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fe46-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/hostedImages
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}/hostedImages
GET /chats/{id}/messages/{id}/hostedImages
GET /users/{id}/chats/{id}/messages/{id}/hostedImages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0fe46-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0fe46-117">Optional query parameters</span></span>

<span data-ttu-id="0fe46-118">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0fe46-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0fe46-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fe46-119">Request headers</span></span>

| <span data-ttu-id="0fe46-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0fe46-120">Header</span></span>       | <span data-ttu-id="0fe46-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0fe46-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0fe46-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fe46-122">Authorization</span></span>  | <span data-ttu-id="0fe46-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0fe46-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0fe46-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fe46-125">Request body</span></span>

<span data-ttu-id="0fe46-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0fe46-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fe46-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fe46-127">Response</span></span>

<span data-ttu-id="0fe46-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [hostedImage](../resources/chatmessagehostedimage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fe46-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/chatmessagehostedimage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fe46-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0fe46-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0fe46-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fe46-130">Request</span></span>

<span data-ttu-id="0fe46-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fe46-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_messages"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/hostedImages
```

##### <a name="response"></a><span data-ttu-id="0fe46-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fe46-132">Response</span></span>

<span data-ttu-id="0fe46-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fe46-133">Here is an example of the response.</span></span> 

><span data-ttu-id="0fe46-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0fe46-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "value": [
    {
        "id": "id-value",
        "url": "url-value"
    },
    {
        "id": "id-value",
        "url": "url-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List hosted images in a chatmessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chatmessagehostedimage-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
