---
title: 'chamar: changeScreenSharingRole'
description: Iniciar e interromper o compartilhamento de tela na chamada. Essa API é usada para permitir que aplicativos compartilhar o conteúdo de tela com os participantes de uma chamada ou reunião.
ms.openlocfilehash: f0aa69b43813bd248048ad1bd965dfbc4afc012b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036545"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="b9678-104">chamar: changeScreenSharingRole</span><span class="sxs-lookup"><span data-stu-id="b9678-104">call: changeScreenSharingRole</span></span>

> <span data-ttu-id="b9678-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b9678-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9678-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b9678-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9678-107">Iniciar e interromper o compartilhamento de tela na chamada.</span><span class="sxs-lookup"><span data-stu-id="b9678-107">Start and stop sharing screen in the call.</span></span> <span data-ttu-id="b9678-108">Essa API é usada para permitir que aplicativos compartilhar o conteúdo de tela com os participantes de uma chamada ou reunião.</span><span class="sxs-lookup"><span data-stu-id="b9678-108">This API is used to allow applications to share screen content with the participants of a call or meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9678-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="b9678-109">Permissions</span></span>
<span data-ttu-id="b9678-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9678-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9678-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9678-112">Permission type</span></span>                        | <span data-ttu-id="b9678-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9678-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b9678-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9678-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9678-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="b9678-115">Not Supported</span></span>                               |
| <span data-ttu-id="b9678-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9678-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9678-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="b9678-117">Not Supported</span></span>                               |
| <span data-ttu-id="b9678-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9678-118">Application</span></span>                            | <span data-ttu-id="b9678-119">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="b9678-119">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="b9678-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9678-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /applications/{id}/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="b9678-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9678-121">Request headers</span></span>
| <span data-ttu-id="b9678-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b9678-122">Name</span></span>          | <span data-ttu-id="b9678-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9678-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b9678-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9678-124">Authorization</span></span> | <span data-ttu-id="b9678-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9678-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9678-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9678-127">Request body</span></span>
<span data-ttu-id="b9678-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9678-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b9678-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b9678-129">Parameter</span></span>      | <span data-ttu-id="b9678-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9678-130">Type</span></span>    |<span data-ttu-id="b9678-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9678-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9678-132">role</span><span class="sxs-lookup"><span data-stu-id="b9678-132">role</span></span>|<span data-ttu-id="b9678-133">String</span><span class="sxs-lookup"><span data-stu-id="b9678-133">String</span></span>|<span data-ttu-id="b9678-134">Os valores possíveis são: 'Visualizador', 'Compartilhador'</span><span class="sxs-lookup"><span data-stu-id="b9678-134">Possible values are: 'Viewer', 'Sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="b9678-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9678-135">Response</span></span>
<span data-ttu-id="b9678-136">Retorna `202 Accepted` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="b9678-136">Returns `202 Accepted` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b9678-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9678-137">Example</span></span>
<span data-ttu-id="b9678-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="b9678-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b9678-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9678-139">Request</span></span>
<span data-ttu-id="b9678-140">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9678-140">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```

##### <a name="response"></a><span data-ttu-id="b9678-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9678-141">Response</span></span>
<span data-ttu-id="b9678-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9678-142">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: changeScreenSharingRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
