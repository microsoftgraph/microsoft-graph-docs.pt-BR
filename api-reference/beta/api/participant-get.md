---
title: Obter participante
description: Recupere as propriedades e os relacionamentos de um objeto **participante** .
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2d2f5262665faac903c2208e78604cde9efff580
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349583"
---
# <a name="get-participant"></a><span data-ttu-id="8f097-103">Obter participante</span><span class="sxs-lookup"><span data-stu-id="8f097-103">Get participant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f097-104">Recupere as propriedades e os relacionamentos de um objeto **participante** .</span><span class="sxs-lookup"><span data-stu-id="8f097-104">Retrieve the properties and relationships of a **participant** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f097-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8f097-105">Permissions</span></span>
<span data-ttu-id="8f097-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f097-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f097-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f097-108">Permission type</span></span> | <span data-ttu-id="8f097-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f097-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="8f097-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f097-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f097-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="8f097-111">Not Supported</span></span>        |
| <span data-ttu-id="8f097-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f097-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f097-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="8f097-113">Not Supported</span></span>        |
| <span data-ttu-id="8f097-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f097-114">Application</span></span>     | <span data-ttu-id="8f097-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8f097-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="8f097-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f097-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants/{id}
GET /applications/{id}/calls/{id}/participants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8f097-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8f097-117">Optional query parameters</span></span>
<span data-ttu-id="8f097-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8f097-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f097-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f097-119">Request headers</span></span>
| <span data-ttu-id="8f097-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8f097-120">Name</span></span>          | <span data-ttu-id="8f097-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f097-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8f097-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f097-122">Authorization</span></span> | <span data-ttu-id="8f097-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f097-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f097-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f097-125">Request body</span></span>
<span data-ttu-id="8f097-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8f097-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f097-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f097-127">Response</span></span>
<span data-ttu-id="8f097-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [participante](../resources/participant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f097-128">If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f097-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f097-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8f097-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f097-130">Request</span></span>
<span data-ttu-id="8f097-131">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f097-131">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8f097-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f097-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-participant"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/participants/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f097-133">C#</span><span class="sxs-lookup"><span data-stu-id="8f097-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-participant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f097-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f097-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-participant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f097-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8f097-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-participant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8f097-136">Java</span><span class="sxs-lookup"><span data-stu-id="8f097-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-participant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8f097-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f097-137">Response</span></span>

> <span data-ttu-id="8f097-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f097-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.participant"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 977

{
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "info": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "isInLobby": true,
  "isMuted": true,
  "mediaStreams": [
    {
      "sourceId": "1",
      "direction": "sendReceive",
      "label": "main-audio",
      "mediaType": "audio",
      "serverMuted": false
    }
  ],
  "metadata": "metadata-value",
  "recordingInfo": {
    "initiatedBy": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "languageId-value",
      "region": "region-value"
    },
    "status": "recordingCapable"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get participant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
