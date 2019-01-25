---
title: 'message: copy'
description: Copie uma mensagem para uma pasta.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a5dfd92c6478414c8890b6c411b5a9385a992198
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514247"
---
# <a name="message-copy"></a><span data-ttu-id="6eb87-103">message: copy</span><span class="sxs-lookup"><span data-stu-id="6eb87-103">message: copy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6eb87-104">Copie uma mensagem para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="6eb87-104">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="6eb87-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6eb87-105">Permissions</span></span>

<span data-ttu-id="6eb87-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6eb87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6eb87-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6eb87-108">Permission type</span></span> | <span data-ttu-id="6eb87-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6eb87-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="6eb87-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6eb87-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6eb87-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6eb87-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6eb87-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6eb87-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6eb87-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6eb87-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6eb87-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6eb87-114">Application</span></span> | <span data-ttu-id="6eb87-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6eb87-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6eb87-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6eb87-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="6eb87-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6eb87-117">Request headers</span></span>

| <span data-ttu-id="6eb87-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6eb87-118">Header</span></span> | <span data-ttu-id="6eb87-119">Valor</span><span class="sxs-lookup"><span data-stu-id="6eb87-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="6eb87-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="6eb87-120">Authorization</span></span> | <span data-ttu-id="6eb87-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="6eb87-121"></span></span> <span data-ttu-id="6eb87-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6eb87-122">Required.</span></span> |
| <span data-ttu-id="6eb87-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6eb87-123">Content-Type</span></span> | <span data-ttu-id="6eb87-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="6eb87-124"></span></span> <span data-ttu-id="6eb87-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6eb87-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6eb87-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6eb87-126">Request body</span></span>

<span data-ttu-id="6eb87-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6eb87-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6eb87-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6eb87-128">Parameter</span></span> | <span data-ttu-id="6eb87-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6eb87-129">Type</span></span> | <span data-ttu-id="6eb87-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6eb87-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="6eb87-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="6eb87-131">destinationId</span></span>|<span data-ttu-id="6eb87-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6eb87-132">String</span></span>|<span data-ttu-id="6eb87-133">O ID da pasta de destino, ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="6eb87-133">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="6eb87-134">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="6eb87-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="6eb87-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6eb87-135">Response</span></span>

<span data-ttu-id="6eb87-136">Se tiver êxito, este método retornará `201 Created` código de resposta e um recurso de [mensagem](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6eb87-136">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6eb87-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6eb87-137">Example</span></span>

<span data-ttu-id="6eb87-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6eb87-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6eb87-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6eb87-139">Request</span></span>

<span data-ttu-id="6eb87-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6eb87-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="6eb87-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="6eb87-141">Response</span></span>

<span data-ttu-id="6eb87-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6eb87-142">Here is an example of the response.</span></span>

> <span data-ttu-id="6eb87-143">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6eb87-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6eb87-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6eb87-144">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-copy.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
