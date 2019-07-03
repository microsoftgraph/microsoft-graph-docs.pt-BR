---
title: Atualizar contrato
description: Atualizar as propriedades de um objeto de contrato.
localization_priority: Normal
ms.openlocfilehash: 5627afe60cd0db197a54af8038c6f06a065b59bb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439781"
---
# <a name="update-agreement"></a><span data-ttu-id="b6a3f-103">Atualizar contrato</span><span class="sxs-lookup"><span data-stu-id="b6a3f-103">Update agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6a3f-104">Atualizar as propriedades de um objeto de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="b6a3f-104">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b6a3f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6a3f-105">Permissions</span></span>
<span data-ttu-id="b6a3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6a3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6a3f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6a3f-108">Permission type</span></span>                        | <span data-ttu-id="b6a3f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6a3f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6a3f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6a3f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b6a3f-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6a3f-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="b6a3f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6a3f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6a3f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6a3f-113">Not supported.</span></span> |
|<span data-ttu-id="b6a3f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6a3f-114">Application</span></span>                            | <span data-ttu-id="b6a3f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6a3f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6a3f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6a3f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="b6a3f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6a3f-117">Request headers</span></span>
| <span data-ttu-id="b6a3f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b6a3f-118">Name</span></span>         | <span data-ttu-id="b6a3f-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6a3f-119">Type</span></span>        | <span data-ttu-id="b6a3f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6a3f-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b6a3f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6a3f-121">Authorization</span></span> | <span data-ttu-id="b6a3f-122">string</span><span class="sxs-lookup"><span data-stu-id="b6a3f-122">string</span></span> | <span data-ttu-id="b6a3f-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6a3f-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6a3f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6a3f-125">Request body</span></span>
<span data-ttu-id="b6a3f-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="b6a3f-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b6a3f-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="b6a3f-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b6a3f-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b6a3f-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b6a3f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6a3f-129">Property</span></span>     | <span data-ttu-id="b6a3f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6a3f-130">Type</span></span>        | <span data-ttu-id="b6a3f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6a3f-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b6a3f-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b6a3f-132">displayName</span></span>|<span data-ttu-id="b6a3f-133">String</span><span class="sxs-lookup"><span data-stu-id="b6a3f-133">String</span></span>|<span data-ttu-id="b6a3f-134">Nome para exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="b6a3f-134">Display name of the agreement.</span></span>|
|<span data-ttu-id="b6a3f-135">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="b6a3f-135">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="b6a3f-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6a3f-136">Boolean</span></span>|<span data-ttu-id="b6a3f-137">Se o usuário tem que expandir e exibir o contrato antes de aceitar o.</span><span class="sxs-lookup"><span data-stu-id="b6a3f-137">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="b6a3f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6a3f-138">Response</span></span>
<span data-ttu-id="b6a3f-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Agreement](../resources/agreement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6a3f-139">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b6a3f-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6a3f-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6a3f-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6a3f-141">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b6a3f-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6a3f-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b6a3f-143">C#</span><span class="sxs-lookup"><span data-stu-id="b6a3f-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b6a3f-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="b6a3f-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b6a3f-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b6a3f-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b6a3f-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6a3f-146">Response</span></span>
><span data-ttu-id="b6a3f-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6a3f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}
-->
