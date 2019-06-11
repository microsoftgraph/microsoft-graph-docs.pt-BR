---
title: Criar mailSearchFolder
description: Use esta API para criar um novo mailSearchFolder na caixa de correio do usuário especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 55cd832b5fb6a90e919890fb05553384e58807db
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2019
ms.locfileid: "34818657"
---
# <a name="create-mailsearchfolder"></a><span data-ttu-id="9a38f-103">Criar mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="9a38f-103">Create mailSearchFolder</span></span>

<span data-ttu-id="9a38f-104">Criar um novo [mailSearchFolder](../resources/mailsearchfolder.md) na caixa de correio do usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="9a38f-104">Create a new [mailSearchFolder](../resources/mailsearchfolder.md) in the specified user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a38f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a38f-105">Permissions</span></span>

<span data-ttu-id="9a38f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a38f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9a38f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a38f-108">Permission type</span></span> | <span data-ttu-id="9a38f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a38f-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="9a38f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a38f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9a38f-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a38f-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9a38f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a38f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a38f-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a38f-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9a38f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a38f-114">Application</span></span> | <span data-ttu-id="9a38f-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a38f-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a38f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a38f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="9a38f-117">Especifique a pasta pai na URL de consulta como uma ID de pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="9a38f-117">Specify the parent folder in the query URL as a folder ID, or a well-known folder name.</span></span> <span data-ttu-id="9a38f-118">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="9a38f-118">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a38f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a38f-119">Request headers</span></span>

| <span data-ttu-id="9a38f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9a38f-120">Header</span></span> | <span data-ttu-id="9a38f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9a38f-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="9a38f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a38f-122">Authorization</span></span> | <span data-ttu-id="9a38f-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="9a38f-123"></span></span> <span data-ttu-id="9a38f-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a38f-124">Required.</span></span> |
| <span data-ttu-id="9a38f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9a38f-125">Content-Type</span></span> | <span data-ttu-id="9a38f-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="9a38f-126"></span></span> <span data-ttu-id="9a38f-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a38f-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a38f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a38f-128">Request body</span></span>

<span data-ttu-id="9a38f-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a38f-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9a38f-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9a38f-130">Parameter</span></span> | <span data-ttu-id="9a38f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a38f-131">Type</span></span> | <span data-ttu-id="9a38f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a38f-132">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="9a38f-133">@odata.type</span><span class="sxs-lookup"><span data-stu-id="9a38f-133">@odata.type</span></span> | <span data-ttu-id="9a38f-134">String</span><span class="sxs-lookup"><span data-stu-id="9a38f-134">String</span></span> | <span data-ttu-id="9a38f-135">O tipo de pasta a ser criada.</span><span class="sxs-lookup"><span data-stu-id="9a38f-135">The type of folder to be created.</span></span> <span data-ttu-id="9a38f-136">Defina como "Microsoft. Graph. mailSearchFolder".</span><span class="sxs-lookup"><span data-stu-id="9a38f-136">Set to "microsoft.graph.mailSearchFolder".</span></span> |
| <span data-ttu-id="9a38f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9a38f-137">displayName</span></span> | <span data-ttu-id="9a38f-138">String</span><span class="sxs-lookup"><span data-stu-id="9a38f-138">String</span></span> | <span data-ttu-id="9a38f-139">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="9a38f-139">The display name of the new folder.</span></span>|
| <span data-ttu-id="9a38f-140">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="9a38f-140">includeNestedFolders</span></span> | <span data-ttu-id="9a38f-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="9a38f-141">Boolean</span></span> | <span data-ttu-id="9a38f-142">Indica como a hierarquia da pasta da caixa de correio deve ser percorrida na pesquisa.</span><span class="sxs-lookup"><span data-stu-id="9a38f-142">Indicates how the mailbox folder hierarchy should be traversed in the search.</span></span> <span data-ttu-id="9a38f-143">`true`significa que uma pesquisa profunda deve ser feita para incluir pastas filhas na hierarquia de cada pasta explicitamente especificada no **sourceFolderIds**.</span><span class="sxs-lookup"><span data-stu-id="9a38f-143">`true` means that a deep search should be done to include child folders in the hierarchy of each folder explicitly specified in **sourceFolderIds**.</span></span> <span data-ttu-id="9a38f-144">`false`significa uma pesquisa superficial de apenas cada uma das pastas explicitamente especificadas no **sourceFolderIds**.</span><span class="sxs-lookup"><span data-stu-id="9a38f-144">`false` means a shallow search of only each of the folders explicitly specified in **sourceFolderIds**.</span></span> |
| <span data-ttu-id="9a38f-145">sourceFolderIds</span><span class="sxs-lookup"><span data-stu-id="9a38f-145">sourceFolderIds</span></span> | <span data-ttu-id="9a38f-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a38f-146">String collection</span></span> | <span data-ttu-id="9a38f-147">As pastas de caixa de correio que devem ser minadas.</span><span class="sxs-lookup"><span data-stu-id="9a38f-147">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="9a38f-148">filterQuery</span><span class="sxs-lookup"><span data-stu-id="9a38f-148">filterQuery</span></span> | <span data-ttu-id="9a38f-149">String</span><span class="sxs-lookup"><span data-stu-id="9a38f-149">String</span></span> | <span data-ttu-id="9a38f-150">A consulta OData para filtrar as mensagens.</span><span class="sxs-lookup"><span data-stu-id="9a38f-150">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="9a38f-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a38f-151">Response</span></span>

