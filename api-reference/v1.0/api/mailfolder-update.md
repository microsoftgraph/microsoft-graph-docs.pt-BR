---
title: Atualizar mailfolder
description: Atualize as propriedades do objeto mailfolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: daa089d51af768e8ab07b6cedb0c88e0030ab435
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612507"
---
# <a name="update-mailfolder"></a><span data-ttu-id="47fee-103">Atualizar mailfolder</span><span class="sxs-lookup"><span data-stu-id="47fee-103">Update mailfolder</span></span>

<span data-ttu-id="47fee-104">Atualize as propriedades do objeto mailfolder.</span><span class="sxs-lookup"><span data-stu-id="47fee-104">Update the properties of mailfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="47fee-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="47fee-105">Permissions</span></span>
<span data-ttu-id="47fee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47fee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47fee-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47fee-108">Permission type</span></span>      | <span data-ttu-id="47fee-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47fee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47fee-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47fee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="47fee-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47fee-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="47fee-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47fee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47fee-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47fee-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="47fee-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47fee-114">Application</span></span> | <span data-ttu-id="47fee-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47fee-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="47fee-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47fee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="47fee-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47fee-117">Request headers</span></span>
| <span data-ttu-id="47fee-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="47fee-118">Header</span></span>       | <span data-ttu-id="47fee-119">Valor</span><span class="sxs-lookup"><span data-stu-id="47fee-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="47fee-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="47fee-120">Authorization</span></span>  | <span data-ttu-id="47fee-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47fee-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="47fee-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="47fee-123">Content-Type</span></span>  | <span data-ttu-id="47fee-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47fee-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="47fee-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47fee-126">Request body</span></span>
<span data-ttu-id="47fee-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="47fee-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="47fee-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47fee-130">Property</span></span>     | <span data-ttu-id="47fee-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="47fee-131">Type</span></span>   |<span data-ttu-id="47fee-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="47fee-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47fee-133">displayName</span><span class="sxs-lookup"><span data-stu-id="47fee-133">displayName</span></span>|<span data-ttu-id="47fee-134">String</span><span class="sxs-lookup"><span data-stu-id="47fee-134">String</span></span>|<span data-ttu-id="47fee-135">O nome de exibição da mailFolder.</span><span class="sxs-lookup"><span data-stu-id="47fee-135">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="47fee-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="47fee-136">Response</span></span>

<span data-ttu-id="47fee-137">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [mailFolder](../resources/mailfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47fee-137">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="47fee-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47fee-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47fee-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47fee-139">Request</span></span>
<span data-ttu-id="47fee-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47fee-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailFolders/{id}
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
##### <a name="response"></a><span data-ttu-id="47fee-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="47fee-141">Response</span></span>
<span data-ttu-id="47fee-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47fee-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="47fee-145">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="47fee-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="47fee-146">Basic</span><span class="sxs-lookup"><span data-stu-id="47fee-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="47fee-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47fee-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_mailfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/mailfolder-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/mailfolder-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
