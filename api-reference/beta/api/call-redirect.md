---
title: 'Call: Redirect'
description: Redirecione as chamadas recebidas.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 8a3919c2a84b8b248f81599359dcba92d58f830f
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719675"
---
# <a name="call-redirect"></a><span data-ttu-id="e8538-103">Call: Redirect</span><span class="sxs-lookup"><span data-stu-id="e8538-103">call: redirect</span></span>

<span data-ttu-id="e8538-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8538-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8538-105">Redirecione uma chamada de entrada que ainda não foi [respondida](./call-answer.md) ou [rejeitada](./call-reject.md) .</span><span class="sxs-lookup"><span data-stu-id="e8538-105">Redirect an incoming call that hasn't been [answered](./call-answer.md) or [rejected](./call-reject.md) yet.</span></span> <span data-ttu-id="e8538-106">Os termos "redirecionando" e "encaminhando" uma chamada são usados de forma intercambiável.</span><span class="sxs-lookup"><span data-stu-id="e8538-106">The terms "redirecting" and "forwarding" a call are used interchangeably.</span></span>

<span data-ttu-id="e8538-107">O bot deve redirecionar a chamada antes que a chamada expire. O valor de tempo limite atual é de 15 segundos.</span><span class="sxs-lookup"><span data-stu-id="e8538-107">The bot is expected to redirect the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8538-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8538-108">Permissions</span></span>

