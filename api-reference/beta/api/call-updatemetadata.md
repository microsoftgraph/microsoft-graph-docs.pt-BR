---
title: 'chamar: updateMetadata'
description: Atualize os metadados do aplicativo associado a uma chamada.
author: VinodRavichandran
ms.openlocfilehash: b81b41b827aee17fbc2ebed2dee56c15c5376a88
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380538"
---
# <a name="call-updatemetadata"></a><span data-ttu-id="a10d2-103">chamar: updateMetadata</span><span class="sxs-lookup"><span data-stu-id="a10d2-103">call: updateMetadata</span></span>

> <span data-ttu-id="a10d2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a10d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a10d2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a10d2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a10d2-106">Atualize os metadados do aplicativo associado a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="a10d2-106">Update the appliation's metadata associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="a10d2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a10d2-107">Permissions</span></span>
<span data-ttu-id="a10d2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a10d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a10d2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a10d2-110">Permission type</span></span>                        | <span data-ttu-id="a10d2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a10d2-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a10d2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a10d2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a10d2-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="a10d2-113">Not Supported</span></span>                               |
| <span data-ttu-id="a10d2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a10d2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a10d2-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="a10d2-115">Not Supported</span></span>                               |
| <span data-ttu-id="a10d2-116">Application</span><span class="sxs-lookup"><span data-stu-id="a10d2-116">Application</span></span>     | <span data-ttu-id="a10d2-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="a10d2-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a10d2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a10d2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateMetadata
POST /applications/{id}/calls/{id}/updateMetadata
```

## <a name="request-headers"></a><span data-ttu-id="a10d2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a10d2-119">Request headers</span></span>
| <span data-ttu-id="a10d2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a10d2-120">Name</span></span>          | <span data-ttu-id="a10d2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a10d2-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a10d2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a10d2-122">Authorization</span></span> | <span data-ttu-id="a10d2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a10d2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a10d2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a10d2-125">Request body</span></span>
<span data-ttu-id="a10d2-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a10d2-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a10d2-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a10d2-127">Parameter</span></span>      | <span data-ttu-id="a10d2-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="a10d2-128">Type</span></span>    |<span data-ttu-id="a10d2-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="a10d2-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a10d2-130">metadados</span><span class="sxs-lookup"><span data-stu-id="a10d2-130">metadata</span></span>|<span data-ttu-id="a10d2-131">String</span><span class="sxs-lookup"><span data-stu-id="a10d2-131">String</span></span>|<span data-ttu-id="a10d2-132">Um blob de dados fornecidos pelo participante na lista.</span><span class="sxs-lookup"><span data-stu-id="a10d2-132">A blob of data provided by the participant in the roster.</span></span>|
|<span data-ttu-id="a10d2-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="a10d2-133">clientContext</span></span>|<span data-ttu-id="a10d2-134">String</span><span class="sxs-lookup"><span data-stu-id="a10d2-134">String</span></span>|<span data-ttu-id="a10d2-135">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="a10d2-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="a10d2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a10d2-136">Response</span></span>
<span data-ttu-id="a10d2-137">Retorna `202 Accepted` código de resposta e um cabeçalho de local com um uri para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="a10d2-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="a10d2-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a10d2-138">Example</span></span>
<span data-ttu-id="a10d2-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="a10d2-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a10d2-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a10d2-140">Request</span></span>
<span data-ttu-id="a10d2-141">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="a10d2-141">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-updateMetadata"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/updateMetadata
Content-Type: application/json
Content-Length: 79

{
  "metadata": "metadata-value",
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="a10d2-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a10d2-142">Response</span></span>

> <span data-ttu-id="a10d2-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a10d2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: updateMetadata",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
