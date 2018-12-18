---
title: 'participante: muteAll'
description: Ativar Mudo de todos os participantes na chamada.
author: VinodRavichandran
ms.openlocfilehash: 26369f3dc0c6502950c46ed1f9befe80ea1a320a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310175"
---
# <a name="participant-muteall"></a><span data-ttu-id="5d22d-103">participante: muteAll</span><span class="sxs-lookup"><span data-stu-id="5d22d-103">participant: muteAll</span></span>

> <span data-ttu-id="5d22d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5d22d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d22d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5d22d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5d22d-106">Ativar Mudo de todos os participantes na chamada.</span><span class="sxs-lookup"><span data-stu-id="5d22d-106">Mute all participants in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d22d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d22d-107">Permissions</span></span>
<span data-ttu-id="5d22d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d22d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5d22d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d22d-110">Permission type</span></span>                        | <span data-ttu-id="5d22d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d22d-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5d22d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d22d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5d22d-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="5d22d-113">Not Supported</span></span>                               |
| <span data-ttu-id="5d22d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d22d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d22d-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="5d22d-115">Not Supported</span></span>                               |
| <span data-ttu-id="5d22d-116">Application</span><span class="sxs-lookup"><span data-stu-id="5d22d-116">Application</span></span>                            | <span data-ttu-id="5d22d-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5d22d-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="5d22d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d22d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /applications/{id}/calls/{id}/participants/muteAll
```

## <a name="request-headers"></a><span data-ttu-id="5d22d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d22d-119">Request headers</span></span>
| <span data-ttu-id="5d22d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5d22d-120">Name</span></span>          | <span data-ttu-id="5d22d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d22d-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5d22d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d22d-122">Authorization</span></span> | <span data-ttu-id="5d22d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d22d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d22d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d22d-125">Request body</span></span>
<span data-ttu-id="5d22d-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d22d-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5d22d-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5d22d-127">Parameter</span></span>      | <span data-ttu-id="5d22d-128">Type</span><span class="sxs-lookup"><span data-stu-id="5d22d-128">Type</span></span>    |<span data-ttu-id="5d22d-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d22d-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d22d-130">participantes</span><span class="sxs-lookup"><span data-stu-id="5d22d-130">participants</span></span>|<span data-ttu-id="5d22d-131">String collection</span><span class="sxs-lookup"><span data-stu-id="5d22d-131">String collection</span></span>|<span data-ttu-id="5d22d-132">Os participantes para ser ativado.</span><span class="sxs-lookup"><span data-stu-id="5d22d-132">The participants to be muted.</span></span>|
|<span data-ttu-id="5d22d-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="5d22d-133">clientContext</span></span>|<span data-ttu-id="5d22d-134">String</span><span class="sxs-lookup"><span data-stu-id="5d22d-134">String</span></span>|<span data-ttu-id="5d22d-135">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="5d22d-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="5d22d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d22d-136">Response</span></span>
<span data-ttu-id="5d22d-137">Se tiver êxito, este método retornará `200 OK` objeto response de código e [commsOperation](../resources/commsoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d22d-137">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d22d-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d22d-138">Example</span></span>
<span data-ttu-id="5d22d-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5d22d-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5d22d-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d22d-140">Request</span></span>
<span data-ttu-id="5d22d-141">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d22d-141">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "participant_muteAll"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/muteAll
Content-Type: application/json
Content-Length: 81

{
  "participants": [
    ""
  ],
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="5d22d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d22d-142">Response</span></span>

> <span data-ttu-id="5d22d-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d22d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participant: muteAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