<span data-ttu-id="e8538-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8538-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8538-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8538-111">Permission type</span></span> | <span data-ttu-id="e8538-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8538-112">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="e8538-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8538-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8538-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="e8538-114">Not Supported</span></span>                |
| <span data-ttu-id="e8538-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8538-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8538-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="e8538-116">Not Supported</span></span>                |
| <span data-ttu-id="e8538-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8538-117">Application</span></span>     | <span data-ttu-id="e8538-118">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="e8538-118">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="e8538-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8538-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /app/calls/{id}/redirect
POST /communications/calls/{id}/redirect
```
> <span data-ttu-id="e8538-120">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="e8538-120">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="e8538-121">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="e8538-121">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8538-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8538-122">Request headers</span></span>

| <span data-ttu-id="e8538-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e8538-123">Name</span></span>          | <span data-ttu-id="e8538-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8538-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e8538-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8538-125">Authorization</span></span> | <span data-ttu-id="e8538-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8538-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8538-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8538-128">Request body</span></span>

<span data-ttu-id="e8538-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8538-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e8538-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e8538-130">Parameter</span></span>      | <span data-ttu-id="e8538-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8538-131">Type</span></span>    |<span data-ttu-id="e8538-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8538-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8538-133">targets</span><span class="sxs-lookup"><span data-stu-id="e8538-133">targets</span></span>|<span data-ttu-id="e8538-134">conjunto [invitationParticipantInfo](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="e8538-134">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="e8538-135">Os participantes de destino da operação de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="e8538-135">The target participants of the redirect operation.</span></span> <span data-ttu-id="e8538-136">Se mais de um destino for especificado, será uma chamada toque simultâneo.</span><span class="sxs-lookup"><span data-stu-id="e8538-136">If more than one target is specified, it's a simulring call.</span></span> <span data-ttu-id="e8538-137">Isso significa que todos os destinos serão variados ao mesmo tempo e apenas o primeiro destino que escolher será conectado.</span><span class="sxs-lookup"><span data-stu-id="e8538-137">This means that all of the targets will be rang at the same time and only the first target that picks up will be connected.</span></span> <span data-ttu-id="e8538-138">Oferecemos suporte para até 25 metas para o toque simultâneo.</span><span class="sxs-lookup"><span data-stu-id="e8538-138">We support up to 25 targets for simulring.</span></span>
|<span data-ttu-id="e8538-139">targetDisposition</span><span class="sxs-lookup"><span data-stu-id="e8538-139">targetDisposition</span></span>|<span data-ttu-id="e8538-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8538-140">String</span></span>|<span data-ttu-id="e8538-141">Preterido Os valores possíveis são: `default` , `simultaneousRing` , `forward` .</span><span class="sxs-lookup"><span data-stu-id="e8538-141">(Deprecated) The possible values are: `default` , `simultaneousRing` , `forward`.</span></span> <span data-ttu-id="e8538-142">Esse parâmetro é preterido, identificaremos automaticamente se é uma chamada ou chamada de toque simultâneo do número de destinos fornecidos.</span><span class="sxs-lookup"><span data-stu-id="e8538-142">This parameter is deprecated, we will automatically identify whether it's a forward call or simulring call from the number of targets provided.</span></span>|
|<span data-ttu-id="e8538-143">timeout</span><span class="sxs-lookup"><span data-stu-id="e8538-143">timeout</span></span>|<span data-ttu-id="e8538-144">Int32</span><span class="sxs-lookup"><span data-stu-id="e8538-144">Int32</span></span>|<span data-ttu-id="e8538-145">O tempo limite (em segundos) para a operação de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="e8538-145">The timeout (in seconds) for the redirect operation.</span></span> <span data-ttu-id="e8538-146">O intervalo do valor de tempo limite é entre 15 e 90 segundos, inclusive.</span><span class="sxs-lookup"><span data-stu-id="e8538-146">The range of the timeout value is between 15 and 90 seconds inclusive.</span></span> <span data-ttu-id="e8538-147">O valor de tempo limite padrão é de 55 segundos para um destino e 60 segundos para vários destinos (sujeito a alterações).</span><span class="sxs-lookup"><span data-stu-id="e8538-147">The default timeout value is 55 seconds for one target and 60 seconds for multiple targets (subject to change).</span></span> |
|<span data-ttu-id="e8538-148">maskCallee</span><span class="sxs-lookup"><span data-stu-id="e8538-148">maskCallee</span></span>|<span data-ttu-id="e8538-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="e8538-149">Boolean</span></span>|<span data-ttu-id="e8538-150">Indica se o receptor deve ser oculto do chamador.</span><span class="sxs-lookup"><span data-stu-id="e8538-150">Indicates whether the callee is to be hidden from the caller.</span></span> <span data-ttu-id="e8538-151">Se true, a identidade do receptor é a identidade do bot.</span><span class="sxs-lookup"><span data-stu-id="e8538-151">If true, then the callee identity is the bot identity.</span></span> <span data-ttu-id="e8538-152">Padrão: false.</span><span class="sxs-lookup"><span data-stu-id="e8538-152">Default: false.</span></span>|
|<span data-ttu-id="e8538-153">maskCaller</span><span class="sxs-lookup"><span data-stu-id="e8538-153">maskCaller</span></span>|<span data-ttu-id="e8538-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="e8538-154">Boolean</span></span>|<span data-ttu-id="e8538-155">Indica se o chamador deve ser oculto do receptor.</span><span class="sxs-lookup"><span data-stu-id="e8538-155">Indicates whether the caller is to be hidden from the callee.</span></span> <span data-ttu-id="e8538-156">Se true, a identidade do chamador é a identidade do bot.</span><span class="sxs-lookup"><span data-stu-id="e8538-156">If true, then the caller identity is the bot identity.</span></span> <span data-ttu-id="e8538-157">Padrão: false.</span><span class="sxs-lookup"><span data-stu-id="e8538-157">Default: false.</span></span>|
|<span data-ttu-id="e8538-158">callbackUri</span><span class="sxs-lookup"><span data-stu-id="e8538-158">callbackUri</span></span>|<span data-ttu-id="e8538-159">String</span><span class="sxs-lookup"><span data-stu-id="e8538-159">String</span></span>|<span data-ttu-id="e8538-160">Isso permite que os bots forneçam um URI de retorno de chamada específico para que a chamada atual receba notificações posteriores.</span><span class="sxs-lookup"><span data-stu-id="e8538-160">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="e8538-161">Se essa propriedade não tiver sido definida, o URI de retorno de chamada global do bot será usado em seu lugar.</span><span class="sxs-lookup"><span data-stu-id="e8538-161">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="e8538-162">Deve ser `https` .</span><span class="sxs-lookup"><span data-stu-id="e8538-162">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="e8538-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8538-163">Response</span></span>
<span data-ttu-id="e8538-164">Se tiver êxito, este método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="e8538-164">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e8538-165">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e8538-165">Examples</span></span>
<span data-ttu-id="e8538-166">Estes exemplos abordarão um fluxo de trabalho de uma notificação de chamada de entrada e como essa chamada será redirecionada.</span><span class="sxs-lookup"><span data-stu-id="e8538-166">These examples will cover a workflow of an incoming call notification and how that call will be redirected.</span></span>

> <span data-ttu-id="e8538-167">**Observação:** Os objetos Response mostrados aqui podem ser reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="e8538-167">**Note:** The response objects shown here might be shortened for readability.</span></span> <span data-ttu-id="e8538-168">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8538-168">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-forward-a-call-to-a-target"></a><span data-ttu-id="e8538-169">Exemplo 1: encaminhar uma chamada para um destino</span><span class="sxs-lookup"><span data-stu-id="e8538-169">Example 1: Forward a call to a target</span></span>

#### <a name="notification---incoming"></a><span data-ttu-id="e8538-170">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="e8538-170">Notification - incoming</span></span>
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

#### <a name="request"></a><span data-ttu-id="e8538-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8538-171">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e8538-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8538-172">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e8538-173">C#</span><span class="sxs-lookup"><span data-stu-id="e8538-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8538-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8538-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8538-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8538-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8538-176">Java</span><span class="sxs-lookup"><span data-stu-id="e8538-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-redirect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e8538-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8538-177">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="notification---terminated"></a><span data-ttu-id="e8538-178">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="e8538-178">Notification - terminated</span></span>

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

### <a name="example-2-forward-a-call-to-multiple-targets-with-simultaneous-ring"></a><span data-ttu-id="e8538-179">Exemplo 2: encaminhar uma chamada para vários destinos com toque simultâneo</span><span class="sxs-lookup"><span data-stu-id="e8538-179">Example 2: Forward a call to multiple targets with simultaneous ring</span></span>

#### <a name="notification---incoming"></a><span data-ttu-id="e8538-180">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="e8538-180">Notification - incoming</span></span>

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

#### <a name="request"></a><span data-ttu-id="e8538-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8538-181">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="e8538-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8538-182">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->

``` http
HTTP/1.1 202 Accepted
```

#### <a name="notification---terminated"></a><span data-ttu-id="e8538-183">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="e8538-183">Notification - terminated</span></span>

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

### <a name="example-3-forward-a-call-to-a-pstn-number"></a><span data-ttu-id="e8538-184">Exemplo 3: encaminhar uma chamada para um número PSTN</span><span class="sxs-lookup"><span data-stu-id="e8538-184">Example 3: Forward a call to a PSTN number</span></span>

<span data-ttu-id="e8538-185">Essa chamada requer uma instância de aplicativo com um número PSTN atribuído.</span><span class="sxs-lookup"><span data-stu-id="e8538-185">This call requires an application instance with a PSTN number assigned.</span></span>

#### <a name="step-1-create-application-instance"></a><span data-ttu-id="e8538-186">Etapa 1: criar instância de aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8538-186">Step 1: Create application instance</span></span>
<span data-ttu-id="e8538-187">Usando credenciais de administrador de locatário, chame os seguintes cmdlets no PowerShell remoto do locatário para criar a instância do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e8538-187">Using tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to create the application instance.</span></span> <span data-ttu-id="e8538-188">Para obter mais informações, consulte [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) e [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="e8538-188">For more information, see [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <UPN> -DisplayName <DisplayName> -ApplicationId <AppId>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
#### <a name="step-2-assign-microsoft-365-licenses"></a><span data-ttu-id="e8538-189">Etapa 2: atribuir licenças do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e8538-189">Step 2: Assign Microsoft 365 licenses</span></span>
1. <span data-ttu-id="e8538-190">Use as credenciais de administrador de locatário para entrar https://admin.microsoft.com/ e acessar a guia **usuários-> ativos** .</span><span class="sxs-lookup"><span data-stu-id="e8538-190">Use tenant admin credentials to sign in to https://admin.microsoft.com/ and go to the **Users -> Active users** tab.</span></span>
2. <span data-ttu-id="e8538-191">Selecione a instância do aplicativo, atribua o **plano de chamadas domésticas e internacionais da microsoft 365** e **o Microsoft 365 Phone System-licenças de usuário virtual** e clique em **salvar alterações**.</span><span class="sxs-lookup"><span data-stu-id="e8538-191">Select the application instance, assign **Microsoft 365 Domestic and International Calling Plan** and **Microsoft 365 Phone System - Virtual User** licenses, and click **Save changes**.</span></span> <span data-ttu-id="e8538-192">Se as licenças necessárias não estiverem disponíveis no locatário, você poderá obtê-las na guia **serviços de compra de > de cobrança** .</span><span class="sxs-lookup"><span data-stu-id="e8538-192">If the required licenses are not available in the tenant, you can get them from the **Billing -> Purchase services** tab.</span></span>
#### <a name="step-3-acquire-pstn-number"></a><span data-ttu-id="e8538-193">Etapa 3: adquirir o número PSTN</span><span class="sxs-lookup"><span data-stu-id="e8538-193">Step 3: Acquire PSTN number</span></span>
1. <span data-ttu-id="e8538-194">Use as credenciais de administrador de locatário para entrar no https://admin.teams.microsoft.com/ e clique na guia **portal herdado** no painel esquerdo.</span><span class="sxs-lookup"><span data-stu-id="e8538-194">Use tenant admin credentials to sign in to https://admin.teams.microsoft.com/ and click the **Legacy portal** tab on the left panel.</span></span>
2. <span data-ttu-id="e8538-195">Na nova página, vá para a guia **números de telefone de > de voz** .</span><span class="sxs-lookup"><span data-stu-id="e8538-195">In the new page, go to the **voice -> phone numbers** tab.</span></span>
3. <span data-ttu-id="e8538-196">Clique no **+** botão, selecione **novos números de serviço** e vá para a página **Adicionar novos números de serviço** .</span><span class="sxs-lookup"><span data-stu-id="e8538-196">Click the **+** button, select **New Service Numbers**, and go to the **Add new service numbers** page.</span></span>
4. <span data-ttu-id="e8538-197">Selecione **país/região**, **estado/região**, **cidade**, **quantidade** de entrada e clique em **Adicionar** para pesquisar.</span><span class="sxs-lookup"><span data-stu-id="e8538-197">Select **Country/Region**, **State/Region**, **City**, input **Quantity**, and click **add** to search.</span></span> <span data-ttu-id="e8538-198">Clique em **adquirir números**.</span><span class="sxs-lookup"><span data-stu-id="e8538-198">Click **acquire numbers**.</span></span> <span data-ttu-id="e8538-199">O número adquirido recentemente será exibido na guia **números de telefone** .</span><span class="sxs-lookup"><span data-stu-id="e8538-199">The newly acquired number will show on  the **phone numbers** tab.</span></span>
#### <a name="step-4-assign-pstn-number-to-application-instance"></a><span data-ttu-id="e8538-200">Etapa 4: atribuir o número PSTN à instância do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8538-200">Step 4: Assign PSTN number to application instance</span></span>
<span data-ttu-id="e8538-201">Com as credenciais de administrador de locatário, chame os seguintes cmdlets no PowerShell remoto do locatário para atribuir o número PSTN à instância do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e8538-201">With tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to assign the PSTN number to the application instance.</span></span> <span data-ttu-id="e8538-202">Para obter mais informações, consulte [set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) e [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="e8538-202">For more information, see [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <UPN> -TelephoneNumber <TelephoneNumber>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
> <span data-ttu-id="e8538-203">**Observação:** Se um locatário tem números PSTN australianos atribuídos a qualquer instância de aplicativo, essa chamada pode falhar.</span><span class="sxs-lookup"><span data-stu-id="e8538-203">**Note:** If a tenant has Australian PSTN numbers assigned to any application instances, this call might fail.</span></span> <span data-ttu-id="e8538-204">Se um locatário é recém-criado, pode levar alguns dias para que esse recurso esteja disponível.</span><span class="sxs-lookup"><span data-stu-id="e8538-204">If a tenant is newly created, it might take several days for this feature to be available.</span></span>

#### <a name="notification---incoming"></a><span data-ttu-id="e8538-205">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="e8538-205">Notification - incoming</span></span>
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
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "applicationInstance": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "PstnAppInstance",
                "id": "7629bdce-046c-4903-86b4-a8f718277e1a",
                "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f"
              }
            },
            "endpointType": "default",
            "id": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
            "region": "amer",
            "languageId": null
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

#### <a name="request"></a><span data-ttu-id="e8538-206">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8538-206">Request</span></span>

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
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
      }
    }
  ],
  "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039"
}
```
#### <a name="response"></a><span data-ttu-id="e8538-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8538-207">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="notification---terminated"></a><span data-ttu-id="e8538-208">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="e8538-208">Notification - terminated</span></span>

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
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "applicationInstance": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "PstnAppInstance",
                "id": "7629bdce-046c-4903-86b4-a8f718277e1a",
                "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f"
              }
            },
            "endpointType": "default",
            "id": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
            "region": "amer",
            "languageId": null
          }
        ],
        "answeredBy": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "@odata.type": "#microsoft.graph.identitySet",
            "encrypted": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "1xt4uextl99sdzwdxuvdxrvgrv8gehcq7jdgf9yhzeto"
            }
          },
          "endpointType": "default"
        },
        "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f",
        "myParticipantId": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
        "id": "491f0b00-ffff-4bc9-a43e-b226498ec22a"
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


