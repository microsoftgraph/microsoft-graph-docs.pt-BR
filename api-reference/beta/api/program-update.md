---
title: Programa de atualização
description: No recurso de revisões do Azure AD Access, atualize um objeto Program existente.
localization_priority: Normal
ms.openlocfilehash: bc4971dd825b031d786d50aeffe3a96eb5a7ef80
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264096"
---
# <a name="update-program"></a><span data-ttu-id="b1e93-103">Programa de atualização</span><span class="sxs-lookup"><span data-stu-id="b1e93-103">Update program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1e93-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , atualize um objeto [Program](../resources/program.md) existente.</span><span class="sxs-lookup"><span data-stu-id="b1e93-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b1e93-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1e93-105">Permissions</span></span>
<span data-ttu-id="b1e93-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1e93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1e93-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1e93-108">Permission type</span></span>                        | <span data-ttu-id="b1e93-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1e93-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1e93-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1e93-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b1e93-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1e93-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="b1e93-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1e93-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1e93-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1e93-113">Not supported.</span></span> |
|<span data-ttu-id="b1e93-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1e93-114">Application</span></span>                            | <span data-ttu-id="b1e93-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1e93-115">Not supported.</span></span> |

<span data-ttu-id="b1e93-116">O usuário conectado também deve estar em uma função de diretório que permite a atualização de um programa.</span><span class="sxs-lookup"><span data-stu-id="b1e93-116">The signed in user must also be in a directory role that permits them to update a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="b1e93-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1e93-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="b1e93-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1e93-118">Request headers</span></span>
| <span data-ttu-id="b1e93-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b1e93-119">Name</span></span>         | <span data-ttu-id="b1e93-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1e93-120">Type</span></span>        | <span data-ttu-id="b1e93-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1e93-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b1e93-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1e93-122">Authorization</span></span> | <span data-ttu-id="b1e93-123">string</span><span class="sxs-lookup"><span data-stu-id="b1e93-123">string</span></span> | <span data-ttu-id="b1e93-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1e93-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1e93-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1e93-126">Request body</span></span>
<span data-ttu-id="b1e93-127">No corpo da solicitação, forneça uma representação JSON de um objeto [Program](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="b1e93-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="b1e93-128">A tabela a seguir mostra as propriedades que podem ser fornecidas quando você atualiza um programa.</span><span class="sxs-lookup"><span data-stu-id="b1e93-128">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="b1e93-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1e93-129">Property</span></span>     | <span data-ttu-id="b1e93-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1e93-130">Type</span></span>        | <span data-ttu-id="b1e93-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1e93-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="b1e93-132">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="b1e93-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="b1e93-133">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="b1e93-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="b1e93-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1e93-134">Response</span></span>
<span data-ttu-id="b1e93-135">Se bem-sucedido, este método retorna um `204, Accepted` código de resposta e um objeto [Program](../resources/program.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1e93-135">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1e93-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1e93-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1e93-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1e93-137">Request</span></span>
<span data-ttu-id="b1e93-138">No corpo da solicitação, forneça uma representação JSON dos parâmetros do objeto [Program](../resources/program.md) a ser alterado.</span><span class="sxs-lookup"><span data-stu-id="b1e93-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_program"
}-->
```http
PATCH https://graph.microsoft.com/beta/programs/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
Content-type: application/json

{
    "displayName": "testprogram3 new name"
}
```

##### <a name="response"></a><span data-ttu-id="b1e93-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1e93-139">Response</span></span>
><span data-ttu-id="b1e93-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1e93-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
} -->
```http
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3 new name",
    "description": "test description"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b1e93-142">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="b1e93-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b1e93-143">C#</span><span class="sxs-lookup"><span data-stu-id="b1e93-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_program-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1e93-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="b1e93-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_program-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b1e93-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b1e93-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_program-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="b1e93-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="b1e93-146">See also</span></span>

| <span data-ttu-id="b1e93-147">Método</span><span class="sxs-lookup"><span data-stu-id="b1e93-147">Method</span></span>           | <span data-ttu-id="b1e93-148">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b1e93-148">Return Type</span></span>    |<span data-ttu-id="b1e93-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1e93-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b1e93-150">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="b1e93-150">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="b1e93-151">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="b1e93-151">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="b1e93-152">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="b1e93-152">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="b1e93-153">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="b1e93-153">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="b1e93-154">programControl</span><span class="sxs-lookup"><span data-stu-id="b1e93-154">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="b1e93-155">Adicionar um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="b1e93-155">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/program-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/program-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
