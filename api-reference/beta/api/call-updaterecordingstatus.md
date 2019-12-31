---
title: 'Call: updateRecordingStatus'
description: Atualize o status de gravação do aplicativo associado a uma chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7de436ecdb24a7288cf515c71598b880ec4122dc
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912731"
---
# <a name="call-updaterecordingstatus"></a><span data-ttu-id="6bf58-103">Call: updateRecordingStatus</span><span class="sxs-lookup"><span data-stu-id="6bf58-103">call: updateRecordingStatus</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bf58-104">Atualize o status de gravação do aplicativo associado a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="6bf58-104">Update the application's recording status associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="6bf58-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6bf58-105">Permissions</span></span>
<span data-ttu-id="6bf58-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bf58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6bf58-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6bf58-108">Permission type</span></span>                        | <span data-ttu-id="6bf58-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6bf58-109">Permissions (from least to most privileged)</span></span>      |
|:---------------------------------------|:-------------------------------------------------|
| <span data-ttu-id="6bf58-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6bf58-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6bf58-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="6bf58-111">Not Supported</span></span>                                    |
| <span data-ttu-id="6bf58-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6bf58-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bf58-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="6bf58-113">Not Supported</span></span>                                    |
| <span data-ttu-id="6bf58-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6bf58-114">Application</span></span>                            | <span data-ttu-id="6bf58-115">Calls. JoinGroupCalls. All, calls. AccessMedia. All</span><span class="sxs-lookup"><span data-stu-id="6bf58-115">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="6bf58-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6bf58-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateRecordingStatus
POST /communications/calls/{id}/updateRecordingStatus
```
> <span data-ttu-id="6bf58-117">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="6bf58-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="6bf58-118">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="6bf58-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6bf58-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6bf58-119">Request headers</span></span>
| <span data-ttu-id="6bf58-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6bf58-120">Name</span></span>          | <span data-ttu-id="6bf58-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bf58-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6bf58-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6bf58-122">Authorization</span></span> | <span data-ttu-id="6bf58-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bf58-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6bf58-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="6bf58-125">Content-type</span></span> | <span data-ttu-id="6bf58-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bf58-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6bf58-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6bf58-128">Request body</span></span>
<span data-ttu-id="6bf58-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6bf58-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6bf58-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6bf58-130">Parameter</span></span>       | <span data-ttu-id="6bf58-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bf58-131">Type</span></span>    | <span data-ttu-id="6bf58-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bf58-132">Description</span></span>                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| <span data-ttu-id="6bf58-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="6bf58-133">clientContext</span></span>   | <span data-ttu-id="6bf58-134">String</span><span class="sxs-lookup"><span data-stu-id="6bf58-134">String</span></span>  | <span data-ttu-id="6bf58-135">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="6bf58-135">Unique Client Context string.</span></span> <span data-ttu-id="6bf58-136">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="6bf58-136">Max limit is 256 chars.</span></span>                                 |
| <span data-ttu-id="6bf58-137">status</span><span class="sxs-lookup"><span data-stu-id="6bf58-137">status</span></span>          | <span data-ttu-id="6bf58-138">String</span><span class="sxs-lookup"><span data-stu-id="6bf58-138">String</span></span>  | <span data-ttu-id="6bf58-139">O status de gravação.</span><span class="sxs-lookup"><span data-stu-id="6bf58-139">The recording status.</span></span> <span data-ttu-id="6bf58-140">Os valores possíveis são `notRecording`: `recording`,, `failed`ou.</span><span class="sxs-lookup"><span data-stu-id="6bf58-140">Possible values are: `notRecording`, `recording`, or `failed`.</span></span>  |

## <a name="response"></a><span data-ttu-id="6bf58-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bf58-141">Response</span></span>
<span data-ttu-id="6bf58-142">Este método retorna um `200 OK` código de resposta e um cabeçalho de local com um URI para o objeto [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="6bf58-142">This method returns a `200 OK` response code and a Location header with a URI to the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="6bf58-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6bf58-143">Example</span></span>
<span data-ttu-id="6bf58-144">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="6bf58-144">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="6bf58-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bf58-145">Request</span></span>
<span data-ttu-id="6bf58-146">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="6bf58-146">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6bf58-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="6bf58-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6bf58-148">C#</span><span class="sxs-lookup"><span data-stu-id="6bf58-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updaterecordingstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6bf58-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6bf58-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updaterecordingstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6bf58-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6bf58-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updaterecordingstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6bf58-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bf58-151">Response</span></span>

> <span data-ttu-id="6bf58-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6bf58-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
