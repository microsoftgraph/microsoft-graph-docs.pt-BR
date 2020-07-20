---
title: 'Call: updateRecordingStatus'
description: Atualize o status de gravação do aplicativo associado a uma chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: bb8f68f53453662d8ab0707138c011548379a4e6
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/20/2020
ms.locfileid: "45183964"
---
# <a name="call-updaterecordingstatus"></a><span data-ttu-id="7989a-103">Call: updateRecordingStatus</span><span class="sxs-lookup"><span data-stu-id="7989a-103">call: updateRecordingStatus</span></span>

<span data-ttu-id="7989a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7989a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7989a-105">Atualize o status de gravação do aplicativo associado a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="7989a-105">Update the application's recording status associated with a call.</span></span> <span data-ttu-id="7989a-106">Isso requer o uso da solução de [gravação baseada em políticas do teams](https://docs.microsoft.com/MicrosoftTeams/teams-recording-policy) .</span><span class="sxs-lookup"><span data-stu-id="7989a-106">This requires the use of the [Teams policy-based recording](https://docs.microsoft.com/MicrosoftTeams/teams-recording-policy) solution.</span></span>

> <span data-ttu-id="7989a-107">**Restrição adicional**: você não pode usar a API de acesso à mídia para registrar ou manter o conteúdo de mídia de chamadas ou reuniões que seu aplicativo acessa, ou dados derivados desse conteúdo de mídia ("Record" ou "Recording"), sem primeiro chamar a API **updateRecordingStatus** para indicar que a gravação começou e receber uma resposta de êxito dessa API.</span><span class="sxs-lookup"><span data-stu-id="7989a-107">**Additional Restriction**: You may NOT use the Media Access API to record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content ("record" or "recording"), without first calling the **updateRecordingStatus** API to indicate that recording has begun, and receiving a success reply from that API.</span></span> <span data-ttu-id="7989a-108">Se o aplicativo começar a gravar qualquer reunião, ele deverá finalizar a gravação antes de chamar a API **updateRecordingStatus** para indicar que a gravação foi concluída.</span><span class="sxs-lookup"><span data-stu-id="7989a-108">If your application begins recording any meeting, it must end the recording prior to calling the **updateRecordingStatus** API to indicate that the recording has ended.</span></span>

## <a name="permissions"></a><span data-ttu-id="7989a-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="7989a-109">Permissions</span></span>
<span data-ttu-id="7989a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7989a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7989a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7989a-112">Permission type</span></span>                        | <span data-ttu-id="7989a-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7989a-113">Permissions (from least to most privileged)</span></span>      |
|:---------------------------------------|:-------------------------------------------------|
| <span data-ttu-id="7989a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7989a-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="7989a-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="7989a-115">Not Supported</span></span>                                    |
| <span data-ttu-id="7989a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7989a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7989a-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="7989a-117">Not Supported</span></span>                                    |
| <span data-ttu-id="7989a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7989a-118">Application</span></span>                            | <span data-ttu-id="7989a-119">Calls. JoinGroupCalls. All, calls. AccessMedia. All</span><span class="sxs-lookup"><span data-stu-id="7989a-119">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="7989a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7989a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/updateRecordingStatus
```

## <a name="request-headers"></a><span data-ttu-id="7989a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7989a-121">Request headers</span></span>
| <span data-ttu-id="7989a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7989a-122">Name</span></span>          | <span data-ttu-id="7989a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7989a-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7989a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7989a-124">Authorization</span></span> | <span data-ttu-id="7989a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7989a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7989a-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="7989a-127">Content-type</span></span> | <span data-ttu-id="7989a-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7989a-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7989a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7989a-130">Request body</span></span>
<span data-ttu-id="7989a-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7989a-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7989a-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7989a-132">Parameter</span></span>       | <span data-ttu-id="7989a-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="7989a-133">Type</span></span>    | <span data-ttu-id="7989a-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="7989a-134">Description</span></span>                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| <span data-ttu-id="7989a-135">clientContext</span><span class="sxs-lookup"><span data-stu-id="7989a-135">clientContext</span></span>   | <span data-ttu-id="7989a-136">String</span><span class="sxs-lookup"><span data-stu-id="7989a-136">String</span></span>  | <span data-ttu-id="7989a-137">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="7989a-137">Unique client context string.</span></span> <span data-ttu-id="7989a-138">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="7989a-138">Max limit is 256 chars.</span></span>                                 |
| <span data-ttu-id="7989a-139">status</span><span class="sxs-lookup"><span data-stu-id="7989a-139">status</span></span>          | <span data-ttu-id="7989a-140">String</span><span class="sxs-lookup"><span data-stu-id="7989a-140">String</span></span>  | <span data-ttu-id="7989a-141">O status de gravação.</span><span class="sxs-lookup"><span data-stu-id="7989a-141">The recording status.</span></span> <span data-ttu-id="7989a-142">Os valores possíveis são: `notRecording` , `recording` , ou `failed` .</span><span class="sxs-lookup"><span data-stu-id="7989a-142">Possible values are: `notRecording`, `recording`, or `failed`.</span></span>  |

## <a name="response"></a><span data-ttu-id="7989a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7989a-143">Response</span></span>
<span data-ttu-id="7989a-144">Este método retorna um `200 OK` código de resposta e um cabeçalho de local com um URI para o objeto [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="7989a-144">This method returns a `200 OK` response code and a Location header with a URI to the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="7989a-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7989a-145">Example</span></span>
<span data-ttu-id="7989a-146">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="7989a-146">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="7989a-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7989a-147">Request</span></span>
<span data-ttu-id="7989a-148">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="7989a-148">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7989a-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="7989a-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-updateRecordingStatus"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/updateRecordingStatus
Content-Type: application/json
Content-Length: 79

{
  "clientContext": "clientContext-value",
  "status": "notRecording | recording | failed"
}
```
# <a name="c"></a>[<span data-ttu-id="7989a-150">C#</span><span class="sxs-lookup"><span data-stu-id="7989a-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updaterecordingstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7989a-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7989a-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updaterecordingstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7989a-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7989a-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updaterecordingstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7989a-153">Java</span><span class="sxs-lookup"><span data-stu-id="7989a-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-updaterecordingstatus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="7989a-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="7989a-154">Response</span></span>

> <span data-ttu-id="7989a-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7989a-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "call-updateRecordingStatus",
  "truncated": true,
  "@odata.type": "microsoft.graph.updateRecordingStatusOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

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
