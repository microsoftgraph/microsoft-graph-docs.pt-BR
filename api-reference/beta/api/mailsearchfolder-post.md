---
title: Criar mailSearchFolder
description: Use essa API para criar um novo mailSearchFolder na caixa de correio do usuário especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 626bf3a2e8bc77ba929895eed74ac0bb803aa5d4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912873"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="a01d2-103">Criar mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="a01d2-103">Create mailSearchFolder</span></span>

> <span data-ttu-id="a01d2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a01d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a01d2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a01d2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a01d2-106">Use essa API para criar um novo [mailSearchFolder](../resources/mailsearchfolder.md) na caixa de correio do usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="a01d2-106">Use this API to create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="a01d2-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="a01d2-107">Permissions</span></span>

<span data-ttu-id="a01d2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a01d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a01d2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a01d2-110">Permission type</span></span> | <span data-ttu-id="a01d2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a01d2-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="a01d2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a01d2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a01d2-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a01d2-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a01d2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a01d2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a01d2-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a01d2-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a01d2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a01d2-116">Application</span></span> | <span data-ttu-id="a01d2-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a01d2-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a01d2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a01d2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="a01d2-119">Especifique a pasta pai na URL de consulta como uma ID de pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="a01d2-119">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="a01d2-120">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="a01d2-120">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a01d2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a01d2-121">Request headers</span></span>

| <span data-ttu-id="a01d2-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a01d2-122">Header</span></span> | <span data-ttu-id="a01d2-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a01d2-123">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="a01d2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a01d2-124">Authorization</span></span> | <span data-ttu-id="a01d2-125">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="a01d2-125"></span></span> <span data-ttu-id="a01d2-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a01d2-126">Required.</span></span> |
| <span data-ttu-id="a01d2-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a01d2-127">Content-Type</span></span> | <span data-ttu-id="a01d2-128">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="a01d2-128"></span></span> <span data-ttu-id="a01d2-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a01d2-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a01d2-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a01d2-130">Request body</span></span>

<span data-ttu-id="a01d2-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a01d2-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a01d2-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a01d2-132">Parameter</span></span> | <span data-ttu-id="a01d2-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="a01d2-133">Type</span></span> | <span data-ttu-id="a01d2-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="a01d2-134">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="a01d2-135">@odata.type</span><span class="sxs-lookup"><span data-stu-id="a01d2-135">@odata.type</span></span> | <span data-ttu-id="a01d2-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a01d2-136">String</span></span> | <span data-ttu-id="a01d2-137">O tipo da pasta a ser criado.</span><span class="sxs-lookup"><span data-stu-id="a01d2-137">The type of folder to be created.</span></span> <span data-ttu-id="a01d2-138">Definido como "microsoft.graph.mailSearchFolder".</span><span class="sxs-lookup"><span data-stu-id="a01d2-138">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="a01d2-139">displayName</span><span class="sxs-lookup"><span data-stu-id="a01d2-139">displayName</span></span> | <span data-ttu-id="a01d2-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a01d2-140">String</span></span> | <span data-ttu-id="a01d2-141">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="a01d2-141">The display name of the new folder.</span></span>|
| <span data-ttu-id="a01d2-142">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="a01d2-142">includeNestedFolders</span></span> | <span data-ttu-id="a01d2-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="a01d2-143">Boolean</span></span> | <span data-ttu-id="a01d2-144">Como a hierarquia de pastas de caixa de correio deve ser percorrida.</span><span class="sxs-lookup"><span data-stu-id="a01d2-144">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="a01d2-145">`true`significa que uma profundidade de pesquisa deve ser feito ao `false` significa rasos de pesquisa devem ser feito em vez disso.</span><span class="sxs-lookup"><span data-stu-id="a01d2-145">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="a01d2-146">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="a01d2-146">sourceFolderIDs</span></span> | <span data-ttu-id="a01d2-147">String collection</span><span class="sxs-lookup"><span data-stu-id="a01d2-147">String collection</span></span> | <span data-ttu-id="a01d2-148">As pastas de caixa de correio que devem ser extraídas.</span><span class="sxs-lookup"><span data-stu-id="a01d2-148">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="a01d2-149">filterQuery</span><span class="sxs-lookup"><span data-stu-id="a01d2-149">filterQuery</span></span> | <span data-ttu-id="a01d2-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a01d2-150">String</span></span> | <span data-ttu-id="a01d2-151">A consulta OData para filtrar as mensagens.</span><span class="sxs-lookup"><span data-stu-id="a01d2-151">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="a01d2-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="a01d2-152">Response</span></span>

<span data-ttu-id="a01d2-153">Se tiver êxito, este método retornará `201 Created` código de resposta e um objeto [mailSearchFolder](../resources/mailsearchfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a01d2-153">If successful, this method returns `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a01d2-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a01d2-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a01d2-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a01d2-155">Request</span></span>

<span data-ttu-id="a01d2-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a01d2-156">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailsearchfolder"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childfolders
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "displayName": "Get MyAnalytics",
  "includeNestedFolders": true,
  "sourceFolderIDs": ["AAMkAGVmMDEzM"],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```

#### <a name="response"></a><span data-ttu-id="a01d2-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="a01d2-157">Response</span></span>

<span data-ttu-id="a01d2-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a01d2-158">The following is an example of the response.</span></span>

><span data-ttu-id="a01d2-159">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a01d2-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a01d2-160">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a01d2-160">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzMx",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzMy",
  "childFolderCount": 0,
  "unreadItemCount": 0,
  "totalItemCount": 13,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": [
    "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
