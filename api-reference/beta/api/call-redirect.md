---
title: 'Call: Redirect'
description: Redirecione as chamadas recebidas.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7eeddd2bbecb82ee0c5b90232a6e0b64de050f9d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440763"
---
# <a name="call-redirect"></a><span data-ttu-id="978f0-103">Call: Redirect</span><span class="sxs-lookup"><span data-stu-id="978f0-103">call: redirect</span></span>

<span data-ttu-id="978f0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="978f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="978f0-105">Redirecione uma chamada de entrada que ainda não foi [respondida](./call-answer.md) ou [rejeitada](./call-reject.md) .</span><span class="sxs-lookup"><span data-stu-id="978f0-105">Redirect an incoming call that hasn't been [answered](./call-answer.md) or [rejected](./call-reject.md) yet.</span></span> <span data-ttu-id="978f0-106">Os termos "redirecionando" e "encaminhando" uma chamada são usados de forma intercambiável.</span><span class="sxs-lookup"><span data-stu-id="978f0-106">The terms "redirecting" and "forwarding" a call are used interchangeably.</span></span>

<span data-ttu-id="978f0-107">O bot deve redirecionar a chamada antes que a chamada expire. O valor de tempo limite atual é de 15 segundos.</span><span class="sxs-lookup"><span data-stu-id="978f0-107">The bot is expected to redirect the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="978f0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="978f0-108">Permissions</span></span>