<span data-ttu-id="9a38f-152">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [mailSearchFolder](../resources/mailsearchfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a38f-152">If successful, this method returns a `201 Created` response code and a [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a38f-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a38f-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9a38f-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a38f-154">Request</span></span>

<span data-ttu-id="9a38f-155">Veja a seguir um exemplo de solicitação-ele cria uma pasta de pesquisa de mensagens que contêm a cadeia de caracteres "semanalmente Resumo" no assunto.</span><span class="sxs-lookup"><span data-stu-id="9a38f-155">The following is an example of the request - it creates a search folder of messages that contain the string "weekly digest" in the subject.</span></span> <span data-ttu-id="9a38f-156">A pasta de pesquisa está na mesma pasta em que a consulta de filtro especificado se aplica.</span><span class="sxs-lookup"><span data-stu-id="9a38f-156">The search folder is under the same folder on which the specified filter query applies.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADYAAAIBDAAAAA=="],
  "name": "create_mailsearchfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADYAAAIBDAAAAA==/childfolders
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "displayName": "Weekly digests",
  "includeNestedFolders": true,
  "sourceFolderIds": ["AQMkADYAAAIBDAAAAA=="],
  "filterQuery": "contains(subject, 'weekly digest')"
}
```

#### <a name="response"></a><span data-ttu-id="9a38f-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a38f-157">Response</span></span>

<span data-ttu-id="9a38f-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9a38f-158">The following is an example of the response.</span></span>

><span data-ttu-id="9a38f-159">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9a38f-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9a38f-160">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a38f-160">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/mailFolders('AQMkADYAAAIBDAAAAA%3D%3D')/childFolders/$entity",
    "@odata.type": "#microsoft.graph.mailSearchFolder",
    "id": "AAMkADYfRAAAZg1yTAAA=",
    "displayName": "Weekly digests",
    "parentFolderId": "AQMkADYAAAIBDAAAAA==",
    "childFolderCount": 0,
    "unreadItemCount": 0,
    "totalItemCount": 0,
    "wellKnownName": null,
    "isSupported": true,
    "includeNestedFolders": true,
    "sourceFolderIds": [
        "AQMkADYAAAIBDAAAAA=="
    ],
    "filterQuery": "contains(subject, 'weekly digest')"
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
  
  ]
}
-->
