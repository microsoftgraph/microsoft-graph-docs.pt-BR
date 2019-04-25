---
title: 'participante: muteAll'
description: Ative o mudo para todos os participantes em uma chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2a74a224141b77f0a09718bbafee3cf1dab0e8e9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539369"
---
# <a name="participant-muteall"></a><span data-ttu-id="e81e5-103">participante: muteAll</span><span class="sxs-lookup"><span data-stu-id="e81e5-103">participant: muteAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e81e5-104">Ative o mudo para todos os participantes em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="e81e5-104">Mute all participants in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="e81e5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e81e5-105">Permissions</span></span>
<span data-ttu-id="e81e5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e81e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e81e5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e81e5-108">Permission type</span></span>                        | <span data-ttu-id="e81e5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e81e5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e81e5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e81e5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e81e5-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="e81e5-111">Not Supported</span></span>                               |
| <span data-ttu-id="e81e5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e81e5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e81e5-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="e81e5-113">Not Supported</span></span>                               |
| <span data-ttu-id="e81e5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e81e5-114">Application</span></span>                            | <span data-ttu-id="e81e5-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e81e5-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="e81e5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e81e5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /applications/{id}/calls/{id}/participants/muteAll
```

## <a name="request-headers"></a><span data-ttu-id="e81e5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e81e5-117">Request headers</span></span>
| <span data-ttu-id="e81e5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e81e5-118">Name</span></span>          | <span data-ttu-id="e81e5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e81e5-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e81e5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e81e5-120">Authorization</span></span> | <span data-ttu-id="e81e5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e81e5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e81e5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e81e5-123">Request body</span></span>
<span data-ttu-id="e81e5-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e81e5-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e81e5-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e81e5-125">Parameter</span></span>      | <span data-ttu-id="e81e5-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e81e5-126">Type</span></span>    |<span data-ttu-id="e81e5-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e81e5-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e81e5-128">participantes</span><span class="sxs-lookup"><span data-stu-id="e81e5-128">participants</span></span>|<span data-ttu-id="e81e5-129">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e81e5-129">String collection</span></span>|<span data-ttu-id="e81e5-130">Os participantes a serem mudo.</span><span class="sxs-lookup"><span data-stu-id="e81e5-130">The participants to be muted.</span></span>|
|<span data-ttu-id="e81e5-131">clientContext</span><span class="sxs-lookup"><span data-stu-id="e81e5-131">clientContext</span></span>|<span data-ttu-id="e81e5-132">String</span><span class="sxs-lookup"><span data-stu-id="e81e5-132">String</span></span>|<span data-ttu-id="e81e5-133">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="e81e5-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="e81e5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e81e5-134">Response</span></span>
<span data-ttu-id="e81e5-135">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [commsOperation](../resources/commsoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e81e5-135">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e81e5-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e81e5-136">Example</span></span>
<span data-ttu-id="e81e5-137">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e81e5-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e81e5-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e81e5-138">Request</span></span>
<span data-ttu-id="e81e5-139">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="e81e5-139">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "participant-muteAll"
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

##### <a name="response"></a><span data-ttu-id="e81e5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e81e5-140">Response</span></span>

> <span data-ttu-id="e81e5-p103">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e81e5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "participant: muteAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/participant-muteall.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
