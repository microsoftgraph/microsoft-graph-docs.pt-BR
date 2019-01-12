---
title: 'message: copy'
description: Copie uma mensagem para uma pasta.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: cacc827079089cf977a28f5bb45bb1ac62884275
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934713"
---
# <a name="message-copy"></a><span data-ttu-id="13428-103">message: copy</span><span class="sxs-lookup"><span data-stu-id="13428-103">message: copy</span></span>

> <span data-ttu-id="13428-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="13428-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13428-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="13428-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13428-106">Copie uma mensagem para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="13428-106">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="13428-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="13428-107">Permissions</span></span>

<span data-ttu-id="13428-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13428-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="13428-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13428-110">Permission type</span></span> | <span data-ttu-id="13428-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13428-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="13428-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13428-112">Delegated (work or school account)</span></span> | <span data-ttu-id="13428-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13428-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="13428-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13428-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13428-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13428-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="13428-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13428-116">Application</span></span> | <span data-ttu-id="13428-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13428-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="13428-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13428-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="13428-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13428-119">Request headers</span></span>

| <span data-ttu-id="13428-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13428-120">Header</span></span> | <span data-ttu-id="13428-121">Valor</span><span class="sxs-lookup"><span data-stu-id="13428-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="13428-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="13428-122">Authorization</span></span> | <span data-ttu-id="13428-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="13428-123"></span></span> <span data-ttu-id="13428-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13428-124">Required.</span></span> |
| <span data-ttu-id="13428-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="13428-125">Content-Type</span></span> | <span data-ttu-id="13428-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="13428-126"></span></span> <span data-ttu-id="13428-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13428-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13428-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13428-128">Request body</span></span>

<span data-ttu-id="13428-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13428-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="13428-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="13428-130">Parameter</span></span> | <span data-ttu-id="13428-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="13428-131">Type</span></span> | <span data-ttu-id="13428-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="13428-132">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="13428-133">destinationId</span><span class="sxs-lookup"><span data-stu-id="13428-133">destinationId</span></span>|<span data-ttu-id="13428-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13428-134">String</span></span>|<span data-ttu-id="13428-135">O ID da pasta de destino, ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="13428-135">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="13428-136">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="13428-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="13428-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="13428-137">Response</span></span>

<span data-ttu-id="13428-138">Se tiver êxito, este método retornará `201 Created` código de resposta e um recurso de [mensagem](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13428-138">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13428-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13428-139">Example</span></span>

<span data-ttu-id="13428-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="13428-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="13428-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13428-141">Request</span></span>

<span data-ttu-id="13428-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13428-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="13428-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="13428-143">Response</span></span>

<span data-ttu-id="13428-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13428-144">Here is an example of the response.</span></span>

> <span data-ttu-id="13428-145">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="13428-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="13428-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13428-146">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
