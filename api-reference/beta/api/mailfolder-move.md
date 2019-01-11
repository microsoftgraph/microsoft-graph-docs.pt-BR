---
title: 'mailFolder: move'
description: Mova uma mailFolder e seu conteúdo para outra mailFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 8d96e01c54c91b3de38b0594c29e38ccf8691603
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831112"
---
# <a name="mailfolder-move"></a><span data-ttu-id="3fdeb-103">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="3fdeb-103">mailFolder: move</span></span>

> <span data-ttu-id="3fdeb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3fdeb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3fdeb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3fdeb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3fdeb-106">Mova uma mailFolder e seu conteúdo para outra mailFolder.</span><span class="sxs-lookup"><span data-stu-id="3fdeb-106">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="3fdeb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3fdeb-107">Permissions</span></span>

<span data-ttu-id="3fdeb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fdeb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3fdeb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3fdeb-110">Permission type</span></span> | <span data-ttu-id="3fdeb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3fdeb-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="3fdeb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3fdeb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3fdeb-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fdeb-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3fdeb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3fdeb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fdeb-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fdeb-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3fdeb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3fdeb-116">Application</span></span> | <span data-ttu-id="3fdeb-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fdeb-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3fdeb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3fdeb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="3fdeb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3fdeb-119">Request headers</span></span>

| <span data-ttu-id="3fdeb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3fdeb-120">Header</span></span> | <span data-ttu-id="3fdeb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3fdeb-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="3fdeb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3fdeb-122">Authorization</span></span> | <span data-ttu-id="3fdeb-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="3fdeb-123"></span></span> <span data-ttu-id="3fdeb-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3fdeb-124">Required.</span></span> |
| <span data-ttu-id="3fdeb-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3fdeb-125">Content-Type</span></span> | <span data-ttu-id="3fdeb-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="3fdeb-126"></span></span> <span data-ttu-id="3fdeb-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3fdeb-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3fdeb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3fdeb-128">Request body</span></span>

<span data-ttu-id="3fdeb-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3fdeb-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3fdeb-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3fdeb-130">Parameter</span></span> | <span data-ttu-id="3fdeb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fdeb-131">Type</span></span> | <span data-ttu-id="3fdeb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fdeb-132">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="3fdeb-133">destinationId</span><span class="sxs-lookup"><span data-stu-id="3fdeb-133">destinationId</span></span>|<span data-ttu-id="3fdeb-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3fdeb-134">String</span></span>|<span data-ttu-id="3fdeb-135">O ID da pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="3fdeb-135">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="3fdeb-136">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="3fdeb-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="3fdeb-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fdeb-137">Response</span></span>

<span data-ttu-id="3fdeb-138">Se tiver êxito, este método retornará `200 OK` código de resposta e um objeto [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3fdeb-138">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fdeb-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3fdeb-139">Example</span></span>

<span data-ttu-id="3fdeb-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3fdeb-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="3fdeb-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3fdeb-141">Request</span></span>

<span data-ttu-id="3fdeb-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3fdeb-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "mailfolder_move"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/move
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="3fdeb-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fdeb-143">Response</span></span>

<span data-ttu-id="3fdeb-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3fdeb-144">Here is an example of the response.</span></span>

> <span data-ttu-id="3fdeb-145">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3fdeb-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3fdeb-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3fdeb-146">All the properties will be returned from an actual call.</span></span>
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
  "description": "mailFolder: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
