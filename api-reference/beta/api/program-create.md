---
title: Criar programa
description: No recurso de revisões do Azure AD Access, crie um novo objeto de programa.
localization_priority: Normal
ms.openlocfilehash: fba14e8c16afae7f1b5160ff1709d678193766ec
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455326"
---
# <a name="create-program"></a><span data-ttu-id="cfb4e-103">Criar programa</span><span class="sxs-lookup"><span data-stu-id="cfb4e-103">Create program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfb4e-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , crie um novo objeto de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="cfb4e-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cfb4e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cfb4e-105">Permissions</span></span>
<span data-ttu-id="cfb4e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfb4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfb4e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cfb4e-108">Permission type</span></span>                        | <span data-ttu-id="cfb4e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cfb4e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfb4e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cfb4e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cfb4e-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfb4e-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="cfb4e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cfb4e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfb4e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfb4e-113">Not supported.</span></span> |
|<span data-ttu-id="cfb4e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cfb4e-114">Application</span></span>                            | <span data-ttu-id="cfb4e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfb4e-115">Not supported.</span></span> |

<span data-ttu-id="cfb4e-116">O usuário conectado também deve estar em uma função de diretório que permite que eles criem um programa.</span><span class="sxs-lookup"><span data-stu-id="cfb4e-116">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="cfb4e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cfb4e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="cfb4e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cfb4e-118">Request headers</span></span>
| <span data-ttu-id="cfb4e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cfb4e-119">Name</span></span>         | <span data-ttu-id="cfb4e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfb4e-120">Type</span></span>        | <span data-ttu-id="cfb4e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfb4e-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="cfb4e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cfb4e-122">Authorization</span></span> | <span data-ttu-id="cfb4e-123">string</span><span class="sxs-lookup"><span data-stu-id="cfb4e-123">string</span></span> | <span data-ttu-id="cfb4e-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfb4e-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfb4e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cfb4e-126">Request body</span></span>
<span data-ttu-id="cfb4e-127">No corpo da solicitação, forneça uma representação JSON de um objeto [Program](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="cfb4e-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="cfb4e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar um programa.</span><span class="sxs-lookup"><span data-stu-id="cfb4e-128">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="cfb4e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfb4e-129">Property</span></span>     | <span data-ttu-id="cfb4e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfb4e-130">Type</span></span>        | <span data-ttu-id="cfb4e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfb4e-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="cfb4e-132">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="cfb4e-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="cfb4e-133">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="cfb4e-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="cfb4e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfb4e-134">Response</span></span>
<span data-ttu-id="cfb4e-135">Se bem-sucedido, este método retorna um `201, Created` código de resposta e um objeto [Program](../resources/program.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cfb4e-135">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfb4e-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cfb4e-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cfb4e-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfb4e-137">Request</span></span>
<span data-ttu-id="cfb4e-138">No corpo da solicitação, forneça uma representação JSON do objeto [Program](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="cfb4e-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cfb4e-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfb4e-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="cfb4e-140">C#</span><span class="sxs-lookup"><span data-stu-id="cfb4e-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-program-from-programs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cfb4e-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="cfb4e-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-program-from-programs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cfb4e-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="cfb4e-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-program-from-programs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cfb4e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfb4e-143">Response</span></span>
><span data-ttu-id="cfb4e-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cfb4e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="cfb4e-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="cfb4e-146">See also</span></span>

| <span data-ttu-id="cfb4e-147">Método</span><span class="sxs-lookup"><span data-stu-id="cfb4e-147">Method</span></span>           | <span data-ttu-id="cfb4e-148">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cfb4e-148">Return Type</span></span>    |<span data-ttu-id="cfb4e-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfb4e-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cfb4e-150">Listar programas</span><span class="sxs-lookup"><span data-stu-id="cfb4e-150">List programs</span></span>](program-list.md) | <span data-ttu-id="cfb4e-151">coleção [Program](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="cfb4e-151">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="cfb4e-152">Obtenha uma coleção de todos os programas.</span><span class="sxs-lookup"><span data-stu-id="cfb4e-152">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="cfb4e-153">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="cfb4e-153">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="cfb4e-154">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="cfb4e-154">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="cfb4e-155">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="cfb4e-155">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="cfb4e-156">Programa de atualização</span><span class="sxs-lookup"><span data-stu-id="cfb4e-156">Update program</span></span>](program-update.md) |  [<span data-ttu-id="cfb4e-157">programa</span><span class="sxs-lookup"><span data-stu-id="cfb4e-157">program</span></span>](../resources/program.md)| <span data-ttu-id="cfb4e-158">Atualizar um programa.</span><span class="sxs-lookup"><span data-stu-id="cfb4e-158">Update a program.</span></span>|
|[<span data-ttu-id="cfb4e-159">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="cfb4e-159">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="cfb4e-160">programControl</span><span class="sxs-lookup"><span data-stu-id="cfb4e-160">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="cfb4e-161">Adicionar um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="cfb4e-161">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
