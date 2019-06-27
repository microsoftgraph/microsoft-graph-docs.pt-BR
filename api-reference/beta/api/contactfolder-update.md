---
title: Atualizar contactfolder
description: Atualiza as propriedades do objeto contactfolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a01cc70222205bcafd5cd892561b1ca831f51a59
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261233"
---
# <a name="update-contactfolder"></a><span data-ttu-id="480f0-103">Atualizar contactfolder</span><span class="sxs-lookup"><span data-stu-id="480f0-103">Update contactfolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="480f0-104">Atualiza as propriedades do objeto contactfolder.</span><span class="sxs-lookup"><span data-stu-id="480f0-104">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="480f0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="480f0-105">Permissions</span></span>
<span data-ttu-id="480f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="480f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="480f0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="480f0-108">Permission type</span></span>      | <span data-ttu-id="480f0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="480f0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="480f0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="480f0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="480f0-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="480f0-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="480f0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="480f0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="480f0-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="480f0-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="480f0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="480f0-114">Application</span></span> | <span data-ttu-id="480f0-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="480f0-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="480f0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="480f0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="480f0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="480f0-117">Request headers</span></span>
| <span data-ttu-id="480f0-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="480f0-118">Header</span></span>       | <span data-ttu-id="480f0-119">Valor</span><span class="sxs-lookup"><span data-stu-id="480f0-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="480f0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="480f0-120">Authorization</span></span>  | <span data-ttu-id="480f0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="480f0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="480f0-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="480f0-123">Content-Type</span></span>  | <span data-ttu-id="480f0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="480f0-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="480f0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="480f0-126">Request body</span></span>
<span data-ttu-id="480f0-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="480f0-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="480f0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="480f0-130">Property</span></span>     | <span data-ttu-id="480f0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="480f0-131">Type</span></span>   |<span data-ttu-id="480f0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="480f0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="480f0-133">displayName</span><span class="sxs-lookup"><span data-stu-id="480f0-133">displayName</span></span>|<span data-ttu-id="480f0-134">String</span><span class="sxs-lookup"><span data-stu-id="480f0-134">String</span></span>|<span data-ttu-id="480f0-135">O nome de exibição da pasta.</span><span class="sxs-lookup"><span data-stu-id="480f0-135">The folder's display name.</span></span>|
|<span data-ttu-id="480f0-136">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="480f0-136">parentFolderId</span></span>|<span data-ttu-id="480f0-137">String</span><span class="sxs-lookup"><span data-stu-id="480f0-137">String</span></span>|<span data-ttu-id="480f0-138">A ID da pasta pai da pasta.</span><span class="sxs-lookup"><span data-stu-id="480f0-138">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="480f0-139">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="480f0-139">wellKnownName</span></span>|<span data-ttu-id="480f0-140">string</span><span class="sxs-lookup"><span data-stu-id="480f0-140">string</span></span>|<span data-ttu-id="480f0-141">O nome da pasta se a pasta for uma pasta reconhecida.</span><span class="sxs-lookup"><span data-stu-id="480f0-141">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="480f0-142">Atualmente `contacts` é a única pasta de contatos reconhecida.</span><span class="sxs-lookup"><span data-stu-id="480f0-142">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="response"></a><span data-ttu-id="480f0-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="480f0-143">Response</span></span>

<span data-ttu-id="480f0-144">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [contactFolder](../resources/contactfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="480f0-144">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="480f0-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="480f0-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="480f0-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="480f0-146">Request</span></span>
<span data-ttu-id="480f0-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="480f0-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="480f0-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="480f0-148">Response</span></span>
<span data-ttu-id="480f0-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="480f0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "wellKnownName": "wellKnownName-value",
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="480f0-152">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="480f0-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="480f0-153">C#</span><span class="sxs-lookup"><span data-stu-id="480f0-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_contactfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="480f0-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="480f0-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_contactfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="480f0-155">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="480f0-155">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_contactfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update contactfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contactfolder-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/contactfolder-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/contactfolder-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
