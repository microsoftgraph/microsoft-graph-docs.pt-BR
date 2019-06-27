---
title: Obter participante
description: Recupere as propriedades e os relacionamentos de um objeto **participante** .
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fc60b6f6a4ed1a1b1e97c9bdfddec37384faf05d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265608"
---
# <a name="get-participant"></a><span data-ttu-id="cccef-103">Obter participante</span><span class="sxs-lookup"><span data-stu-id="cccef-103">Get participant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cccef-104">Recupere as propriedades e os relacionamentos de um objeto **participante** .</span><span class="sxs-lookup"><span data-stu-id="cccef-104">Retrieve the properties and relationships of a **participant** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cccef-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cccef-105">Permissions</span></span>
<span data-ttu-id="cccef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cccef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cccef-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cccef-108">Permission type</span></span> | <span data-ttu-id="cccef-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cccef-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="cccef-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cccef-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cccef-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="cccef-111">Not Supported</span></span>        |
| <span data-ttu-id="cccef-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cccef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cccef-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="cccef-113">Not Supported</span></span>        |
| <span data-ttu-id="cccef-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cccef-114">Application</span></span>     | <span data-ttu-id="cccef-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cccef-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="cccef-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cccef-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants/{id}
GET /applications/{id}/calls/{id}/participants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cccef-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cccef-117">Optional query parameters</span></span>
<span data-ttu-id="cccef-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cccef-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cccef-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cccef-119">Request headers</span></span>
| <span data-ttu-id="cccef-120">Nome</span><span class="sxs-lookup"><span data-stu-id="cccef-120">Name</span></span>          | <span data-ttu-id="cccef-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="cccef-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="cccef-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cccef-122">Authorization</span></span> | <span data-ttu-id="cccef-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cccef-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cccef-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cccef-125">Request body</span></span>
<span data-ttu-id="cccef-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cccef-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cccef-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="cccef-127">Response</span></span>
<span data-ttu-id="cccef-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [participante](../resources/participant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cccef-128">If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cccef-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cccef-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cccef-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cccef-130">Request</span></span>
<span data-ttu-id="cccef-131">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="cccef-131">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get-participant"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/participants/{id}
```

##### <a name="response"></a><span data-ttu-id="cccef-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="cccef-132">Response</span></span>

> <span data-ttu-id="cccef-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cccef-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="cccef-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="cccef-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cccef-136">C#</span><span class="sxs-lookup"><span data-stu-id="cccef-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-participant-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cccef-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="cccef-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-participant-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="cccef-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="cccef-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-participant-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/participant-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/participant-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/participant-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
