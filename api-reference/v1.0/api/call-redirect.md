---
title: 'Call: Redirect'
description: Redirecione as chamadas recebidas.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d9398c42c8f4404e2d61a8d63f9d30870cb9d751
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2020
ms.locfileid: "43510830"
---
# <a name="call-redirect"></a><span data-ttu-id="374ff-103">Call: Redirect</span><span class="sxs-lookup"><span data-stu-id="374ff-103">call: redirect</span></span>

<span data-ttu-id="374ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="374ff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="374ff-105">Redirecione uma chamada de entrada que ainda não foi [respondida](./call-answer.md) ou [rejeitada](./call-reject.md) .</span><span class="sxs-lookup"><span data-stu-id="374ff-105">Redirect an incoming call that hasn't been [answered](./call-answer.md) or [rejected](./call-reject.md) yet.</span></span> <span data-ttu-id="374ff-106">Os termos "redirecionando" e "encaminhando" uma chamada são usados de forma intercambiável.</span><span class="sxs-lookup"><span data-stu-id="374ff-106">The terms "redirecting" and "forwarding" a call are used interchangeably.</span></span>

<span data-ttu-id="374ff-107">O bot deve redirecionar a chamada antes que a chamada expire. O valor de tempo limite atual é de 15 segundos.</span><span class="sxs-lookup"><span data-stu-id="374ff-107">The bot is expected to redirect the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="374ff-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="374ff-108">Permissions</span></span>

<span data-ttu-id="374ff-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="374ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="374ff-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="374ff-111">Permission type</span></span> | <span data-ttu-id="374ff-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="374ff-112">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="374ff-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="374ff-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="374ff-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="374ff-114">Not Supported</span></span>                |
| <span data-ttu-id="374ff-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="374ff-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="374ff-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="374ff-116">Not Supported</span></span>                |
| <span data-ttu-id="374ff-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="374ff-117">Application</span></span>     | <span data-ttu-id="374ff-118">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="374ff-118">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="374ff-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="374ff-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /communications/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="374ff-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="374ff-120">Request headers</span></span>

| <span data-ttu-id="374ff-121">Nome</span><span class="sxs-lookup"><span data-stu-id="374ff-121">Name</span></span>          | <span data-ttu-id="374ff-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="374ff-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="374ff-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="374ff-123">Authorization</span></span> | <span data-ttu-id="374ff-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="374ff-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="374ff-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="374ff-126">Request body</span></span>

