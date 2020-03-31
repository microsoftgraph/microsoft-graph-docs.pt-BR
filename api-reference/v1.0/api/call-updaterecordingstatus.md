---
title: 'Call: updateRecordingStatus'
description: Atualize o status de gravação do aplicativo associado a uma chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 9601c3a4589ba899d76b4ce55c1b0fdf8b3da355
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062578"
---
# <a name="call-updaterecordingstatus"></a><span data-ttu-id="8669e-103">Call: updateRecordingStatus</span><span class="sxs-lookup"><span data-stu-id="8669e-103">call: updateRecordingStatus</span></span>

<span data-ttu-id="8669e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8669e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8669e-105">Atualize o status de gravação do aplicativo associado a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="8669e-105">Update the application's recording status associated with a call.</span></span>

> <span data-ttu-id="8669e-106">**Restrição adicional**: você não pode usar a API de acesso à mídia para registrar ou manter o conteúdo de mídia de chamadas ou reuniões que seu aplicativo acessa, ou dados derivados desse conteúdo de mídia ("Record" ou "Recording"), sem primeiro chamar a API **updateRecordingStatus** para indicar que a gravação começou e receber uma resposta de êxito dessa API.</span><span class="sxs-lookup"><span data-stu-id="8669e-106">**Additional Restriction**: You may NOT use the Media Access API to record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content ("record" or "recording"), without first calling the **updateRecordingStatus** API to indicate that recording has begun, and receiving a success reply from that API.</span></span> <span data-ttu-id="8669e-107">Se o aplicativo começar a gravar qualquer reunião, ele deverá finalizar a gravação antes de chamar a API **updateRecordingStatus** para indicar que a gravação foi concluída.</span><span class="sxs-lookup"><span data-stu-id="8669e-107">If your application begins recording any meeting, it must end the recording prior to calling the **updateRecordingStatus** API to indicate that the recording has ended.</span></span>

## <a name="permissions"></a><span data-ttu-id="8669e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="8669e-108">Permissions</span></span>
<span data-ttu-id="8669e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8669e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8669e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8669e-111">Permission type</span></span>                        | <span data-ttu-id="8669e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8669e-112">Permissions (from least to most privileged)</span></span>      |
|:---------------------------------------|:-------------------------------------------------|
| <span data-ttu-id="8669e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8669e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8669e-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="8669e-114">Not Supported</span></span>                                    |
| <span data-ttu-id="8669e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8669e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8669e-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="8669e-116">Not Supported</span></span>                                    |
| <span data-ttu-id="8669e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8669e-117">Application</span></span>                            | <span data-ttu-id="8669e-118">Calls. JoinGroupCalls. All, calls. AccessMedia. All</span><span class="sxs-lookup"><span data-stu-id="8669e-118">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="8669e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8669e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/updateRecordingStatus
```

## <a name="request-headers"></a><span data-ttu-id="8669e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8669e-120">Request headers</span></span>
| <span data-ttu-id="8669e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8669e-121">Name</span></span>          | <span data-ttu-id="8669e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8669e-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8669e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8669e-123">Authorization</span></span> | <span data-ttu-id="8669e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8669e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8669e-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="8669e-126">Content-type</span></span> | <span data-ttu-id="8669e-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8669e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8669e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8669e-129">Request body</span></span>
<span data-ttu-id="8669e-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8669e-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8669e-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8669e-131">Parameter</span></span>       | <span data-ttu-id="8669e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="8669e-132">Type</span></span>    | <span data-ttu-id="8669e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="8669e-133">Description</span></span>                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| <span data-ttu-id="8669e-134">clientContext</span><span class="sxs-lookup"><span data-stu-id="8669e-134">clientContext</span></span>   | <span data-ttu-id="8669e-135">String</span><span class="sxs-lookup"><span data-stu-id="8669e-135">String</span></span>  | <span data-ttu-id="8669e-136">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="8669e-136">Unique client context string.</span></span> <span data-ttu-id="8669e-137">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="8669e-137">Max limit is 256 chars.</span></span>                                 |
| <span data-ttu-id="8669e-138">status</span><span class="sxs-lookup"><span data-stu-id="8669e-138">status</span></span>          | <span data-ttu-id="8669e-139">String</span><span class="sxs-lookup"><span data-stu-id="8669e-139">String</span></span>  | <span data-ttu-id="8669e-140">O status de gravação.</span><span class="sxs-lookup"><span data-stu-id="8669e-140">The recording status.</span></span> <span data-ttu-id="8669e-141">Os valores possíveis são `notRecording`: `recording`,, `failed`ou.</span><span class="sxs-lookup"><span data-stu-id="8669e-141">Possible values are: `notRecording`, `recording`, or `failed`.</span></span>  |

## <a name="response"></a><span data-ttu-id="8669e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8669e-142">Response</span></span>
<span data-ttu-id="8669e-143">Este método retorna um `200 OK` código de resposta e um cabeçalho de local com um URI para o objeto [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="8669e-143">This method returns a `200 OK` response code and a Location header with a URI to the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="8669e-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8669e-144">Example</span></span>
<span data-ttu-id="8669e-145">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8669e-145">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8669e-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8669e-146">Request</span></span>
<span data-ttu-id="8669e-147">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="8669e-147">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8669e-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="8669e-148">HTTP</span></span>](#tab/http)
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
---

### <a name="response"></a><span data-ttu-id="8669e-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="8669e-149">Response</span></span>

> <span data-ttu-id="8669e-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8669e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
