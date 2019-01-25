---
title: Obter thread de conversas
description: Obter um objeto thread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 5e5f0e21c8a73e10d069b5a6a7315d7713f170ac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525651"
---
# <a name="get-conversation-thread"></a><span data-ttu-id="c0e82-103">Obter thread de conversas</span><span class="sxs-lookup"><span data-stu-id="c0e82-103">Get conversation thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0e82-104">Obter um objeto [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="c0e82-104">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0e82-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0e82-105">Permissions</span></span>
<span data-ttu-id="c0e82-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0e82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0e82-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0e82-108">Permission type</span></span>      | <span data-ttu-id="c0e82-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0e82-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0e82-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0e82-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c0e82-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0e82-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c0e82-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0e82-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0e82-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0e82-113">Not supported.</span></span>    |
|<span data-ttu-id="c0e82-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0e82-114">Application</span></span> | <span data-ttu-id="c0e82-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0e82-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0e82-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0e82-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0e82-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c0e82-117">Optional query parameters</span></span>
<span data-ttu-id="c0e82-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c0e82-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0e82-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0e82-119">Request headers</span></span>
| <span data-ttu-id="c0e82-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0e82-120">Header</span></span>       | <span data-ttu-id="c0e82-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c0e82-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c0e82-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0e82-122">Authorization</span></span>  | <span data-ttu-id="c0e82-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0e82-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c0e82-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0e82-125">Request body</span></span>
<span data-ttu-id="c0e82-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0e82-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0e82-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0e82-127">Response</span></span>
<span data-ttu-id="c0e82-128">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [thread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0e82-128">If successful, this method returns a `200 OK` response code and a [thread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0e82-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0e82-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c0e82-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0e82-130">Request</span></span>
<span data-ttu-id="c0e82-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0e82-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_thread"
}-->
```http
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="c0e82-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0e82-132">Response</span></span>
<span data-ttu-id="c0e82-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c0e82-133">The following is an example of the response.</span></span>
><span data-ttu-id="c0e82-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0e82-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 655

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "isLocked": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-get-thread.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
