---
title: 'Call: updateRecordingStatus'
description: Atualize o status de gravação do aplicativo associado a uma chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7a86276b42244b6fc1443d07d5170175f7166a92
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440679"
---
# <a name="call-updaterecordingstatus"></a><span data-ttu-id="f4100-103">Call: updateRecordingStatus</span><span class="sxs-lookup"><span data-stu-id="f4100-103">call: updateRecordingStatus</span></span>

<span data-ttu-id="f4100-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f4100-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4100-105">Atualize o status de gravação do aplicativo associado a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="f4100-105">Update the application's recording status associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4100-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f4100-106">Permissions</span></span>
<span data-ttu-id="f4100-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4100-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f4100-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4100-109">Permission type</span></span>                        | <span data-ttu-id="f4100-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f4100-110">Permissions (from least to most privileged)</span></span>      |
|:---------------------------------------|:-------------------------------------------------|
| <span data-ttu-id="f4100-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4100-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f4100-112">Não suportado</span><span class="sxs-lookup"><span data-stu-id="f4100-112">Not Supported</span></span>                                    |
| <span data-ttu-id="f4100-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4100-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4100-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="f4100-114">Not Supported</span></span>                                    |
| <span data-ttu-id="f4100-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4100-115">Application</span></span>                            | <span data-ttu-id="f4100-116">Calls. JoinGroupCalls. All, calls. AccessMedia. All</span><span class="sxs-lookup"><span data-stu-id="f4100-116">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="f4100-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4100-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateRecordingStatus
POST /communications/calls/{id}/updateRecordingStatus
```
> <span data-ttu-id="f4100-118">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="f4100-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="f4100-119">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="f4100-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4100-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4100-120">Request headers</span></span>
| <span data-ttu-id="f4100-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f4100-121">Name</span></span>          | <span data-ttu-id="f4100-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4100-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f4100-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4100-123">Authorization</span></span> | <span data-ttu-id="f4100-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4100-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f4100-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="f4100-126">Content-type</span></span> | <span data-ttu-id="f4100-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4100-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4100-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4100-129">Request body</span></span>
<span data-ttu-id="f4100-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4100-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f4100-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f4100-131">Parameter</span></span>       | <span data-ttu-id="f4100-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4100-132">Type</span></span>    | <span data-ttu-id="f4100-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4100-133">Description</span></span>                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| <span data-ttu-id="f4100-134">clientContext</span><span class="sxs-lookup"><span data-stu-id="f4100-134">clientContext</span></span>   | <span data-ttu-id="f4100-135">String</span><span class="sxs-lookup"><span data-stu-id="f4100-135">String</span></span>  | <span data-ttu-id="f4100-136">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="f4100-136">Unique Client Context string.</span></span> <span data-ttu-id="f4100-137">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="f4100-137">Max limit is 256 chars.</span></span>                                 |
| <span data-ttu-id="f4100-138">status</span><span class="sxs-lookup"><span data-stu-id="f4100-138">status</span></span>          | <span data-ttu-id="f4100-139">String</span><span class="sxs-lookup"><span data-stu-id="f4100-139">String</span></span>  | <span data-ttu-id="f4100-140">O status de gravação.</span><span class="sxs-lookup"><span data-stu-id="f4100-140">The recording status.</span></span> <span data-ttu-id="f4100-141">Os valores possíveis são `notRecording`: `recording`,, `failed`ou.</span><span class="sxs-lookup"><span data-stu-id="f4100-141">Possible values are: `notRecording`, `recording`, or `failed`.</span></span>  |

## <a name="response"></a><span data-ttu-id="f4100-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4100-142">Response</span></span>
<span data-ttu-id="f4100-143">Este método retorna um `200 OK` código de resposta e um cabeçalho de local com um URI para o objeto [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4100-143">This method returns a `200 OK` response code and a Location header with a URI to the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="f4100-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4100-144">Example</span></span>
<span data-ttu-id="f4100-145">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f4100-145">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="f4100-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4100-146">Request</span></span>
<span data-ttu-id="f4100-147">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4100-147">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f4100-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4100-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f4100-149">C#</span><span class="sxs-lookup"><span data-stu-id="f4100-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updaterecordingstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4100-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4100-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updaterecordingstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4100-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4100-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updaterecordingstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f4100-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4100-152">Response</span></span>

> <span data-ttu-id="f4100-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4100-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
