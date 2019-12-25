---
title: 'Call: Redirect'
description: Redirecione as chamadas recebidas.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d9f366f601fe7b9580b359c2b469f6a074771b5d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871023"
---
# <a name="call-redirect"></a><span data-ttu-id="86550-103">Call: Redirect</span><span class="sxs-lookup"><span data-stu-id="86550-103">call: redirect</span></span>

<span data-ttu-id="86550-104">Redirecione uma chamada de entrada que ainda não foi [respondida](./call-answer.md) ou [rejeitada](./call-reject.md) .</span><span class="sxs-lookup"><span data-stu-id="86550-104">Redirect an incoming call that hasn't been [answered](./call-answer.md) or [rejected](./call-reject.md) yet.</span></span> <span data-ttu-id="86550-105">Os termos "redirecionando" e "encaminhando" uma chamada são usados de forma intercambiável.</span><span class="sxs-lookup"><span data-stu-id="86550-105">The terms "redirecting" and "forwarding" a call are used interchangeably.</span></span>

<span data-ttu-id="86550-106">O bot deve redirecionar a chamada antes que a chamada expire. O valor de tempo limite atual é de 15 segundos.</span><span class="sxs-lookup"><span data-stu-id="86550-106">The bot is expected to redirect the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="86550-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="86550-107">Permissions</span></span>

<span data-ttu-id="86550-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86550-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="86550-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86550-110">Permission type</span></span> | <span data-ttu-id="86550-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86550-111">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="86550-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86550-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="86550-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="86550-113">Not Supported</span></span>                |
| <span data-ttu-id="86550-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86550-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86550-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="86550-115">Not Supported</span></span>                |
| <span data-ttu-id="86550-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86550-116">Application</span></span>     | <span data-ttu-id="86550-117">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="86550-117">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="86550-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86550-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /communications/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="86550-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86550-119">Request headers</span></span>

| <span data-ttu-id="86550-120">Nome</span><span class="sxs-lookup"><span data-stu-id="86550-120">Name</span></span>          | <span data-ttu-id="86550-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="86550-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="86550-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="86550-122">Authorization</span></span> | <span data-ttu-id="86550-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86550-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86550-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86550-125">Request body</span></span>

