---
title: Programa de atualização
description: No recurso de revisões do Azure AD Access, atualize um objeto Program existente.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: c1f50f81d4c87283ce686da5626b5482055ec5fd
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412492"
---
# <a name="update-program"></a><span data-ttu-id="20e1b-103">Programa de atualização</span><span class="sxs-lookup"><span data-stu-id="20e1b-103">Update program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20e1b-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , atualize um objeto [Program](../resources/program.md) existente.</span><span class="sxs-lookup"><span data-stu-id="20e1b-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="20e1b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="20e1b-105">Permissions</span></span>
<span data-ttu-id="20e1b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20e1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20e1b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20e1b-108">Permission type</span></span>                        | <span data-ttu-id="20e1b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20e1b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="20e1b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20e1b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="20e1b-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20e1b-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="20e1b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20e1b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20e1b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20e1b-113">Not supported.</span></span> |
|<span data-ttu-id="20e1b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20e1b-114">Application</span></span>                            | <span data-ttu-id="20e1b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20e1b-115">Not supported.</span></span> |

<span data-ttu-id="20e1b-116">O usuário conectado também deve estar em uma função de diretório que permite a atualização de um programa.</span><span class="sxs-lookup"><span data-stu-id="20e1b-116">The signed in user must also be in a directory role that permits them to update a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="20e1b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20e1b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="20e1b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20e1b-118">Request headers</span></span>
| <span data-ttu-id="20e1b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="20e1b-119">Name</span></span>         | <span data-ttu-id="20e1b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="20e1b-120">Type</span></span>        | <span data-ttu-id="20e1b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="20e1b-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="20e1b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="20e1b-122">Authorization</span></span> | <span data-ttu-id="20e1b-123">string</span><span class="sxs-lookup"><span data-stu-id="20e1b-123">string</span></span> | <span data-ttu-id="20e1b-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20e1b-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20e1b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20e1b-126">Request body</span></span>
<span data-ttu-id="20e1b-127">No corpo da solicitação, forneça uma representação JSON de um objeto [Program](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="20e1b-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="20e1b-128">A tabela a seguir mostra as propriedades que podem ser fornecidas quando você atualiza um programa.</span><span class="sxs-lookup"><span data-stu-id="20e1b-128">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="20e1b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20e1b-129">Property</span></span>     | <span data-ttu-id="20e1b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="20e1b-130">Type</span></span>        | <span data-ttu-id="20e1b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="20e1b-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="20e1b-132">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="20e1b-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="20e1b-133">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="20e1b-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="20e1b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="20e1b-134">Response</span></span>
<span data-ttu-id="20e1b-135">Se bem-sucedido, este método retorna um `204, Accepted` código de resposta e um objeto [Program](../resources/program.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20e1b-135">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20e1b-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20e1b-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20e1b-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20e1b-137">Request</span></span>
<span data-ttu-id="20e1b-138">No corpo da solicitação, forneça uma representação JSON dos parâmetros do objeto [Program](../resources/program.md) a ser alterado.</span><span class="sxs-lookup"><span data-stu-id="20e1b-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="20e1b-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="20e1b-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="20e1b-140">C#</span><span class="sxs-lookup"><span data-stu-id="20e1b-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20e1b-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20e1b-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="20e1b-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="20e1b-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="20e1b-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="20e1b-143">Response</span></span>
><span data-ttu-id="20e1b-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20e1b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="20e1b-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="20e1b-146">See also</span></span>

| <span data-ttu-id="20e1b-147">Método</span><span class="sxs-lookup"><span data-stu-id="20e1b-147">Method</span></span>           | <span data-ttu-id="20e1b-148">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="20e1b-148">Return Type</span></span>    |<span data-ttu-id="20e1b-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="20e1b-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="20e1b-150">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="20e1b-150">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="20e1b-151">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="20e1b-151">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="20e1b-152">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="20e1b-152">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="20e1b-153">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="20e1b-153">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="20e1b-154">programControl</span><span class="sxs-lookup"><span data-stu-id="20e1b-154">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="20e1b-155">Adicionar um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="20e1b-155">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
