---
title: 'chamar: Ativar Mudo'
description: Permite que o aplicativo ativar mudo em si.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 603c0d49f47291ec5050cd08dfbb0cc0faa2bc0e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813437"
---
# <a name="call-mute"></a><span data-ttu-id="2872c-103">chamar: Ativar Mudo</span><span class="sxs-lookup"><span data-stu-id="2872c-103">call: mute</span></span>

> <span data-ttu-id="2872c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2872c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2872c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2872c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2872c-106">Permite que o aplicativo ativar mudo em si.</span><span class="sxs-lookup"><span data-stu-id="2872c-106">Allows the application to mute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="2872c-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="2872c-107">Permissions</span></span>
<span data-ttu-id="2872c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2872c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2872c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2872c-110">Permission type</span></span>                        | <span data-ttu-id="2872c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2872c-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2872c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2872c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2872c-113">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="2872c-113">Not Supported.</span></span>                               |
| <span data-ttu-id="2872c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2872c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2872c-115">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="2872c-115">Not Supported.</span></span>                               |
| <span data-ttu-id="2872c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2872c-116">Application</span></span>                            | <span data-ttu-id="2872c-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2872c-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="2872c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2872c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/mute
POST /applications/{id}/calls/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="2872c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2872c-119">Request headers</span></span>
| <span data-ttu-id="2872c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2872c-120">Name</span></span>          | <span data-ttu-id="2872c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2872c-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2872c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2872c-122">Authorization</span></span> | <span data-ttu-id="2872c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2872c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2872c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2872c-125">Request body</span></span>
<span data-ttu-id="2872c-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2872c-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2872c-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2872c-127">Parameter</span></span>      | <span data-ttu-id="2872c-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="2872c-128">Type</span></span>    |<span data-ttu-id="2872c-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="2872c-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2872c-130">clientContext</span><span class="sxs-lookup"><span data-stu-id="2872c-130">clientContext</span></span>|<span data-ttu-id="2872c-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2872c-131">String</span></span>|<span data-ttu-id="2872c-132">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="2872c-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="2872c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2872c-133">Response</span></span>
<span data-ttu-id="2872c-134">Se tiver êxito, este método retornará `200 OK` código de resposta e um objeto [commsOperation](../resources/commsoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2872c-134">If successful, this method returns `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2872c-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2872c-135">Example</span></span>
<span data-ttu-id="2872c-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="2872c-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2872c-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2872c-137">Request</span></span>
<span data-ttu-id="2872c-138">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="2872c-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-mute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/mute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="2872c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2872c-139">Response</span></span>

> <span data-ttu-id="2872c-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2872c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
