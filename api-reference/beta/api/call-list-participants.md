---
title: Participantes da lista
description: Recupere uma lista de objetos de participantes na chamada.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 4b0fb6ede331168cb9f10483e4628cd76046f211
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870312"
---
# <a name="list-participants"></a><span data-ttu-id="60f17-103">Participantes da lista</span><span class="sxs-lookup"><span data-stu-id="60f17-103">List participants</span></span>

> <span data-ttu-id="60f17-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="60f17-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60f17-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="60f17-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="60f17-106">Recupere uma lista de objetos de participantes na chamada.</span><span class="sxs-lookup"><span data-stu-id="60f17-106">Retrieve a list of participant objects in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="60f17-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="60f17-107">Permissions</span></span>
<span data-ttu-id="60f17-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60f17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="60f17-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60f17-110">Permission type</span></span> | <span data-ttu-id="60f17-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60f17-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="60f17-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60f17-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="60f17-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="60f17-113">Not Supported</span></span>        |
| <span data-ttu-id="60f17-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60f17-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60f17-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="60f17-115">Not Supported</span></span>        |
| <span data-ttu-id="60f17-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60f17-116">Application</span></span>     | <span data-ttu-id="60f17-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="60f17-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="60f17-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60f17-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants
GET /applications/{id}/calls/{id}/participants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="60f17-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="60f17-119">Optional query parameters</span></span>
<span data-ttu-id="60f17-120">Este método oferece suporte para os [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="60f17-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="60f17-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60f17-121">Request headers</span></span>
| <span data-ttu-id="60f17-122">Nome</span><span class="sxs-lookup"><span data-stu-id="60f17-122">Name</span></span>          | <span data-ttu-id="60f17-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="60f17-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="60f17-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="60f17-124">Authorization</span></span> | <span data-ttu-id="60f17-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60f17-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60f17-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60f17-127">Request body</span></span>
<span data-ttu-id="60f17-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="60f17-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60f17-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="60f17-129">Response</span></span>
<span data-ttu-id="60f17-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos de [participante](../resources/participant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60f17-130">If successful, this method returns a `200 OK` response code and collection of [participant](../resources/participant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="60f17-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="60f17-131">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="60f17-132">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="60f17-132">Example 1</span></span>

##### <a name="request"></a><span data-ttu-id="60f17-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60f17-133">Request</span></span>
<span data-ttu-id="60f17-134">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="60f17-134">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-participants"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/participants
```

##### <a name="response"></a><span data-ttu-id="60f17-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="60f17-135">Response</span></span>

> <span data-ttu-id="60f17-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60f17-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.participant",
  "isCollection": true,
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1152

{
  "value": [
    {
      "id": "id-value",
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
      "isInLobby": false,
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
      "metadata": "metadata-value"
    }
  ]
}
```

### <a name="example-2"></a><span data-ttu-id="60f17-138">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="60f17-138">Example 2</span></span>

##### <a name="request"></a><span data-ttu-id="60f17-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60f17-139">Request</span></span>

```http
GET /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants
Authorization: Bearer <TOKEN>
```

##### <a name="response"></a><span data-ttu-id="60f17-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="60f17-140">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participant",
  "isCollection": true,
  "truncated": true
}-->
```json
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
<!-- {
  "type": "#page.annotation",
  "description": "List participants",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
