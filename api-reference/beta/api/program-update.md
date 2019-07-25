---
title: Programa de atualização
description: No recurso de revisões do Azure AD Access, atualize um objeto Program existente.
localization_priority: Normal
ms.openlocfilehash: b2918f59033d26372dd7ec8010c7ef2e90a65934
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875360"
---
# <a name="update-program"></a><span data-ttu-id="618b5-103">Programa de atualização</span><span class="sxs-lookup"><span data-stu-id="618b5-103">Update program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="618b5-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , atualize um objeto [Program](../resources/program.md) existente.</span><span class="sxs-lookup"><span data-stu-id="618b5-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="618b5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="618b5-105">Permissions</span></span>
<span data-ttu-id="618b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="618b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="618b5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="618b5-108">Permission type</span></span>                        | <span data-ttu-id="618b5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="618b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="618b5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="618b5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="618b5-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="618b5-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="618b5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="618b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="618b5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="618b5-113">Not supported.</span></span> |
|<span data-ttu-id="618b5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="618b5-114">Application</span></span>                            | <span data-ttu-id="618b5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="618b5-115">Not supported.</span></span> |

<span data-ttu-id="618b5-116">O usuário conectado também deve estar em uma função de diretório que permite a atualização de um programa.</span><span class="sxs-lookup"><span data-stu-id="618b5-116">The signed in user must also be in a directory role that permits them to update a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="618b5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="618b5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="618b5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="618b5-118">Request headers</span></span>
| <span data-ttu-id="618b5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="618b5-119">Name</span></span>         | <span data-ttu-id="618b5-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="618b5-120">Type</span></span>        | <span data-ttu-id="618b5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="618b5-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="618b5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="618b5-122">Authorization</span></span> | <span data-ttu-id="618b5-123">string</span><span class="sxs-lookup"><span data-stu-id="618b5-123">string</span></span> | <span data-ttu-id="618b5-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="618b5-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="618b5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="618b5-126">Request body</span></span>
<span data-ttu-id="618b5-127">No corpo da solicitação, forneça uma representação JSON de um objeto [Program](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="618b5-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="618b5-128">A tabela a seguir mostra as propriedades que podem ser fornecidas quando você atualiza um programa.</span><span class="sxs-lookup"><span data-stu-id="618b5-128">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="618b5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="618b5-129">Property</span></span>     | <span data-ttu-id="618b5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="618b5-130">Type</span></span>        | <span data-ttu-id="618b5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="618b5-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="618b5-132">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="618b5-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="618b5-133">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="618b5-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="618b5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="618b5-134">Response</span></span>
<span data-ttu-id="618b5-135">Se bem-sucedido, este método retorna um `204, Accepted` código de resposta e um objeto [Program](../resources/program.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="618b5-135">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="618b5-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="618b5-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="618b5-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="618b5-137">Request</span></span>
<span data-ttu-id="618b5-138">No corpo da solicitação, forneça uma representação JSON dos parâmetros do objeto [Program](../resources/program.md) a ser alterado.</span><span class="sxs-lookup"><span data-stu-id="618b5-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="618b5-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="618b5-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="618b5-140">C#</span><span class="sxs-lookup"><span data-stu-id="618b5-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="618b5-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="618b5-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="618b5-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="618b5-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="618b5-143">Java</span><span class="sxs-lookup"><span data-stu-id="618b5-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-program-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="618b5-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="618b5-144">Response</span></span>
><span data-ttu-id="618b5-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="618b5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="618b5-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="618b5-147">See also</span></span>

| <span data-ttu-id="618b5-148">Método</span><span class="sxs-lookup"><span data-stu-id="618b5-148">Method</span></span>           | <span data-ttu-id="618b5-149">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="618b5-149">Return Type</span></span>    |<span data-ttu-id="618b5-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="618b5-150">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="618b5-151">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="618b5-151">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="618b5-152">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="618b5-152">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="618b5-153">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="618b5-153">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="618b5-154">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="618b5-154">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="618b5-155">programControl</span><span class="sxs-lookup"><span data-stu-id="618b5-155">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="618b5-156">Adicionar um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="618b5-156">Add a programControl to a program.</span></span>|

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
