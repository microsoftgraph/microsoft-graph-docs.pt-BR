---
title: Participantes da lista
description: Recupere uma lista de objetos de participantes na chamada.
ms.openlocfilehash: a18dc609204712f1b7c7b31150975543277ffa67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034960"
---
# <a name="list-participants"></a><span data-ttu-id="3aaf8-103">Participantes da lista</span><span class="sxs-lookup"><span data-stu-id="3aaf8-103">List participants</span></span>

> <span data-ttu-id="3aaf8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3aaf8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3aaf8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3aaf8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3aaf8-106">Recupere uma lista de objetos de participantes na chamada.</span><span class="sxs-lookup"><span data-stu-id="3aaf8-106">Retrieve a list of participant objects in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="3aaf8-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="3aaf8-107">Permissions</span></span>
<span data-ttu-id="3aaf8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3aaf8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3aaf8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3aaf8-110">Permission type</span></span> | <span data-ttu-id="3aaf8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3aaf8-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="3aaf8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3aaf8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3aaf8-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="3aaf8-113">Not Supported</span></span>        |
| <span data-ttu-id="3aaf8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3aaf8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3aaf8-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="3aaf8-115">Not Supported</span></span>        |
| <span data-ttu-id="3aaf8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3aaf8-116">Application</span></span>     | <span data-ttu-id="3aaf8-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3aaf8-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="3aaf8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3aaf8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants
GET /applications/{id}/calls/{id}/participants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3aaf8-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3aaf8-119">Optional query parameters</span></span>
<span data-ttu-id="3aaf8-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3aaf8-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3aaf8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3aaf8-121">Request headers</span></span>
| <span data-ttu-id="3aaf8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="3aaf8-122">Name</span></span>          | <span data-ttu-id="3aaf8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3aaf8-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3aaf8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3aaf8-124">Authorization</span></span> | <span data-ttu-id="3aaf8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3aaf8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3aaf8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3aaf8-127">Request body</span></span>
<span data-ttu-id="3aaf8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3aaf8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3aaf8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aaf8-129">Response</span></span>
<span data-ttu-id="3aaf8-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos de [participante](../resources/participant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3aaf8-130">If successful, this method returns a `200 OK` response code and collection of [participant](../resources/participant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3aaf8-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3aaf8-131">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="3aaf8-132">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="3aaf8-132">Example 1</span></span>

##### <a name="request"></a><span data-ttu-id="3aaf8-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3aaf8-133">Request</span></span>
<span data-ttu-id="3aaf8-134">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="3aaf8-134">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_participants"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/participants
```

##### <a name="response"></a><span data-ttu-id="3aaf8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aaf8-135">Response</span></span>

> <span data-ttu-id="3aaf8-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3aaf8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2"></a><span data-ttu-id="3aaf8-138">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="3aaf8-138">Example 2</span></span>

##### <a name="request"></a><span data-ttu-id="3aaf8-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3aaf8-139">Request</span></span>

```http
GET /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants
Authorization: Bearer <TOKEN>
```

##### <a name="response"></a><span data-ttu-id="3aaf8-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aaf8-140">Response</span></span>

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
