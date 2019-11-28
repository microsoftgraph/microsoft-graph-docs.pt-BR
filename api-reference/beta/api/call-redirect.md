---
title: 'Call: Redirect'
description: Redirecione as chamadas recebidas.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 51db3a87dbbfae18bb3b1651d34dc9cf1ca28725
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636691"
---
# <a name="call-redirect"></a><span data-ttu-id="d30bf-103">Call: Redirect</span><span class="sxs-lookup"><span data-stu-id="d30bf-103">call: redirect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d30bf-104">Redirecione uma chamada de entrada que ainda não foi [respondida](./call-answer.md) ou [rejeitada](./call-reject.md) .</span><span class="sxs-lookup"><span data-stu-id="d30bf-104">Redirect an incoming call that hasn't been [answered](./call-answer.md) or [rejected](./call-reject.md) yet.</span></span> <span data-ttu-id="d30bf-105">Os termos "redirecionando" e "encaminhando" uma chamada são usados de forma intercambiável.</span><span class="sxs-lookup"><span data-stu-id="d30bf-105">The terms "redirecting" and "forwarding" a call are used interchangeably.</span></span>

<span data-ttu-id="d30bf-106">O bot deve redirecionar a chamada antes que a chamada expire. O valor de tempo limite atual é de 15 segundos.</span><span class="sxs-lookup"><span data-stu-id="d30bf-106">The bot is expected to redirect the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="d30bf-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d30bf-107">Permissions</span></span>

