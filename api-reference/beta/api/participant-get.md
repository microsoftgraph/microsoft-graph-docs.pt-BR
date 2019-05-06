---
title: Obter participante
description: Recupere as propriedades e os relacionamentos de um objeto **participante** .
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 01728c5aa1736a8fca8397ac5ea859c6c7640a1c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33595861"
---
# <a name="get-participant"></a><span data-ttu-id="b5304-103">Obter participante</span><span class="sxs-lookup"><span data-stu-id="b5304-103">Get participant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5304-104">Recupere as propriedades e os relacionamentos de um objeto **participante** .</span><span class="sxs-lookup"><span data-stu-id="b5304-104">Retrieve the properties and relationships of a **participant** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5304-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5304-105">Permissions</span></span>
<span data-ttu-id="b5304-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5304-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5304-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5304-108">Permission type</span></span> | <span data-ttu-id="b5304-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5304-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="b5304-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5304-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5304-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="b5304-111">Not Supported</span></span>        |
| <span data-ttu-id="b5304-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5304-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5304-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="b5304-113">Not Supported</span></span>        |
| <span data-ttu-id="b5304-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5304-114">Application</span></span>     | <span data-ttu-id="b5304-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b5304-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="b5304-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5304-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants/{id}
GET /applications/{id}/calls/{id}/participants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b5304-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b5304-117">Optional query parameters</span></span>
<span data-ttu-id="b5304-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b5304-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5304-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5304-119">Request headers</span></span>
| <span data-ttu-id="b5304-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b5304-120">Name</span></span>          | <span data-ttu-id="b5304-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5304-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b5304-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5304-122">Authorization</span></span> | <span data-ttu-id="b5304-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5304-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5304-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5304-125">Request body</span></span>
<span data-ttu-id="b5304-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b5304-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5304-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5304-127">Response</span></span>
<span data-ttu-id="b5304-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [participante](../resources/participant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5304-128">If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5304-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5304-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b5304-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5304-130">Request</span></span>
<span data-ttu-id="b5304-131">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5304-131">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get-participant"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/participants/{id}
```

##### <a name="response"></a><span data-ttu-id="b5304-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5304-132">Response</span></span>

> <span data-ttu-id="b5304-p103">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5304-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b5304-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="b5304-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b5304-136">Basic</span><span class="sxs-lookup"><span data-stu-id="b5304-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-participant-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5304-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5304-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-participant-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/participant-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/participant-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
