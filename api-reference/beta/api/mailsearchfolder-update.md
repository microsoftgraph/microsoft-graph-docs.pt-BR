---
title: Atualizar mailSearchFolder
description: Atualize as propriedades graváveis do objeto mailSearchFolder.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 54e901751fc404ba2099205c6b16d86c99d9b05f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540595"
---
# <a name="update-mailsearchfolder"></a><span data-ttu-id="0660b-103">Atualizar mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="0660b-103">Update mailSearchFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0660b-104">Atualize as propriedades graváveis do objeto [mailSearchFolder](../resources/mailsearchfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="0660b-104">Update the writable properties of [mailSearchFolder](../resources/mailsearchfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0660b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0660b-105">Permissions</span></span>
<span data-ttu-id="0660b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0660b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0660b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0660b-108">Permission type</span></span>      | <span data-ttu-id="0660b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0660b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0660b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0660b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0660b-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0660b-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0660b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0660b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0660b-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0660b-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0660b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0660b-114">Application</span></span> | <span data-ttu-id="0660b-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0660b-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0660b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0660b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0660b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0660b-117">Request headers</span></span>
| <span data-ttu-id="0660b-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0660b-118">Header</span></span>       | <span data-ttu-id="0660b-119">Valor</span><span class="sxs-lookup"><span data-stu-id="0660b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0660b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0660b-120">Authorization</span></span>  | <span data-ttu-id="0660b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0660b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0660b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0660b-123">Content-Type</span></span>  | <span data-ttu-id="0660b-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0660b-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0660b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0660b-126">Request body</span></span>
<span data-ttu-id="0660b-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0660b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0660b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0660b-130">Property</span></span>     | <span data-ttu-id="0660b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0660b-131">Type</span></span>   |<span data-ttu-id="0660b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0660b-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0660b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0660b-133">displayName</span></span> | <span data-ttu-id="0660b-134">String</span><span class="sxs-lookup"><span data-stu-id="0660b-134">String</span></span> | <span data-ttu-id="0660b-135">O nome de exibição do [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="0660b-135">The display name of the [mailFolder](../resources/mailfolder.md).</span></span>|
| <span data-ttu-id="0660b-136">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="0660b-136">includeNestedFolders</span></span> | <span data-ttu-id="0660b-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="0660b-137">Boolean</span></span> | <span data-ttu-id="0660b-138">Como a hierarquia da pasta de caixa de correio deve ser percorrida.</span><span class="sxs-lookup"><span data-stu-id="0660b-138">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="0660b-139">`true`significa que uma pesquisa profunda deve ser feita enquanto `false` uma pesquisa superficial deve ser realizada.</span><span class="sxs-lookup"><span data-stu-id="0660b-139">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="0660b-140">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="0660b-140">sourceFolderIDs</span></span> | <span data-ttu-id="0660b-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0660b-141">String collection</span></span> | <span data-ttu-id="0660b-142">As pastas de caixa de correio que devem ser minadas.</span><span class="sxs-lookup"><span data-stu-id="0660b-142">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="0660b-143">filterQuery</span><span class="sxs-lookup"><span data-stu-id="0660b-143">filterQuery</span></span> | <span data-ttu-id="0660b-144">String</span><span class="sxs-lookup"><span data-stu-id="0660b-144">String</span></span> | <span data-ttu-id="0660b-145">A consulta OData para filtrar as mensagens.</span><span class="sxs-lookup"><span data-stu-id="0660b-145">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="0660b-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="0660b-146">Response</span></span>
<span data-ttu-id="0660b-147">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [mailFolder](../resources/mailfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0660b-147">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0660b-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0660b-148">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0660b-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0660b-149">Request</span></span>
<span data-ttu-id="0660b-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0660b-150">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailsearchfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "filterQuery": "contains(subject, 'Analytics')))"
}
```

#### <a name="response"></a><span data-ttu-id="0660b-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="0660b-151">Response</span></span>
<span data-ttu-id="0660b-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0660b-152">The following is an example of the response.</span></span>
><span data-ttu-id="0660b-153">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0660b-153">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0660b-154">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0660b-154">All the properties will be returned from an actual call.</span></span>
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
  "totalItemCount": 0,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": [
      "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'Analytics')"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailsearchfolder-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
