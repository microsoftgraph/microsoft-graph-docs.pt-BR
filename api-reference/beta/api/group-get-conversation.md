---
title: Obter conversation
description: Obter um objeto conversation.
ms.openlocfilehash: 09500fa94e5945700f1d91b5d347f8a5e26db981
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037669"
---
# <a name="get-conversation"></a><span data-ttu-id="8708d-103">Obter conversation</span><span class="sxs-lookup"><span data-stu-id="8708d-103">Get conversation</span></span>

> <span data-ttu-id="8708d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8708d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8708d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8708d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8708d-106">Obter um objeto [conversation](../resources/conversation.md).</span><span class="sxs-lookup"><span data-stu-id="8708d-106">Get a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8708d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8708d-107">Permissions</span></span>
<span data-ttu-id="8708d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8708d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8708d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8708d-110">Permission type</span></span>      | <span data-ttu-id="8708d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8708d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8708d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8708d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8708d-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8708d-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8708d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8708d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8708d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8708d-115">Not supported.</span></span>    |
|<span data-ttu-id="8708d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8708d-116">Application</span></span> | <span data-ttu-id="8708d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8708d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8708d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8708d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8708d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8708d-119">Optional query parameters</span></span>
<span data-ttu-id="8708d-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8708d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8708d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8708d-121">Request headers</span></span>
| <span data-ttu-id="8708d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8708d-122">Header</span></span>       | <span data-ttu-id="8708d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8708d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8708d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8708d-124">Authorization</span></span>  | <span data-ttu-id="8708d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8708d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8708d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8708d-127">Request body</span></span>
<span data-ttu-id="8708d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8708d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8708d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8708d-129">Response</span></span>
<span data-ttu-id="8708d-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8708d-130">If successful, this method returns a `200 OK` response code and a [conversation](../resources/conversation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8708d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8708d-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8708d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8708d-132">Request</span></span>
<span data-ttu-id="8708d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8708d-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_conversation"
}-->
```http
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="8708d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8708d-134">Response</span></span>
<span data-ttu-id="8708d-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8708d-135">The following is an example of the response.</span></span>
><span data-ttu-id="8708d-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8708d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 644

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