<span data-ttu-id="86550-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86550-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="86550-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="86550-127">Parameter</span></span>      | <span data-ttu-id="86550-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="86550-128">Type</span></span>    |<span data-ttu-id="86550-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="86550-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86550-130">targets</span><span class="sxs-lookup"><span data-stu-id="86550-130">targets</span></span>|<span data-ttu-id="86550-131">conjunto [invitationParticipantInfo](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="86550-131">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="86550-132">Os participantes de destino da operação de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="86550-132">The target participants of the redirect operation.</span></span> <span data-ttu-id="86550-133">Se mais de um destino for especificado, será uma chamada toque simultâneo.</span><span class="sxs-lookup"><span data-stu-id="86550-133">If more than one target is specified, it's a simulring call.</span></span> <span data-ttu-id="86550-134">Isso significa que todos os destinos serão variados ao mesmo tempo e apenas o primeiro destino que escolher será conectado.</span><span class="sxs-lookup"><span data-stu-id="86550-134">This means that all of the targets will be rang at the same time and only the first target that picks up will be connected.</span></span> <span data-ttu-id="86550-135">Oferecemos suporte para até 25 metas para o toque simultâneo.</span><span class="sxs-lookup"><span data-stu-id="86550-135">We support up to 25 targets for simulring.</span></span>
|<span data-ttu-id="86550-136">timeout</span><span class="sxs-lookup"><span data-stu-id="86550-136">timeout</span></span>|<span data-ttu-id="86550-137">Int32</span><span class="sxs-lookup"><span data-stu-id="86550-137">Int32</span></span>|<span data-ttu-id="86550-138">O tempo limite (em segundos) para a operação de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="86550-138">The timeout (in seconds) for the redirect operation.</span></span> <span data-ttu-id="86550-139">O intervalo do valor de tempo limite é entre 15 e 90 segundos, inclusive.</span><span class="sxs-lookup"><span data-stu-id="86550-139">The range of the timeout value is between 15 and 90 seconds inclusive.</span></span> <span data-ttu-id="86550-140">O valor de tempo limite padrão é de 55 segundos para um destino e 60 segundos para vários destinos (sujeito a alterações).</span><span class="sxs-lookup"><span data-stu-id="86550-140">The default timeout value is 55 seconds for one target and 60 seconds for multiple targets (subject to change).</span></span> |
|<span data-ttu-id="86550-141">callbackUri</span><span class="sxs-lookup"><span data-stu-id="86550-141">callbackUri</span></span>|<span data-ttu-id="86550-142">String</span><span class="sxs-lookup"><span data-stu-id="86550-142">String</span></span>|<span data-ttu-id="86550-143">Isso permite que os bots forneçam um URI de retorno de chamada específico para que a chamada atual receba notificações posteriores.</span><span class="sxs-lookup"><span data-stu-id="86550-143">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="86550-144">Se essa propriedade não tiver sido definida, o URI de retorno de chamada global do bot será usado em seu lugar.</span><span class="sxs-lookup"><span data-stu-id="86550-144">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="86550-145">Deve ser `https`.</span><span class="sxs-lookup"><span data-stu-id="86550-145">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="86550-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="86550-146">Response</span></span>
<span data-ttu-id="86550-147">Se tiver êxito, este método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="86550-147">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="86550-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="86550-148">Examples</span></span>
<span data-ttu-id="86550-149">Estes exemplos abordarão um fluxo de trabalho de uma notificação de chamada de entrada e como essa chamada será redirecionada.</span><span class="sxs-lookup"><span data-stu-id="86550-149">These examples will cover a workflow of an incoming call notification and how that call will be redirected.</span></span>

> <span data-ttu-id="86550-150">**Observação:** Os objetos Response mostrados aqui podem ser reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="86550-150">**Note:** The response objects shown here might be shortened for readability.</span></span> <span data-ttu-id="86550-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86550-151">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-forward-a-call-to-a-target"></a><span data-ttu-id="86550-152">Exemplo 1: encaminhar uma chamada para um destino</span><span class="sxs-lookup"><span data-stu-id="86550-152">Example 1: Forward a Call to a Target</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="86550-153">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="86550-153">Notification - incoming</span></span>
<!-- {
  "blockType": "example", 
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "created",
      "resourceUrl": "/communications/calls/491f0b00-ffff-4bc9-a43e-b226498ec22a",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "incoming",
        "direction": "incoming",
        "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039",
        "source": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "@odata.type": "#microsoft.graph.identitySet",
            "user": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "8d1e6ab6-26c5-4e22-a1bc-06ea7343958e"
            }
          },
          "region": "amer",
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "test bot",
                "id": "24701998-1a73-4d42-8085-bf46ed0ae039"
              }
            }
          }
        ],
        "myParticipantId": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
        "id": "491f0b00-ffff-4bc9-a43e-b226498ec22a"
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="86550-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86550-154">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="86550-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="86550-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request", 
  "name": "call-redirect"
} -->
``` http
POST https://graph.microsoft.com/v1.0/communications/calls/491f0b00-ffff-4bc9-a43e-b226498ec22a/redirect
Content-Type: application/json

{
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "application": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "test bot 2",
          "id": "22bfd41f-550e-477d-8789-f6f7bd2a5e8b"
        }
      }
    }
  ],
  "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="86550-156">C#</span><span class="sxs-lookup"><span data-stu-id="86550-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="86550-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86550-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="86550-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86550-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="86550-159">Java</span><span class="sxs-lookup"><span data-stu-id="86550-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-redirect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="86550-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="86550-160">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
##### <a name="notification---terminated"></a><span data-ttu-id="86550-161">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="86550-161">Notification - terminated</span></span>

<!-- {
  "blockType": "example", 
  "name": "call-redirect"
} -->
``` http
POST https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039
Content-Type: application/json
```

<!-- {
  "blockType": "example", 
  "@odata.type": "microsoft.graph.commsNotifications"
} -->
``` json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/491f0b00-ffff-4bc9-a43e-b226498ec22a",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "direction": "incoming",
        "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039",
        "source": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "@odata.type": "#microsoft.graph.identitySet",
            "user": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "8d1e6ab6-26c5-4e22-a1bc-06ea7343958e"
            }
          },
          "region": "amer",
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "test bot",
                "id": "24701998-1a73-4d42-8085-bf46ed0ae039"
              }
            }
          }
        ],
        "myParticipantId": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
        "id": "491f0b00-ffff-4bc9-a43e-b226498ec22a"
      }
    }
  ]
}
```

### <a name="example-2-forward-a-call-to-multiple-targets-with-simultaneous-ring"></a><span data-ttu-id="86550-162">Exemplo 2: encaminhar uma chamada para vários destinos com toque simultâneo</span><span class="sxs-lookup"><span data-stu-id="86550-162">Example 2: Forward a call to multiple targets with simultaneous ring</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="86550-163">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="86550-163">Notification - incoming</span></span>

<!-- {
  "blockType": "example", 
  "name": "call-redirect"
} -->
``` http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example", 
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "created",
      "resourceUrl": "/communications/calls/481f0b00-ffff-4ca1-8c67-a5f1e31e8e82",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "incoming",
        "direction": "incoming",
        "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039",
        "source": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "@odata.type": "#microsoft.graph.identitySet",
            "user": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "ec040873-8235-45fd-a403-c7259a5a548e"
            }
          },
          "region": "amer"
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "test bot",
                "id": "24701998-1a73-4d42-8085-bf46ed0ae039"
              }
            }
          }
        ],
        "myParticipantId": "f540f1b6-994b-4866-be95-8aad34c4f4dc",
        "id": "481f0b00-ffff-4ca1-8c67-a5f1e31e8e82"
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="86550-164">Solicitar</span><span class="sxs-lookup"><span data-stu-id="86550-164">Request</span></span>

