---
title: Criar MailFolder
description: Use essa API para criar uma nova mailfolder filha.
author: angelgolfer-ms
ms.openlocfilehash: 717baa63f3bb15355eaf59387b8fc701ab1288b7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331518"
---
# <a name="create-mailfolder"></a><span data-ttu-id="c56d3-103">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="c56d3-103">Create MailFolder</span></span>

<span data-ttu-id="c56d3-104">Use essa API para criar uma nova mailfolder filha.</span><span class="sxs-lookup"><span data-stu-id="c56d3-104">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="c56d3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c56d3-105">Permissions</span></span>

<span data-ttu-id="c56d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c56d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c56d3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c56d3-108">Permission type</span></span> | <span data-ttu-id="c56d3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c56d3-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="c56d3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c56d3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c56d3-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c56d3-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c56d3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c56d3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c56d3-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c56d3-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c56d3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c56d3-114">Application</span></span> | <span data-ttu-id="c56d3-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c56d3-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c56d3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c56d3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="c56d3-117">Especifique a pasta pai na URL de consulta como uma ID de pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="c56d3-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="c56d3-118">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c56d3-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c56d3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c56d3-119">Request headers</span></span>

| <span data-ttu-id="c56d3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c56d3-120">Header</span></span> | <span data-ttu-id="c56d3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c56d3-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="c56d3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c56d3-122">Authorization</span></span> | <span data-ttu-id="c56d3-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="c56d3-123"></span></span> <span data-ttu-id="c56d3-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c56d3-124">Required.</span></span> |
| <span data-ttu-id="c56d3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c56d3-125">Content-Type</span></span> | <span data-ttu-id="c56d3-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="c56d3-126"></span></span> <span data-ttu-id="c56d3-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c56d3-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c56d3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c56d3-128">Request body</span></span>

<span data-ttu-id="c56d3-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c56d3-129">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="c56d3-130">**displayName** é a propriedade gravável apenas para um objeto [mailFolder](../resources/mailfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="c56d3-130">**displayName** is the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="c56d3-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c56d3-131">Parameter</span></span> | <span data-ttu-id="c56d3-132">Type</span><span class="sxs-lookup"><span data-stu-id="c56d3-132">Type</span></span> | <span data-ttu-id="c56d3-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="c56d3-133">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="c56d3-134">displayName</span><span class="sxs-lookup"><span data-stu-id="c56d3-134">displayName</span></span>|<span data-ttu-id="c56d3-135">String</span><span class="sxs-lookup"><span data-stu-id="c56d3-135">String</span></span>|<span data-ttu-id="c56d3-136">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="c56d3-136">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="c56d3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c56d3-137">Response</span></span>

<span data-ttu-id="c56d3-138">Se tiver êxito, este método retornará `201 Created` código de resposta e um recurso [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c56d3-138">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c56d3-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c56d3-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c56d3-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c56d3-140">Request</span></span>

<span data-ttu-id="c56d3-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c56d3-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

##### <a name="response"></a><span data-ttu-id="c56d3-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c56d3-142">Response</span></span>
<span data-ttu-id="c56d3-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c56d3-143">Here is an example of the response.</span></span>

> <span data-ttu-id="c56d3-144">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c56d3-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c56d3-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c56d3-145">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
