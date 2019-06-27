---
title: Criar programa
description: No recurso de revisões do Azure AD Access, crie um novo objeto de programa.
localization_priority: Normal
ms.openlocfilehash: 0d2218031e924e7137378a63d932f5533620cc38
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267659"
---
# <a name="create-program"></a><span data-ttu-id="7f455-103">Criar programa</span><span class="sxs-lookup"><span data-stu-id="7f455-103">Create program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f455-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , crie um novo objeto de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="7f455-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7f455-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f455-105">Permissions</span></span>
<span data-ttu-id="7f455-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f455-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f455-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f455-108">Permission type</span></span>                        | <span data-ttu-id="7f455-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f455-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f455-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f455-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f455-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f455-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="7f455-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f455-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f455-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f455-113">Not supported.</span></span> |
|<span data-ttu-id="7f455-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f455-114">Application</span></span>                            | <span data-ttu-id="7f455-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f455-115">Not supported.</span></span> |

<span data-ttu-id="7f455-116">O usuário conectado também deve estar em uma função de diretório que permite que eles criem um programa.</span><span class="sxs-lookup"><span data-stu-id="7f455-116">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="7f455-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f455-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="7f455-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f455-118">Request headers</span></span>
| <span data-ttu-id="7f455-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7f455-119">Name</span></span>         | <span data-ttu-id="7f455-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f455-120">Type</span></span>        | <span data-ttu-id="7f455-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f455-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7f455-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f455-122">Authorization</span></span> | <span data-ttu-id="7f455-123">string</span><span class="sxs-lookup"><span data-stu-id="7f455-123">string</span></span> | <span data-ttu-id="7f455-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f455-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f455-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f455-126">Request body</span></span>
<span data-ttu-id="7f455-127">No corpo da solicitação, forneça uma representação JSON de um objeto [Program](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="7f455-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="7f455-128">A tabela a seguir mostra as propriedades que são necessárias ao criar um programa.</span><span class="sxs-lookup"><span data-stu-id="7f455-128">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="7f455-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f455-129">Property</span></span>     | <span data-ttu-id="7f455-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f455-130">Type</span></span>        | <span data-ttu-id="7f455-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f455-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="7f455-132">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="7f455-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="7f455-133">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="7f455-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="7f455-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f455-134">Response</span></span>
<span data-ttu-id="7f455-135">Se bem-sucedido, este método retorna um `201, Created` código de resposta e um objeto [Program](../resources/program.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f455-135">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f455-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f455-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f455-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f455-137">Request</span></span>
<span data-ttu-id="7f455-138">No corpo da solicitação, forneça uma representação JSON do objeto [Program](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="7f455-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_program_from_programs"
}-->
```http
POST https://graph.microsoft.com/beta/programs
Content-type: application/json

{
    "displayName": "testprogram3",
    "description": "test description"
}
```

##### <a name="response"></a><span data-ttu-id="7f455-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f455-139">Response</span></span>
><span data-ttu-id="7f455-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f455-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3",
    "description": "test description"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7f455-142">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="7f455-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7f455-143">C#</span><span class="sxs-lookup"><span data-stu-id="7f455-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_program_from_programs-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7f455-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="7f455-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_program_from_programs-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7f455-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7f455-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_program_from_programs-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="7f455-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="7f455-146">See also</span></span>

| <span data-ttu-id="7f455-147">Método</span><span class="sxs-lookup"><span data-stu-id="7f455-147">Method</span></span>           | <span data-ttu-id="7f455-148">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7f455-148">Return Type</span></span>    |<span data-ttu-id="7f455-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f455-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7f455-150">Listar programas</span><span class="sxs-lookup"><span data-stu-id="7f455-150">List programs</span></span>](program-list.md) | <span data-ttu-id="7f455-151">coleção [Program](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="7f455-151">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="7f455-152">Obtenha uma coleção de todos os programas.</span><span class="sxs-lookup"><span data-stu-id="7f455-152">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="7f455-153">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="7f455-153">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="7f455-154">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="7f455-154">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="7f455-155">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="7f455-155">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="7f455-156">Programa de atualização</span><span class="sxs-lookup"><span data-stu-id="7f455-156">Update program</span></span>](program-update.md) |  [<span data-ttu-id="7f455-157">programa</span><span class="sxs-lookup"><span data-stu-id="7f455-157">program</span></span>](../resources/program.md)| <span data-ttu-id="7f455-158">Atualizar um programa.</span><span class="sxs-lookup"><span data-stu-id="7f455-158">Update a program.</span></span>|
|[<span data-ttu-id="7f455-159">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="7f455-159">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="7f455-160">programControl</span><span class="sxs-lookup"><span data-stu-id="7f455-160">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="7f455-161">Adicionar um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="7f455-161">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-create.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/program-create.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/program-create.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