<!-- {
  "blockType": "request", 
  "name": "call-redirect-simuring"
} -->

``` http
POST https://graph.microsoft.com/v1.0/communications/calls/481f0b00-ffff-4ca1-8c67-a5f1e31e8e82/redirect
Content-Type: application/json

{
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "test user",
          "id": "98da8a1a-1b87-452c-a713-65d3f10b1253"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "test user 2",
          "id": "bf5aae9a-d11d-47a8-93b1-782504c9c3f3"
        }
      }
    }
  ],
  "routingPolicies": [
    "disableForwarding"
  ],
  "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039"
}
```

##### <a name="response"></a><span data-ttu-id="86550-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="86550-165">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->

``` http
HTTP/1.1 202 Accepted
```

##### <a name="notification---terminated"></a><span data-ttu-id="86550-166">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="86550-166">Notification - terminated</span></span>

<!-- {
  "blockType": "example", 
  "@odata.type": "microsoft.graph.commsNotifications"
} -->

``` http
POST https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/491f0b00-ffff-4bc9-a43e-b226498ec22a",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "direction": "incoming",
        "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039",
        "source": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "@odata.type": "#microsoft.graph.identitySet",
            "user": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "ec040873-8235-45fd-a403-c7259a5a548e"
            }
          },
          "region": "amer"
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "test bot",
                "id": "24701998-1a73-4d42-8085-bf46ed0ae039"
              }
            }
          }
        ],
        "myParticipantId": "f540f1b6-994b-4866-be95-8aad34c4f4dc",
        "id": "481f0b00-ffff-4ca1-8c67-a5f1e31e8e82"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: redirect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
