---
title: Criar programa
description: No recurso de revisões do Azure AD Access, crie um novo objeto de programa.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: f48cb663a28bc5c82c4c1a78877d19ebd72364e9
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412548"
---
# <a name="create-program"></a><span data-ttu-id="4be95-103">Criar programa</span><span class="sxs-lookup"><span data-stu-id="4be95-103">Create program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4be95-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , crie um novo objeto de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="4be95-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4be95-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4be95-105">Permissions</span></span>
<span data-ttu-id="4be95-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4be95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4be95-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4be95-108">Permission type</span></span>                        | <span data-ttu-id="4be95-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4be95-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4be95-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4be95-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4be95-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4be95-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="4be95-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4be95-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4be95-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4be95-113">Not supported.</span></span> |
|<span data-ttu-id="4be95-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4be95-114">Application</span></span>                            | <span data-ttu-id="4be95-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4be95-115">Not supported.</span></span> |

<span data-ttu-id="4be95-116">O usuário conectado também deve estar em uma função de diretório que permite que eles criem um programa.</span><span class="sxs-lookup"><span data-stu-id="4be95-116">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="4be95-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4be95-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="4be95-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4be95-118">Request headers</span></span>
| <span data-ttu-id="4be95-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4be95-119">Name</span></span>         | <span data-ttu-id="4be95-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="4be95-120">Type</span></span>        | <span data-ttu-id="4be95-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4be95-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4be95-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4be95-122">Authorization</span></span> | <span data-ttu-id="4be95-123">string</span><span class="sxs-lookup"><span data-stu-id="4be95-123">string</span></span> | <span data-ttu-id="4be95-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4be95-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4be95-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4be95-126">Request body</span></span>
<span data-ttu-id="4be95-127">No corpo da solicitação, forneça uma representação JSON de um objeto [Program](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="4be95-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="4be95-128">A tabela a seguir mostra as propriedades que são necessárias ao criar um programa.</span><span class="sxs-lookup"><span data-stu-id="4be95-128">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="4be95-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4be95-129">Property</span></span>     | <span data-ttu-id="4be95-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4be95-130">Type</span></span>        | <span data-ttu-id="4be95-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4be95-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="4be95-132">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="4be95-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="4be95-133">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="4be95-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="4be95-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4be95-134">Response</span></span>
<span data-ttu-id="4be95-135">Se bem-sucedido, este método retorna um `201, Created` código de resposta e um objeto [Program](../resources/program.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4be95-135">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4be95-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4be95-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4be95-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4be95-137">Request</span></span>
<span data-ttu-id="4be95-138">No corpo da solicitação, forneça uma representação JSON do objeto [Program](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="4be95-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4be95-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="4be95-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4be95-140">C#</span><span class="sxs-lookup"><span data-stu-id="4be95-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-program-from-programs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4be95-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4be95-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-program-from-programs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4be95-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4be95-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-program-from-programs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4be95-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="4be95-143">Response</span></span>
><span data-ttu-id="4be95-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4be95-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="4be95-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="4be95-146">See also</span></span>

| <span data-ttu-id="4be95-147">Método</span><span class="sxs-lookup"><span data-stu-id="4be95-147">Method</span></span>           | <span data-ttu-id="4be95-148">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4be95-148">Return Type</span></span>    |<span data-ttu-id="4be95-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="4be95-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4be95-150">Listar programas</span><span class="sxs-lookup"><span data-stu-id="4be95-150">List programs</span></span>](program-list.md) | <span data-ttu-id="4be95-151">coleção [Program](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="4be95-151">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="4be95-152">Obtenha uma coleção de todos os programas.</span><span class="sxs-lookup"><span data-stu-id="4be95-152">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="4be95-153">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="4be95-153">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="4be95-154">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="4be95-154">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="4be95-155">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="4be95-155">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="4be95-156">Programa de atualização</span><span class="sxs-lookup"><span data-stu-id="4be95-156">Update program</span></span>](program-update.md) |  [<span data-ttu-id="4be95-157">programa</span><span class="sxs-lookup"><span data-stu-id="4be95-157">program</span></span>](../resources/program.md)| <span data-ttu-id="4be95-158">Atualizar um programa.</span><span class="sxs-lookup"><span data-stu-id="4be95-158">Update a program.</span></span>|
|[<span data-ttu-id="4be95-159">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="4be95-159">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="4be95-160">programControl</span><span class="sxs-lookup"><span data-stu-id="4be95-160">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="4be95-161">Adicionar um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="4be95-161">Add a programControl to a program.</span></span>|

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
