---
title: 'participante: Ativar Mudo'
description: Ativar Mudo de um participante específico na chamada.
author: VinodRavichandran
ms.openlocfilehash: ea84b2944b9a9dd75a72f05f6fa5c4327068e271
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350068"
---
# <a name="participant-mute"></a><span data-ttu-id="41268-103">participante: Ativar Mudo</span><span class="sxs-lookup"><span data-stu-id="41268-103">participant: mute</span></span>

> <span data-ttu-id="41268-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="41268-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41268-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="41268-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="41268-106">Ativar Mudo de um participante específico na chamada.</span><span class="sxs-lookup"><span data-stu-id="41268-106">Mute a specific participant in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="41268-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="41268-107">Permissions</span></span>
<span data-ttu-id="41268-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41268-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41268-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41268-110">Permission type</span></span> | <span data-ttu-id="41268-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41268-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="41268-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41268-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="41268-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="41268-113">Not Supported</span></span>        |
| <span data-ttu-id="41268-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41268-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41268-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="41268-115">Not Supported</span></span>        |
| <span data-ttu-id="41268-116">Application</span><span class="sxs-lookup"><span data-stu-id="41268-116">Application</span></span>     | <span data-ttu-id="41268-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="41268-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="41268-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41268-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/{id}/mute
POST /applications/{id}/calls/{id}/participants/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="41268-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41268-119">Request headers</span></span>
| <span data-ttu-id="41268-120">Nome</span><span class="sxs-lookup"><span data-stu-id="41268-120">Name</span></span>          | <span data-ttu-id="41268-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="41268-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="41268-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="41268-122">Authorization</span></span> | <span data-ttu-id="41268-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41268-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41268-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41268-125">Request body</span></span>
<span data-ttu-id="41268-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41268-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="41268-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="41268-127">Parameter</span></span>      | <span data-ttu-id="41268-128">Type</span><span class="sxs-lookup"><span data-stu-id="41268-128">Type</span></span>    |<span data-ttu-id="41268-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="41268-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41268-130">clientContext</span><span class="sxs-lookup"><span data-stu-id="41268-130">clientContext</span></span>|<span data-ttu-id="41268-131">String</span><span class="sxs-lookup"><span data-stu-id="41268-131">String</span></span>|<span data-ttu-id="41268-132">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="41268-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="41268-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="41268-133">Response</span></span>
<span data-ttu-id="41268-134">Se tiver êxito, este método retornará `200 OK` objeto response de código e [commsOperation](../resources/commsoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41268-134">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41268-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41268-135">Example</span></span>
<span data-ttu-id="41268-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="41268-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="41268-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41268-137">Request</span></span>
<span data-ttu-id="41268-138">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="41268-138">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "participant_mute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/{id}/mute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="41268-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="41268-139">Response</span></span>

> <span data-ttu-id="41268-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41268-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.commsOperation",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

## <a name="example---mute-specific-participant"></a><span data-ttu-id="41268-142">Exemplo - mudo participante específico</span><span class="sxs-lookup"><span data-stu-id="41268-142">Example - Mute specific participant</span></span>

##### <a name="request"></a><span data-ttu-id="41268-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41268-143">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/0698446E77E24E4D85F80597083CB830/mute
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="41268-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="41268-144">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation",
  "truncated": true
}-->
```json
{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="41268-145">Notificação - lista de participação atualizado com o mudo do participante</span><span class="sxs-lookup"><span data-stu-id="41268-145">Notification - roster updated with participant muted</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "0698446E77E24E4D85F80597083CB830",
          "info": {
            "identity": {
              "user": {
                "displayName": "Test User",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "1",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": true,
          "isInLobby": false
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "123456W77E24E4D85F80597083CB830",
          "info": {
            "identity": {
              "application": {
                "displayName": "Test Bot",
                "id": "1234A46B-3D17-4ADC-8DCE-DC4E7D556789"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isInLobby": false
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participant: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
