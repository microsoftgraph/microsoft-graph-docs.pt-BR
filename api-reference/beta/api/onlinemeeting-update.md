---
title: Atualizar onlineMeeting
description: Atualizar as propriedades de uma reunião online.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 4fc506d37bc0166057fe7997e198d02a6771267d
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/20/2020
ms.locfileid: "45184020"
---
# <a name="update-onlinemeeting"></a><span data-ttu-id="ba747-103">Atualizar onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="ba747-103">Update onlineMeeting</span></span>

<span data-ttu-id="ba747-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba747-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba747-105">Atualize as propriedades **StartDateTime**, **EndDateTime**, **participantes**e **Subject** da [onlineMeeting](../resources/onlinemeeting.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="ba747-105">Update the **startDateTime**, **endDateTime**, **participants**, and **subject** properties of the specified [onlineMeeting](../resources/onlinemeeting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ba747-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba747-106">Permissions</span></span>

| <span data-ttu-id="ba747-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba747-107">Permission type</span></span> | <span data-ttu-id="ba747-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba747-108">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="ba747-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba747-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba747-110">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba747-110">OnlineMeetings.ReadWrite</span></span>              |
| <span data-ttu-id="ba747-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba747-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba747-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba747-112">Not Supported.</span></span>                         |
| <span data-ttu-id="ba747-113">Application</span><span class="sxs-lookup"><span data-stu-id="ba747-113">Application</span></span>                            | <span data-ttu-id="ba747-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba747-114">Not Supported.</span></span>                                  |


## <a name="http-request"></a><span data-ttu-id="ba747-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba747-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/onlineMeetings/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ba747-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba747-116">Request headers</span></span>
| <span data-ttu-id="ba747-117">Nome</span><span class="sxs-lookup"><span data-stu-id="ba747-117">Name</span></span>          | <span data-ttu-id="ba747-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba747-118">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="ba747-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba747-119">Authorization</span></span> | <span data-ttu-id="ba747-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba747-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ba747-122">Content-type</span><span class="sxs-lookup"><span data-stu-id="ba747-122">Content-type</span></span>  | <span data-ttu-id="ba747-p102">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba747-p102">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba747-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba747-125">Request body</span></span>
<span data-ttu-id="ba747-126">No corpo da solicitação, forneça uma representação JSON do objeto [onlineMeeting](../resources/onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="ba747-126">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span> <span data-ttu-id="ba747-127">Somente as propriedades **StartDateTime**, **EndDateTime**, **participantes**e **Subject** podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="ba747-127">Only the **startDateTime**, **endDateTime**, **participants**, and **subject** properties can be modified.</span></span> <span data-ttu-id="ba747-128">O **StartDateTime** e **EndDateTime** devem aparecer em pares.</span><span class="sxs-lookup"><span data-stu-id="ba747-128">The **startDateTime** and **endDateTime** must appear in pairs.</span></span>

## <a name="response"></a><span data-ttu-id="ba747-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba747-129">Response</span></span>
<span data-ttu-id="ba747-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [onlineMeeting](../resources/onlinemeeting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba747-130">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba747-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ba747-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba747-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba747-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "patch_onlinemeeting_request"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/onlineMeetings/{id}
Content-Type: application/json 

{ 
    "startDateTime": "2020-09-09T14:33:30.8546353-07:00", 

    "endDateTime": "2020-09-09T15:03:30.8566356-07:00", 

    "subject": "Patch Meeting Subject" 
} 
```

### <a name="response"></a><span data-ttu-id="ba747-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba747-133">Response</span></span>

><span data-ttu-id="ba747-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ba747-134">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "id":"{id}",
   "creationDateTime":"2020-07-03T00:23:39.444642Z",
   "startDateTime":"2020-09-09T21:33:30.8546353Z",
   "endDateTime":"2020-09-09T22:03:30.8566356Z",
   "joinWebUrl":"url",
   "subject":"Patch Meeting Subject",
   "isBroadcast":false,
   "autoAdmittedUsers":"EveryoneInCompany",
   "outerMeetingAutoAdmittedUsers":null,
   "participants":{
      "organizer":{
         "upn":"upn",
         "identity":{
            "azureApplicationInstance":null,
            "applicationInstance":null,
            "application":null,
            "device":null,
            "user":{
               "id":"8716745d-77a9-4be3-afff-009e4b81658e",
               "displayName":null,
               "tenantId":"0823831b-1f1b-424b-b90a-1caa345a742a",
               "identityProvider":"AAD"
            }
         }
      }
   },
   "audioConferencing":{
      "conferenceId":"id",
      "tollNumber":"number",
      "tollFreeNumber":null,
      "dialinUrl":"url"
   }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2020-7-16 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Patch online meeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
