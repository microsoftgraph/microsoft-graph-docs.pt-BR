---
title: 'chamar: Desativar Mudo'
description: Permite que o aplicativo para desativar o mudo.
author: VinodRavichandran
ms.openlocfilehash: abd5abdf0e91a24e2f8de4d5fbb3fa0cc1d7b243
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380398"
---
# <a name="call-unmute"></a><span data-ttu-id="2565f-103">chamar: Desativar Mudo</span><span class="sxs-lookup"><span data-stu-id="2565f-103">call: unmute</span></span>

> <span data-ttu-id="2565f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2565f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2565f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2565f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2565f-106">Permite que o aplicativo para desativar o mudo.</span><span class="sxs-lookup"><span data-stu-id="2565f-106">Allows the application to unmute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="2565f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2565f-107">Permissions</span></span>
<span data-ttu-id="2565f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2565f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2565f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2565f-110">Permission type</span></span>                        | <span data-ttu-id="2565f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2565f-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2565f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2565f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2565f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2565f-113">Not supported.</span></span>                               |
| <span data-ttu-id="2565f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2565f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2565f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2565f-115">Not supported.</span></span>                               |
| <span data-ttu-id="2565f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2565f-116">Application</span></span>                            | <span data-ttu-id="2565f-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2565f-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="2565f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2565f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/unmute
POST /applications/{id}/calls/{id}/unmute
```

## <a name="request-headers"></a><span data-ttu-id="2565f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2565f-119">Request headers</span></span>
| <span data-ttu-id="2565f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2565f-120">Name</span></span>          | <span data-ttu-id="2565f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2565f-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2565f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2565f-122">Authorization</span></span> | <span data-ttu-id="2565f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2565f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2565f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2565f-125">Request body</span></span>
<span data-ttu-id="2565f-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2565f-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2565f-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2565f-127">Parameter</span></span>      | <span data-ttu-id="2565f-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="2565f-128">Type</span></span>    |<span data-ttu-id="2565f-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="2565f-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2565f-130">clientContext</span><span class="sxs-lookup"><span data-stu-id="2565f-130">clientContext</span></span>|<span data-ttu-id="2565f-131">String</span><span class="sxs-lookup"><span data-stu-id="2565f-131">String</span></span>|<span data-ttu-id="2565f-132">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="2565f-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="2565f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2565f-133">Response</span></span>
<span data-ttu-id="2565f-134">Se tiver êxito, este método retornará `200 OK` objeto response de código e [commsOperation](../resources/commsoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2565f-134">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2565f-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2565f-135">Example</span></span>
<span data-ttu-id="2565f-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="2565f-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2565f-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2565f-137">Request</span></span>
<span data-ttu-id="2565f-138">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="2565f-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-unmute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/unmute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="2565f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2565f-139">Response</span></span>

> <span data-ttu-id="2565f-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2565f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "call: unmute",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
