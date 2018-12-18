---
title: 'chamar: Ativar Mudo'
description: Permite que o aplicativo ativar mudo em si.
author: VinodRavichandran
ms.openlocfilehash: 54de4aa598500d1effa1c66c74e5809ad3570959
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341584"
---
# <a name="call-mute"></a><span data-ttu-id="fa023-103">chamar: Ativar Mudo</span><span class="sxs-lookup"><span data-stu-id="fa023-103">call: mute</span></span>

> <span data-ttu-id="fa023-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fa023-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa023-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fa023-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa023-106">Permite que o aplicativo ativar mudo em si.</span><span class="sxs-lookup"><span data-stu-id="fa023-106">Allows the application to mute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa023-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa023-107">Permissions</span></span>
<span data-ttu-id="fa023-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa023-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa023-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa023-110">Permission type</span></span>                        | <span data-ttu-id="fa023-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa023-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fa023-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa023-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa023-113">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="fa023-113">Not Supported.</span></span>                               |
| <span data-ttu-id="fa023-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa023-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa023-115">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="fa023-115">Not Supported.</span></span>                               |
| <span data-ttu-id="fa023-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa023-116">Application</span></span>                            | <span data-ttu-id="fa023-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fa023-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="fa023-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa023-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/mute
POST /applications/{id}/calls/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="fa023-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa023-119">Request headers</span></span>
| <span data-ttu-id="fa023-120">Nome</span><span class="sxs-lookup"><span data-stu-id="fa023-120">Name</span></span>          | <span data-ttu-id="fa023-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa023-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="fa023-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa023-122">Authorization</span></span> | <span data-ttu-id="fa023-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa023-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa023-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa023-125">Request body</span></span>
<span data-ttu-id="fa023-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa023-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fa023-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fa023-127">Parameter</span></span>      | <span data-ttu-id="fa023-128">Type</span><span class="sxs-lookup"><span data-stu-id="fa023-128">Type</span></span>    |<span data-ttu-id="fa023-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa023-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa023-130">clientContext</span><span class="sxs-lookup"><span data-stu-id="fa023-130">clientContext</span></span>|<span data-ttu-id="fa023-131">String</span><span class="sxs-lookup"><span data-stu-id="fa023-131">String</span></span>|<span data-ttu-id="fa023-132">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="fa023-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="fa023-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa023-133">Response</span></span>
<span data-ttu-id="fa023-134">Se tiver êxito, este método retornará `200 OK` código de resposta e um objeto [commsOperation](../resources/commsoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa023-134">If successful, this method returns `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa023-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa023-135">Example</span></span>
<span data-ttu-id="fa023-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="fa023-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="fa023-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa023-137">Request</span></span>
<span data-ttu-id="fa023-138">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa023-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_mute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/mute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="fa023-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa023-139">Response</span></span>

> <span data-ttu-id="fa023-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa023-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "call: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
