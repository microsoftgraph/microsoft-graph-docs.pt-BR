---
title: Listar participantes
description: Recupere uma lista de objetos participantes na chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: dc2452190dd27cde672158c690c9be3f72331cb7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327974"
---
# <a name="list-participants"></a><span data-ttu-id="e29d1-103">Listar participantes</span><span class="sxs-lookup"><span data-stu-id="e29d1-103">List participants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e29d1-104">Recupere uma lista de objetos participantes na chamada.</span><span class="sxs-lookup"><span data-stu-id="e29d1-104">Retrieve a list of participant objects in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="e29d1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e29d1-105">Permissions</span></span>

<span data-ttu-id="e29d1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e29d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e29d1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e29d1-108">Permission type</span></span> | <span data-ttu-id="e29d1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e29d1-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="e29d1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e29d1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e29d1-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="e29d1-111">Not Supported</span></span>        |
| <span data-ttu-id="e29d1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e29d1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e29d1-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="e29d1-113">Not Supported</span></span>        |
| <span data-ttu-id="e29d1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e29d1-114">Application</span></span>     | <span data-ttu-id="e29d1-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e29d1-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="e29d1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e29d1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /app/calls/{id}/participants
GET /applications/{id}/calls/{id}/participants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e29d1-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e29d1-117">Optional query parameters</span></span>

<span data-ttu-id="e29d1-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e29d1-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e29d1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e29d1-119">Request headers</span></span>

| <span data-ttu-id="e29d1-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e29d1-120">Name</span></span>          | <span data-ttu-id="e29d1-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e29d1-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e29d1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e29d1-122">Authorization</span></span> | <span data-ttu-id="e29d1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e29d1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e29d1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e29d1-125">Request body</span></span>

<span data-ttu-id="e29d1-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e29d1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e29d1-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e29d1-127">Response</span></span>

<span data-ttu-id="e29d1-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [participantes](../resources/participant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e29d1-128">If successful, this method returns a `200 OK` response code and collection of [participant](../resources/participant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e29d1-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e29d1-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e29d1-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e29d1-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-participants"
}-->

```http
GET https://graph.microsoft.com/beta/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants
Authorization: Bearer <TOKEN>
```

<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="e29d1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e29d1-131">Response</span></span>

> <span data-ttu-id="e29d1-p103">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e29d1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.participant",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
      "info": {
        "identity" : {
          "user" : {
            "displayName": "Test User",
            "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
          }
        },
        "region": "westus",
        "languageId": "en-US"
      },
      "mediaStreams": [
        {
          "sourceId": "1",
          "mediaType": "audio",
          "label": "main-audio",
          "direction": "sendReceive",
          "serverMuted": false
        }
      ]
    },
    {
      "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
      "info": {
        "identity" : {
          "phone": {
            "displayName": "+12345678890",
            "id": "+12345678890"
          }
        }
      },
      "mediaStreams": [
        {
          "sourceId": "2",
          "mediaType": "audio",
          "label": "main-audio",
          "direction": "sendReceive",
          "serverMuted": false
        }
      ],
      "isMuted": true
    },
    {
      "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
      "info": {
        "identity" : {
          "application" : {
            "displayName": "Test BOT",
            "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
          }
        },
        "region": "westus",
        "languageId": "en-US"
      },
      "mediaStreams": [
        {
          "sourceId": "3",
          "mediaType": "audio",
          "label": "main-audio",
          "direction": "sendReceive",
          "serverMuted": false
        }
      ],
      "isMuted": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List participants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
