---
title: 'Call: updateRecordingStatus'
description: Atualize o status de gravação do aplicativo associado a uma chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 4ed2e5019bf0ea7591f7658b0d81fda438f704ff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987222"
---
# <a name="call-updaterecordingstatus"></a><span data-ttu-id="8e167-103">Call: updateRecordingStatus</span><span class="sxs-lookup"><span data-stu-id="8e167-103">call: updateRecordingStatus</span></span>

<span data-ttu-id="8e167-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e167-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e167-105">Atualize o status de gravação do aplicativo associado a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="8e167-105">Update the application's recording status associated with a call.</span></span> <span data-ttu-id="8e167-106">Isso requer o uso da solução de [gravação baseada em políticas do teams](https://docs.microsoft.com/MicrosoftTeams/teams-recording-policy) .</span><span class="sxs-lookup"><span data-stu-id="8e167-106">This requires the use of the [Teams policy-based recording](https://docs.microsoft.com/MicrosoftTeams/teams-recording-policy) solution.</span></span>

> <span data-ttu-id="8e167-107">**Restrição adicional**: você não pode usar a API de acesso à mídia para registrar ou manter o conteúdo de mídia de chamadas ou reuniões que seu aplicativo acessa, ou dados derivados desse conteúdo de mídia ("Record" ou "Recording"), sem primeiro chamar a API **updateRecordingStatus** para indicar que a gravação começou e receber uma resposta de êxito dessa API.</span><span class="sxs-lookup"><span data-stu-id="8e167-107">**Additional Restriction**: You may NOT use the Media Access API to record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content ("record" or "recording"), without first calling the **updateRecordingStatus** API to indicate that recording has begun, and receiving a success reply from that API.</span></span> <span data-ttu-id="8e167-108">Se o aplicativo começar a gravar qualquer reunião, ele deverá finalizar a gravação antes de chamar a API **updateRecordingStatus** para indicar que a gravação foi concluída.</span><span class="sxs-lookup"><span data-stu-id="8e167-108">If your application begins recording any meeting, it must end the recording prior to calling the **updateRecordingStatus** API to indicate that the recording has ended.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e167-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="8e167-109">Permissions</span></span>
<span data-ttu-id="8e167-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e167-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e167-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e167-112">Permission type</span></span>                        | <span data-ttu-id="8e167-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e167-113">Permissions (from least to most privileged)</span></span>      |
|:---------------------------------------|:-------------------------------------------------|
| <span data-ttu-id="8e167-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e167-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e167-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="8e167-115">Not Supported</span></span>                                    |
| <span data-ttu-id="8e167-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e167-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e167-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="8e167-117">Not Supported</span></span>                                    |
| <span data-ttu-id="8e167-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e167-118">Application</span></span>                            | <span data-ttu-id="8e167-119">Calls. JoinGroupCalls. All, calls. AccessMedia. All</span><span class="sxs-lookup"><span data-stu-id="8e167-119">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="8e167-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e167-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateRecordingStatus
POST /communications/calls/{id}/updateRecordingStatus
```
> <span data-ttu-id="8e167-121">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="8e167-121">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="8e167-122">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="8e167-122">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e167-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e167-123">Request headers</span></span>
| <span data-ttu-id="8e167-124">Nome</span><span class="sxs-lookup"><span data-stu-id="8e167-124">Name</span></span>          | <span data-ttu-id="8e167-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e167-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8e167-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e167-126">Authorization</span></span> | <span data-ttu-id="8e167-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e167-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8e167-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="8e167-129">Content-type</span></span> | <span data-ttu-id="8e167-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e167-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e167-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e167-132">Request body</span></span>
<span data-ttu-id="8e167-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e167-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8e167-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8e167-134">Parameter</span></span>       | <span data-ttu-id="8e167-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e167-135">Type</span></span>    | <span data-ttu-id="8e167-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e167-136">Description</span></span>                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| <span data-ttu-id="8e167-137">clientContext</span><span class="sxs-lookup"><span data-stu-id="8e167-137">clientContext</span></span>   | <span data-ttu-id="8e167-138">String</span><span class="sxs-lookup"><span data-stu-id="8e167-138">String</span></span>  | <span data-ttu-id="8e167-139">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="8e167-139">Unique Client Context string.</span></span> <span data-ttu-id="8e167-140">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="8e167-140">Max limit is 256 chars.</span></span>                                 |
| <span data-ttu-id="8e167-141">status</span><span class="sxs-lookup"><span data-stu-id="8e167-141">status</span></span>          | <span data-ttu-id="8e167-142">String</span><span class="sxs-lookup"><span data-stu-id="8e167-142">String</span></span>  | <span data-ttu-id="8e167-143">O status de gravação.</span><span class="sxs-lookup"><span data-stu-id="8e167-143">The recording status.</span></span> <span data-ttu-id="8e167-144">Os valores possíveis são: `notRecording` , `recording` , ou `failed` .</span><span class="sxs-lookup"><span data-stu-id="8e167-144">Possible values are: `notRecording`, `recording`, or `failed`.</span></span>  |

## <a name="response"></a><span data-ttu-id="8e167-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e167-145">Response</span></span>
<span data-ttu-id="8e167-146">Este método retorna um `200 OK` código de resposta e um cabeçalho de local com um URI para o objeto [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e167-146">This method returns a `200 OK` response code and a Location header with a URI to the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="8e167-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e167-147">Example</span></span>
<span data-ttu-id="8e167-148">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8e167-148">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8e167-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e167-149">Request</span></span>
<span data-ttu-id="8e167-150">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e167-150">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8e167-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e167-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-updateRecordingStatus"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/updateRecordingStatus
Content-Type: application/json
Content-Length: 79

{
  "clientContext": "clientContext-value",
  "status": "notRecording | recording | failed"
}
```
# <a name="c"></a>[<span data-ttu-id="8e167-152">C#</span><span class="sxs-lookup"><span data-stu-id="8e167-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updaterecordingstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e167-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e167-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updaterecordingstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e167-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e167-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updaterecordingstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8e167-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e167-155">Response</span></span>

> <span data-ttu-id="8e167-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e167-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "call-updateRecordingStatus",
  "truncated": true,
  "@odata.type": "microsoft.graph.updateRecordingStatusOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.updateRecordingStatusOperation",
  "clientContext": "clientContext-value",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "resultInfo": null,
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: updateRecordingStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