<span data-ttu-id="374ff-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="374ff-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="374ff-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="374ff-128">Parameter</span></span>      | <span data-ttu-id="374ff-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="374ff-129">Type</span></span>    |<span data-ttu-id="374ff-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="374ff-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="374ff-131">targets</span><span class="sxs-lookup"><span data-stu-id="374ff-131">targets</span></span>|<span data-ttu-id="374ff-132">conjunto [invitationParticipantInfo](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="374ff-132">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="374ff-133">Os participantes de destino da operação de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="374ff-133">The target participants of the redirect operation.</span></span> <span data-ttu-id="374ff-134">Se mais de um destino for especificado, será uma chamada toque simultâneo.</span><span class="sxs-lookup"><span data-stu-id="374ff-134">If more than one target is specified, it's a simulring call.</span></span> <span data-ttu-id="374ff-135">Isso significa que todos os destinos serão variados ao mesmo tempo e apenas o primeiro destino que escolher será conectado.</span><span class="sxs-lookup"><span data-stu-id="374ff-135">This means that all of the targets will be rang at the same time and only the first target that picks up will be connected.</span></span> <span data-ttu-id="374ff-136">Oferecemos suporte para até 25 metas para o toque simultâneo.</span><span class="sxs-lookup"><span data-stu-id="374ff-136">We support up to 25 targets for simulring.</span></span>
|<span data-ttu-id="374ff-137">timeout</span><span class="sxs-lookup"><span data-stu-id="374ff-137">timeout</span></span>|<span data-ttu-id="374ff-138">Int32</span><span class="sxs-lookup"><span data-stu-id="374ff-138">Int32</span></span>|<span data-ttu-id="374ff-139">O tempo limite (em segundos) para a operação de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="374ff-139">The timeout (in seconds) for the redirect operation.</span></span> <span data-ttu-id="374ff-140">O intervalo do valor de tempo limite é entre 15 e 90 segundos, inclusive.</span><span class="sxs-lookup"><span data-stu-id="374ff-140">The range of the timeout value is between 15 and 90 seconds inclusive.</span></span> <span data-ttu-id="374ff-141">O valor de tempo limite padrão é de 55 segundos para um destino e 60 segundos para vários destinos (sujeito a alterações).</span><span class="sxs-lookup"><span data-stu-id="374ff-141">The default timeout value is 55 seconds for one target and 60 seconds for multiple targets (subject to change).</span></span> |
|<span data-ttu-id="374ff-142">callbackUri</span><span class="sxs-lookup"><span data-stu-id="374ff-142">callbackUri</span></span>|<span data-ttu-id="374ff-143">String</span><span class="sxs-lookup"><span data-stu-id="374ff-143">String</span></span>|<span data-ttu-id="374ff-144">Isso permite que os bots forneçam um URI de retorno de chamada específico para que a chamada atual receba notificações posteriores.</span><span class="sxs-lookup"><span data-stu-id="374ff-144">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="374ff-145">Se essa propriedade não tiver sido definida, o URI de retorno de chamada global do bot será usado em seu lugar.</span><span class="sxs-lookup"><span data-stu-id="374ff-145">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="374ff-146">Deve ser `https`.</span><span class="sxs-lookup"><span data-stu-id="374ff-146">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="374ff-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="374ff-147">Response</span></span>
<span data-ttu-id="374ff-148">Se tiver êxito, este método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="374ff-148">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="374ff-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="374ff-149">Examples</span></span>
<span data-ttu-id="374ff-150">Estes exemplos abordarão um fluxo de trabalho de uma notificação de chamada de entrada e como essa chamada será redirecionada.</span><span class="sxs-lookup"><span data-stu-id="374ff-150">These examples will cover a workflow of an incoming call notification and how that call will be redirected.</span></span>

> <span data-ttu-id="374ff-151">**Observação:** Os objetos Response mostrados aqui podem ser reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="374ff-151">**Note:** The response objects shown here might be shortened for readability.</span></span> <span data-ttu-id="374ff-152">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="374ff-152">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-forward-a-call-to-a-target"></a><span data-ttu-id="374ff-153">Exemplo 1: encaminhar uma chamada para um destino</span><span class="sxs-lookup"><span data-stu-id="374ff-153">Example 1: Forward a Call to a Target</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="374ff-154">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="374ff-154">Notification - incoming</span></span>
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

##### <a name="request"></a><span data-ttu-id="374ff-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="374ff-155">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="374ff-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="374ff-156">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="374ff-157">C#</span><span class="sxs-lookup"><span data-stu-id="374ff-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="374ff-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="374ff-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="374ff-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="374ff-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="374ff-160">Java</span><span class="sxs-lookup"><span data-stu-id="374ff-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-redirect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="374ff-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="374ff-161">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
##### <a name="notification---terminated"></a><span data-ttu-id="374ff-162">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="374ff-162">Notification - terminated</span></span>

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

### <a name="example-2-forward-a-call-to-multiple-targets-with-simultaneous-ring"></a><span data-ttu-id="374ff-163">Exemplo 2: encaminhar uma chamada para vários destinos com toque simultâneo</span><span class="sxs-lookup"><span data-stu-id="374ff-163">Example 2: Forward a call to multiple targets with simultaneous ring</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="374ff-164">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="374ff-164">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="374ff-165">Solicitar</span><span class="sxs-lookup"><span data-stu-id="374ff-165">Request</span></span>

<!-- {
  "blockType": "ignored", 
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

##### <a name="response"></a><span data-ttu-id="374ff-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="374ff-166">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->

``` http
HTTP/1.1 202 Accepted
```

##### <a name="notification---terminated"></a><span data-ttu-id="374ff-167">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="374ff-167">Notification - terminated</span></span>

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