<span data-ttu-id="d30bf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d30bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d30bf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d30bf-110">Permission type</span></span> | <span data-ttu-id="d30bf-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d30bf-111">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="d30bf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d30bf-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d30bf-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="d30bf-113">Not Supported</span></span>                |
| <span data-ttu-id="d30bf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d30bf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d30bf-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="d30bf-115">Not Supported</span></span>                |
| <span data-ttu-id="d30bf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d30bf-116">Application</span></span>     | <span data-ttu-id="d30bf-117">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="d30bf-117">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="d30bf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d30bf-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /app/calls/{id}/redirect
POST /communications/calls/{id}/redirect
```
> <span data-ttu-id="d30bf-119">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="d30bf-119">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="d30bf-120">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="d30bf-120">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d30bf-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d30bf-121">Request headers</span></span>

| <span data-ttu-id="d30bf-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d30bf-122">Name</span></span>          | <span data-ttu-id="d30bf-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d30bf-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d30bf-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d30bf-124">Authorization</span></span> | <span data-ttu-id="d30bf-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d30bf-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d30bf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d30bf-127">Request body</span></span>

<span data-ttu-id="d30bf-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d30bf-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d30bf-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d30bf-129">Parameter</span></span>      | <span data-ttu-id="d30bf-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d30bf-130">Type</span></span>    |<span data-ttu-id="d30bf-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d30bf-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d30bf-132">targets</span><span class="sxs-lookup"><span data-stu-id="d30bf-132">targets</span></span>|<span data-ttu-id="d30bf-133">coleção [invitationParticipantInfo](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="d30bf-133">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="d30bf-134">Os participantes de destino da operação de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="d30bf-134">The target participants of the redirect operation.</span></span> <span data-ttu-id="d30bf-135">Se mais de um destino for especificado, será uma chamada toque simultâneo.</span><span class="sxs-lookup"><span data-stu-id="d30bf-135">If more than one target is specified, it's a simulring call.</span></span> <span data-ttu-id="d30bf-136">Isso significa que todos os destinos serão variados ao mesmo tempo e apenas o primeiro destino que escolher será conectado.</span><span class="sxs-lookup"><span data-stu-id="d30bf-136">This means that all of the targets will be rang at the same time and only the first target that picks up will be connected.</span></span> <span data-ttu-id="d30bf-137">Oferecemos suporte para até 25 metas para o toque simultâneo.</span><span class="sxs-lookup"><span data-stu-id="d30bf-137">We support up to 25 targets for simulring.</span></span>
|<span data-ttu-id="d30bf-138">targetDisposition</span><span class="sxs-lookup"><span data-stu-id="d30bf-138">targetDisposition</span></span>|<span data-ttu-id="d30bf-139">String</span><span class="sxs-lookup"><span data-stu-id="d30bf-139">String</span></span>|<span data-ttu-id="d30bf-140">Preterido Os valores possíveis são: `default` , `simultaneousRing` , `forward`.</span><span class="sxs-lookup"><span data-stu-id="d30bf-140">(Deprecated) The possible values are: `default` , `simultaneousRing` , `forward`.</span></span> <span data-ttu-id="d30bf-141">Esse parâmetro é preterido, identificaremos automaticamente se é uma chamada ou chamada de toque simultâneo do número de destinos fornecidos.</span><span class="sxs-lookup"><span data-stu-id="d30bf-141">This parameter is deprecated, we will automatically identify whether it's a forward call or simulring call from the number of targets provided.</span></span>|
|<span data-ttu-id="d30bf-142">timeout</span><span class="sxs-lookup"><span data-stu-id="d30bf-142">timeout</span></span>|<span data-ttu-id="d30bf-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d30bf-143">Int32</span></span>|<span data-ttu-id="d30bf-144">O tempo limite (em segundos) para a operação de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="d30bf-144">The timeout (in seconds) for the redirect operation.</span></span> <span data-ttu-id="d30bf-145">O intervalo do valor de tempo limite é entre 15 e 90 segundos, inclusive.</span><span class="sxs-lookup"><span data-stu-id="d30bf-145">The range of the timeout value is between 15 and 90 seconds inclusive.</span></span> <span data-ttu-id="d30bf-146">O valor de tempo limite padrão é de 55 segundos para um destino e 60 segundos para vários destinos (sujeito a alterações).</span><span class="sxs-lookup"><span data-stu-id="d30bf-146">The default timeout value is 55 seconds for one target and 60 seconds for multiple targets (subject to change).</span></span> |
|<span data-ttu-id="d30bf-147">maskCallee</span><span class="sxs-lookup"><span data-stu-id="d30bf-147">maskCallee</span></span>|<span data-ttu-id="d30bf-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="d30bf-148">Boolean</span></span>|<span data-ttu-id="d30bf-149">Indica se o receptor deve ser oculto do chamador.</span><span class="sxs-lookup"><span data-stu-id="d30bf-149">Indicates whether the callee is to be hidden from the caller.</span></span> <span data-ttu-id="d30bf-150">Se true, a identidade do receptor é a identidade do bot.</span><span class="sxs-lookup"><span data-stu-id="d30bf-150">If true, then the callee identity is the bot identity.</span></span> <span data-ttu-id="d30bf-151">Padrão: false.</span><span class="sxs-lookup"><span data-stu-id="d30bf-151">Default: false.</span></span>|
|<span data-ttu-id="d30bf-152">maskCaller</span><span class="sxs-lookup"><span data-stu-id="d30bf-152">maskCaller</span></span>|<span data-ttu-id="d30bf-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="d30bf-153">Boolean</span></span>|<span data-ttu-id="d30bf-154">Indica se o chamador deve ser oculto do receptor.</span><span class="sxs-lookup"><span data-stu-id="d30bf-154">Indicates whether the caller is to be hidden from the callee.</span></span> <span data-ttu-id="d30bf-155">Se true, a identidade do chamador é a identidade do bot.</span><span class="sxs-lookup"><span data-stu-id="d30bf-155">If true, then the caller identity is the bot identity.</span></span> <span data-ttu-id="d30bf-156">Padrão: false.</span><span class="sxs-lookup"><span data-stu-id="d30bf-156">Default: false.</span></span>|
|<span data-ttu-id="d30bf-157">callbackUri</span><span class="sxs-lookup"><span data-stu-id="d30bf-157">callbackUri</span></span>|<span data-ttu-id="d30bf-158">String</span><span class="sxs-lookup"><span data-stu-id="d30bf-158">String</span></span>|<span data-ttu-id="d30bf-159">Isso permite que os bots forneçam um URI de retorno de chamada específico para que a chamada atual receba notificações posteriores.</span><span class="sxs-lookup"><span data-stu-id="d30bf-159">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="d30bf-160">Se essa propriedade não tiver sido definida, o URI de retorno de chamada global do bot será usado em seu lugar.</span><span class="sxs-lookup"><span data-stu-id="d30bf-160">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="d30bf-161">Deve ser `https`.</span><span class="sxs-lookup"><span data-stu-id="d30bf-161">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="d30bf-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="d30bf-162">Response</span></span>
<span data-ttu-id="d30bf-163">Se tiver êxito, este método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="d30bf-163">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d30bf-164">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d30bf-164">Examples</span></span>
<span data-ttu-id="d30bf-165">Estes exemplos abordarão um fluxo de trabalho de uma notificação de chamada de entrada e como essa chamada será redirecionada.</span><span class="sxs-lookup"><span data-stu-id="d30bf-165">These examples will cover a workflow of an incoming call notification and how that call will be redirected.</span></span>

> <span data-ttu-id="d30bf-166">**Observação:** Os objetos Response mostrados aqui podem ser reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="d30bf-166">**Note:** The response objects shown here might be shortened for readability.</span></span> <span data-ttu-id="d30bf-167">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d30bf-167">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-forward-a-call-to-a-target"></a><span data-ttu-id="d30bf-168">Exemplo 1: encaminhar uma chamada para um destino</span><span class="sxs-lookup"><span data-stu-id="d30bf-168">Example 1: Forward a Call to a Target</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="d30bf-169">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="d30bf-169">Notification - incoming</span></span>
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

##### <a name="request"></a><span data-ttu-id="d30bf-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d30bf-170">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d30bf-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="d30bf-171">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d30bf-172">C#</span><span class="sxs-lookup"><span data-stu-id="d30bf-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d30bf-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d30bf-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d30bf-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d30bf-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d30bf-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="d30bf-175">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
##### <a name="notification---terminated"></a><span data-ttu-id="d30bf-176">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="d30bf-176">Notification - terminated</span></span>

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

### <a name="example-2-forward-a-call-to-multiple-targets-with-simultaneous-ring"></a><span data-ttu-id="d30bf-177">Exemplo 2: encaminhar uma chamada para vários destinos com toque simultâneo</span><span class="sxs-lookup"><span data-stu-id="d30bf-177">Example 2: Forward a call to multiple targets with simultaneous ring</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="d30bf-178">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="d30bf-178">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="d30bf-179">Solicitar</span><span class="sxs-lookup"><span data-stu-id="d30bf-179">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="d30bf-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="d30bf-180">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->

``` http
HTTP/1.1 202 Accepted
```

##### <a name="notification---terminated"></a><span data-ttu-id="d30bf-181">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="d30bf-181">Notification - terminated</span></span>

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
