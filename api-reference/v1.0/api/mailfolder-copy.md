---
title: 'mailFolder: copy'
description: Copie uma mailFolder e seu conteúdo para outra mailFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 37160f5b6f62ce29d605e84a93a7748f426bd240
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940733"
---
# <a name="mailfolder-copy"></a><span data-ttu-id="f91d6-103">mailFolder: copy</span><span class="sxs-lookup"><span data-stu-id="f91d6-103">mailFolder: copy</span></span>

<span data-ttu-id="f91d6-104">Copie uma mailFolder e seu conteúdo para outra mailFolder.</span><span class="sxs-lookup"><span data-stu-id="f91d6-104">Copy a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="f91d6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f91d6-105">Permissions</span></span>

<span data-ttu-id="f91d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f91d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f91d6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f91d6-108">Permission type</span></span> | <span data-ttu-id="f91d6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f91d6-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="f91d6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f91d6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f91d6-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f91d6-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f91d6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f91d6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f91d6-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f91d6-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f91d6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f91d6-114">Application</span></span> | <span data-ttu-id="f91d6-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f91d6-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f91d6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f91d6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="f91d6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f91d6-117">Request headers</span></span>
| <span data-ttu-id="f91d6-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f91d6-118">Header</span></span> | <span data-ttu-id="f91d6-119">Valor</span><span class="sxs-lookup"><span data-stu-id="f91d6-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="f91d6-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f91d6-120">Authorization</span></span> | <span data-ttu-id="f91d6-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="f91d6-121"></span></span> <span data-ttu-id="f91d6-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f91d6-122">Required.</span></span> |
| <span data-ttu-id="f91d6-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f91d6-123">Content-Type</span></span> | <span data-ttu-id="f91d6-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="f91d6-124"></span></span> <span data-ttu-id="f91d6-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f91d6-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f91d6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f91d6-126">Request body</span></span>

<span data-ttu-id="f91d6-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f91d6-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f91d6-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f91d6-128">Parameter</span></span> | <span data-ttu-id="f91d6-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f91d6-129">Type</span></span> | <span data-ttu-id="f91d6-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f91d6-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="f91d6-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="f91d6-131">destinationId</span></span>|<span data-ttu-id="f91d6-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f91d6-132">String</span></span>|<span data-ttu-id="f91d6-133">O ID da pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="f91d6-133">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="f91d6-134">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="f91d6-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="f91d6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f91d6-135">Response</span></span>

<span data-ttu-id="f91d6-136">Se tiver êxito, este método retornará `200 OK` código de resposta e um recurso [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f91d6-136">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f91d6-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f91d6-137">Example</span></span>

<span data-ttu-id="f91d6-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f91d6-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f91d6-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f91d6-139">Request</span></span>
<span data-ttu-id="f91d6-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f91d6-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "mailfolder_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="f91d6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f91d6-141">Response</span></span>

<span data-ttu-id="f91d6-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f91d6-142">Here is an example of the response.</span></span>

> <span data-ttu-id="f91d6-143">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f91d6-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f91d6-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f91d6-144">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
