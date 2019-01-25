---
title: Criar mailSearchFolder
description: Use essa API para criar um novo mailSearchFolder na caixa de correio do usuário especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7ef9992e1b0eaee83c39831424215cb9756f895d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517726"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="f6dcf-103">Criar mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="f6dcf-103">Create mailSearchFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6dcf-104">Use essa API para criar um novo [mailSearchFolder](../resources/mailsearchfolder.md) na caixa de correio do usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="f6dcf-104">Use this API to create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6dcf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f6dcf-105">Permissions</span></span>

<span data-ttu-id="f6dcf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6dcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f6dcf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6dcf-108">Permission type</span></span> | <span data-ttu-id="f6dcf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f6dcf-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="f6dcf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6dcf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f6dcf-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6dcf-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f6dcf-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6dcf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6dcf-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6dcf-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f6dcf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6dcf-114">Application</span></span> | <span data-ttu-id="f6dcf-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6dcf-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6dcf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6dcf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="f6dcf-117">Especifique a pasta pai na URL de consulta como uma ID de pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="f6dcf-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="f6dcf-118">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="f6dcf-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6dcf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6dcf-119">Request headers</span></span>

| <span data-ttu-id="f6dcf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f6dcf-120">Header</span></span> | <span data-ttu-id="f6dcf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f6dcf-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="f6dcf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6dcf-122">Authorization</span></span> | <span data-ttu-id="f6dcf-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="f6dcf-123"></span></span> <span data-ttu-id="f6dcf-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6dcf-124">Required.</span></span> |
| <span data-ttu-id="f6dcf-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f6dcf-125">Content-Type</span></span> | <span data-ttu-id="f6dcf-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="f6dcf-126"></span></span> <span data-ttu-id="f6dcf-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6dcf-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6dcf-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6dcf-128">Request body</span></span>

<span data-ttu-id="f6dcf-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6dcf-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f6dcf-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f6dcf-130">Parameter</span></span> | <span data-ttu-id="f6dcf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6dcf-131">Type</span></span> | <span data-ttu-id="f6dcf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6dcf-132">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="f6dcf-133">@odata.type</span><span class="sxs-lookup"><span data-stu-id="f6dcf-133">@odata.type</span></span> | <span data-ttu-id="f6dcf-134">String</span><span class="sxs-lookup"><span data-stu-id="f6dcf-134">String</span></span> | <span data-ttu-id="f6dcf-135">O tipo da pasta a ser criado.</span><span class="sxs-lookup"><span data-stu-id="f6dcf-135">The type of folder to be created.</span></span> <span data-ttu-id="f6dcf-136">Definido como "microsoft.graph.mailSearchFolder".</span><span class="sxs-lookup"><span data-stu-id="f6dcf-136">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="f6dcf-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f6dcf-137">displayName</span></span> | <span data-ttu-id="f6dcf-138">String</span><span class="sxs-lookup"><span data-stu-id="f6dcf-138">String</span></span> | <span data-ttu-id="f6dcf-139">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="f6dcf-139">The display name of the new folder.</span></span>|
| <span data-ttu-id="f6dcf-140">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="f6dcf-140">includeNestedFolders</span></span> | <span data-ttu-id="f6dcf-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6dcf-141">Boolean</span></span> | <span data-ttu-id="f6dcf-142">Como a hierarquia de pastas de caixa de correio deve ser percorrida.</span><span class="sxs-lookup"><span data-stu-id="f6dcf-142">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="f6dcf-143">`true`significa que uma profundidade de pesquisa deve ser feito ao `false` significa rasos de pesquisa devem ser feito em vez disso.</span><span class="sxs-lookup"><span data-stu-id="f6dcf-143">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="f6dcf-144">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="f6dcf-144">sourceFolderIDs</span></span> | <span data-ttu-id="f6dcf-145">String collection</span><span class="sxs-lookup"><span data-stu-id="f6dcf-145">String collection</span></span> | <span data-ttu-id="f6dcf-146">As pastas de caixa de correio que devem ser extraídas.</span><span class="sxs-lookup"><span data-stu-id="f6dcf-146">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="f6dcf-147">filterQuery</span><span class="sxs-lookup"><span data-stu-id="f6dcf-147">filterQuery</span></span> | <span data-ttu-id="f6dcf-148">String</span><span class="sxs-lookup"><span data-stu-id="f6dcf-148">String</span></span> | <span data-ttu-id="f6dcf-149">A consulta OData para filtrar as mensagens.</span><span class="sxs-lookup"><span data-stu-id="f6dcf-149">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="f6dcf-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6dcf-150">Response</span></span>

<span data-ttu-id="f6dcf-151">Se tiver êxito, este método retornará `201 Created` código de resposta e um objeto [mailSearchFolder](../resources/mailsearchfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6dcf-151">If successful, this method returns `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6dcf-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6dcf-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f6dcf-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6dcf-153">Request</span></span>

<span data-ttu-id="f6dcf-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6dcf-154">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="f6dcf-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6dcf-155">Response</span></span>

<span data-ttu-id="f6dcf-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f6dcf-156">The following is an example of the response.</span></span>

><span data-ttu-id="f6dcf-157">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f6dcf-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f6dcf-158">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f6dcf-158">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailsearchfolder-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
