---
title: Criar mailFolder
description: Use essa API para criar um novo mailFolder de filho.
ms.openlocfilehash: 44d9e9ebfd721a68734376342500ad1e2a182cda
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037529"
---
# <a name="create-mailfolder"></a><span data-ttu-id="c6939-103">Criar mailFolder</span><span class="sxs-lookup"><span data-stu-id="c6939-103">Create mailFolder</span></span>

> <span data-ttu-id="c6939-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c6939-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6939-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c6939-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c6939-106">Use essa API para criar um novo de filho [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c6939-106">Use this API to create a new child [mailFolder](../resources/mailfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c6939-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="c6939-107">Permissions</span></span>

<span data-ttu-id="c6939-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6939-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c6939-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6939-110">Permission type</span></span> | <span data-ttu-id="c6939-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6939-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="c6939-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6939-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c6939-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6939-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c6939-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6939-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6939-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6939-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c6939-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6939-116">Application</span></span> | <span data-ttu-id="c6939-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6939-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6939-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6939-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="c6939-119">Especifique a pasta pai na URL de consulta como uma ID de pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="c6939-119">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="c6939-120">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c6939-120">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c6939-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6939-121">Request headers</span></span>

| <span data-ttu-id="c6939-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c6939-122">Header</span></span> | <span data-ttu-id="c6939-123">Valor</span><span class="sxs-lookup"><span data-stu-id="c6939-123">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="c6939-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6939-124">Authorization</span></span> | <span data-ttu-id="c6939-125">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="c6939-125"></span></span> <span data-ttu-id="c6939-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6939-126">Required.</span></span> |
| <span data-ttu-id="c6939-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c6939-127">Content-Type</span></span> | <span data-ttu-id="c6939-128">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="c6939-128"></span></span> <span data-ttu-id="c6939-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6939-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6939-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6939-130">Request body</span></span>

<span data-ttu-id="c6939-p106">No corpo da solicitação, forneça um objeto JSON com os parâmetros a seguir. **displayName** é a única propriedade gravável para um objeto [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c6939-p106">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="c6939-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c6939-133">Parameter</span></span> | <span data-ttu-id="c6939-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6939-134">Type</span></span> | <span data-ttu-id="c6939-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6939-135">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="c6939-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c6939-136">displayName</span></span>|<span data-ttu-id="c6939-137">String</span><span class="sxs-lookup"><span data-stu-id="c6939-137">String</span></span>|<span data-ttu-id="c6939-138">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="c6939-138">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="c6939-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6939-139">Response</span></span>

<span data-ttu-id="c6939-140">Se tiver êxito, este método retornará `201 Created` código de resposta e um objeto [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6939-140">If successful, this method returns `201 Created` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6939-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6939-141">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c6939-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6939-142">Request</span></span>

<span data-ttu-id="c6939-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6939-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

#### <a name="response"></a><span data-ttu-id="c6939-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6939-144">Response</span></span>

<span data-ttu-id="c6939-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c6939-145">The following is an example of the response.</span></span>

> <span data-ttu-id="c6939-146">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c6939-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c6939-147">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6939-147">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