<span data-ttu-id="978f0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="978f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="978f0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="978f0-111">Permission type</span></span> | <span data-ttu-id="978f0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="978f0-112">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="978f0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="978f0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="978f0-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="978f0-114">Not Supported</span></span>                |
| <span data-ttu-id="978f0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="978f0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="978f0-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="978f0-116">Not Supported</span></span>                |
| <span data-ttu-id="978f0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="978f0-117">Application</span></span>     | <span data-ttu-id="978f0-118">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="978f0-118">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="978f0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="978f0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /app/calls/{id}/redirect
POST /communications/calls/{id}/redirect
```
> <span data-ttu-id="978f0-120">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="978f0-120">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="978f0-121">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="978f0-121">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="978f0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="978f0-122">Request headers</span></span>

| <span data-ttu-id="978f0-123">Nome</span><span class="sxs-lookup"><span data-stu-id="978f0-123">Name</span></span>          | <span data-ttu-id="978f0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="978f0-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="978f0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="978f0-125">Authorization</span></span> | <span data-ttu-id="978f0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="978f0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="978f0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="978f0-128">Request body</span></span>

<span data-ttu-id="978f0-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="978f0-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="978f0-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="978f0-130">Parameter</span></span>      | <span data-ttu-id="978f0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="978f0-131">Type</span></span>    |<span data-ttu-id="978f0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="978f0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="978f0-133">targets</span><span class="sxs-lookup"><span data-stu-id="978f0-133">targets</span></span>|<span data-ttu-id="978f0-134">conjunto [invitationParticipantInfo](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="978f0-134">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="978f0-135">Os participantes de destino da operação de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="978f0-135">The target participants of the redirect operation.</span></span> <span data-ttu-id="978f0-136">Se mais de um destino for especificado, será uma chamada toque simultâneo.</span><span class="sxs-lookup"><span data-stu-id="978f0-136">If more than one target is specified, it's a simulring call.</span></span> <span data-ttu-id="978f0-137">Isso significa que todos os destinos serão variados ao mesmo tempo e apenas o primeiro destino que escolher será conectado.</span><span class="sxs-lookup"><span data-stu-id="978f0-137">This means that all of the targets will be rang at the same time and only the first target that picks up will be connected.</span></span> <span data-ttu-id="978f0-138">Oferecemos suporte para até 25 metas para o toque simultâneo.</span><span class="sxs-lookup"><span data-stu-id="978f0-138">We support up to 25 targets for simulring.</span></span>
|<span data-ttu-id="978f0-139">targetDisposition</span><span class="sxs-lookup"><span data-stu-id="978f0-139">targetDisposition</span></span>|<span data-ttu-id="978f0-140">String</span><span class="sxs-lookup"><span data-stu-id="978f0-140">String</span></span>|<span data-ttu-id="978f0-141">Preterido Os valores possíveis são: `default` , `simultaneousRing` , `forward`.</span><span class="sxs-lookup"><span data-stu-id="978f0-141">(Deprecated) The possible values are: `default` , `simultaneousRing` , `forward`.</span></span> <span data-ttu-id="978f0-142">Esse parâmetro é preterido, identificaremos automaticamente se é uma chamada ou chamada de toque simultâneo do número de destinos fornecidos.</span><span class="sxs-lookup"><span data-stu-id="978f0-142">This parameter is deprecated, we will automatically identify whether it's a forward call or simulring call from the number of targets provided.</span></span>|
|<span data-ttu-id="978f0-143">timeout</span><span class="sxs-lookup"><span data-stu-id="978f0-143">timeout</span></span>|<span data-ttu-id="978f0-144">Int32</span><span class="sxs-lookup"><span data-stu-id="978f0-144">Int32</span></span>|<span data-ttu-id="978f0-145">O tempo limite (em segundos) para a operação de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="978f0-145">The timeout (in seconds) for the redirect operation.</span></span> <span data-ttu-id="978f0-146">O intervalo do valor de tempo limite é entre 15 e 90 segundos, inclusive.</span><span class="sxs-lookup"><span data-stu-id="978f0-146">The range of the timeout value is between 15 and 90 seconds inclusive.</span></span> <span data-ttu-id="978f0-147">O valor de tempo limite padrão é de 55 segundos para um destino e 60 segundos para vários destinos (sujeito a alterações).</span><span class="sxs-lookup"><span data-stu-id="978f0-147">The default timeout value is 55 seconds for one target and 60 seconds for multiple targets (subject to change).</span></span> |
|<span data-ttu-id="978f0-148">maskCallee</span><span class="sxs-lookup"><span data-stu-id="978f0-148">maskCallee</span></span>|<span data-ttu-id="978f0-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="978f0-149">Boolean</span></span>|<span data-ttu-id="978f0-150">Indica se o receptor deve ser oculto do chamador.</span><span class="sxs-lookup"><span data-stu-id="978f0-150">Indicates whether the callee is to be hidden from the caller.</span></span> <span data-ttu-id="978f0-151">Se true, a identidade do receptor é a identidade do bot.</span><span class="sxs-lookup"><span data-stu-id="978f0-151">If true, then the callee identity is the bot identity.</span></span> <span data-ttu-id="978f0-152">Padrão: false.</span><span class="sxs-lookup"><span data-stu-id="978f0-152">Default: false.</span></span>|
|<span data-ttu-id="978f0-153">maskCaller</span><span class="sxs-lookup"><span data-stu-id="978f0-153">maskCaller</span></span>|<span data-ttu-id="978f0-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="978f0-154">Boolean</span></span>|<span data-ttu-id="978f0-155">Indica se o chamador deve ser oculto do receptor.</span><span class="sxs-lookup"><span data-stu-id="978f0-155">Indicates whether the caller is to be hidden from the callee.</span></span> <span data-ttu-id="978f0-156">Se true, a identidade do chamador é a identidade do bot.</span><span class="sxs-lookup"><span data-stu-id="978f0-156">If true, then the caller identity is the bot identity.</span></span> <span data-ttu-id="978f0-157">Padrão: false.</span><span class="sxs-lookup"><span data-stu-id="978f0-157">Default: false.</span></span>|
|<span data-ttu-id="978f0-158">callbackUri</span><span class="sxs-lookup"><span data-stu-id="978f0-158">callbackUri</span></span>|<span data-ttu-id="978f0-159">String</span><span class="sxs-lookup"><span data-stu-id="978f0-159">String</span></span>|<span data-ttu-id="978f0-160">Isso permite que os bots forneçam um URI de retorno de chamada específico para que a chamada atual receba notificações posteriores.</span><span class="sxs-lookup"><span data-stu-id="978f0-160">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="978f0-161">Se essa propriedade não tiver sido definida, o URI de retorno de chamada global do bot será usado em seu lugar.</span><span class="sxs-lookup"><span data-stu-id="978f0-161">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="978f0-162">Deve ser `https`.</span><span class="sxs-lookup"><span data-stu-id="978f0-162">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="978f0-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="978f0-163">Response</span></span>
<span data-ttu-id="978f0-164">Se tiver êxito, este método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="978f0-164">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="978f0-165">Exemplos</span><span class="sxs-lookup"><span data-stu-id="978f0-165">Examples</span></span>
<span data-ttu-id="978f0-166">Estes exemplos abordarão um fluxo de trabalho de uma notificação de chamada de entrada e como essa chamada será redirecionada.</span><span class="sxs-lookup"><span data-stu-id="978f0-166">These examples will cover a workflow of an incoming call notification and how that call will be redirected.</span></span>

> <span data-ttu-id="978f0-167">**Observação:** Os objetos Response mostrados aqui podem ser reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="978f0-167">**Note:** The response objects shown here might be shortened for readability.</span></span> <span data-ttu-id="978f0-168">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="978f0-168">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-forward-a-call-to-a-target"></a><span data-ttu-id="978f0-169">Exemplo 1: encaminhar uma chamada para um destino</span><span class="sxs-lookup"><span data-stu-id="978f0-169">Example 1: Forward a Call to a Target</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="978f0-170">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="978f0-170">Notification - incoming</span></span>
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
              "id": "8d1e6ab6-26c5-4e22-a1bc-06ea7343958e",
              "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f"
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
        "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f",
        "myParticipantId": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
        "id": "491f0b00-ffff-4bc9-a43e-b226498ec22a"
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="978f0-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="978f0-171">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="978f0-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="978f0-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request", 
  "name": "call-redirect"
} -->
``` http
POST https://graph.microsoft.com/beta/communications/calls/491f0b00-ffff-4bc9-a43e-b226498ec22a/redirect
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
# <a name="c"></a>[<span data-ttu-id="978f0-173">C#</span><span class="sxs-lookup"><span data-stu-id="978f0-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="978f0-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="978f0-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="978f0-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="978f0-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="978f0-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="978f0-176">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
##### <a name="notification---terminated"></a><span data-ttu-id="978f0-177">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="978f0-177">Notification - terminated</span></span>

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
              "id": "8d1e6ab6-26c5-4e22-a1bc-06ea7343958e",
              "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f"
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
        "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f",
        "myParticipantId": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
        "id": "491f0b00-ffff-4bc9-a43e-b226498ec22a"
      }
    }
  ]
}
```

### <a name="example-2-forward-a-call-to-multiple-targets-with-simultaneous-ring"></a><span data-ttu-id="978f0-178">Exemplo 2: encaminhar uma chamada para vários destinos com toque simultâneo</span><span class="sxs-lookup"><span data-stu-id="978f0-178">Example 2: Forward a call to multiple targets with simultaneous ring</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="978f0-179">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="978f0-179">Notification - incoming</span></span>

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
              "id": "ec040873-8235-45fd-a403-c7259a5a548e",
              "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f"
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
        "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f",
        "myParticipantId": "f540f1b6-994b-4866-be95-8aad34c4f4dc",
        "id": "481f0b00-ffff-4ca1-8c67-a5f1e31e8e82"
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="978f0-180">Solicitar</span><span class="sxs-lookup"><span data-stu-id="978f0-180">Request</span></span>

<!-- {
  "blockType": "ignored", 
  "name": "call-redirect-simuring"
} -->

``` http
POST https://graph.microsoft.com/beta/communications/calls/481f0b00-ffff-4ca1-8c67-a5f1e31e8e82/redirect
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

##### <a name="response"></a><span data-ttu-id="978f0-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="978f0-181">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->

``` http
HTTP/1.1 202 Accepted
```

##### <a name="notification---terminated"></a><span data-ttu-id="978f0-182">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="978f0-182">Notification - terminated</span></span>

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
              "id": "ec040873-8235-45fd-a403-c7259a5a548e",
              "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f"
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
        "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f",
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
