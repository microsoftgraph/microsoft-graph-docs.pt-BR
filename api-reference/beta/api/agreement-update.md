---
title: Atualizar contrato
description: Atualizar as propriedades de um objeto de contrato.
localization_priority: Normal
ms.openlocfilehash: 6dacf9bfbfdf3cf85a673c68555b8deb3aeab1c7
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636615"
---
# <a name="update-agreement"></a><span data-ttu-id="16387-103">Atualizar contrato</span><span class="sxs-lookup"><span data-stu-id="16387-103">Update agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16387-104">Atualizar as propriedades de um objeto de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="16387-104">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="16387-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="16387-105">Permissions</span></span>
<span data-ttu-id="16387-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16387-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16387-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16387-108">Permission type</span></span>                        | <span data-ttu-id="16387-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16387-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="16387-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16387-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="16387-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16387-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="16387-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16387-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16387-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16387-113">Not supported.</span></span> |
|<span data-ttu-id="16387-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16387-114">Application</span></span>                            | <span data-ttu-id="16387-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16387-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16387-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16387-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="16387-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16387-117">Request headers</span></span>
| <span data-ttu-id="16387-118">Nome</span><span class="sxs-lookup"><span data-stu-id="16387-118">Name</span></span>         | <span data-ttu-id="16387-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="16387-119">Type</span></span>        | <span data-ttu-id="16387-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="16387-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="16387-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="16387-121">Authorization</span></span> | <span data-ttu-id="16387-122">string</span><span class="sxs-lookup"><span data-stu-id="16387-122">string</span></span> | <span data-ttu-id="16387-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16387-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16387-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16387-125">Request body</span></span>
<span data-ttu-id="16387-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="16387-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="16387-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="16387-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="16387-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="16387-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="16387-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16387-129">Property</span></span>     | <span data-ttu-id="16387-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="16387-130">Type</span></span>        | <span data-ttu-id="16387-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="16387-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="16387-132">displayName</span><span class="sxs-lookup"><span data-stu-id="16387-132">displayName</span></span>|<span data-ttu-id="16387-133">String</span><span class="sxs-lookup"><span data-stu-id="16387-133">String</span></span>|<span data-ttu-id="16387-134">Nome para exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="16387-134">Display name of the agreement.</span></span>|
|<span data-ttu-id="16387-135">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="16387-135">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="16387-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="16387-136">Boolean</span></span>|<span data-ttu-id="16387-137">Se o usuário tem que expandir e exibir o contrato antes de aceitar o.</span><span class="sxs-lookup"><span data-stu-id="16387-137">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="16387-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="16387-138">Response</span></span>
<span data-ttu-id="16387-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Agreement](../resources/agreement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16387-139">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="16387-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16387-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="16387-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16387-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_agreement"
}-->
```http
PATCH https://graph.microsoft.com/beta/agreements/<id>
Content-type: application/json
Content-length: 85

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true
}
```
##### <a name="response"></a><span data-ttu-id="16387-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="16387-142">Response</span></span>
><span data-ttu-id="16387-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16387-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 105

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="16387-145">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="16387-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="16387-146">Basic</span><span class="sxs-lookup"><span data-stu-id="16387-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_agreement-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="16387-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16387-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_agreement-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/agreement-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
