---
title: Atualizar programa
description: No recurso de revisões de acesso do Azure AD, atualize um objeto de programa existente.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 29b30bd80dba96b061d0c83f2710d224c3da8758
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721773"
---
# <a name="update-program"></a><span data-ttu-id="e6a40-103">Atualizar programa</span><span class="sxs-lookup"><span data-stu-id="e6a40-103">Update program</span></span>

<span data-ttu-id="e6a40-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6a40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6a40-105">No recurso de [revisões](../resources/accessreviews-root.md) de acesso do Azure AD, atualize um objeto [de programa](../resources/program.md) existente.</span><span class="sxs-lookup"><span data-stu-id="e6a40-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e6a40-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6a40-106">Permissions</span></span>
<span data-ttu-id="e6a40-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6a40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6a40-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6a40-109">Permission type</span></span>                        | <span data-ttu-id="e6a40-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6a40-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6a40-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6a40-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6a40-112">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6a40-112">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="e6a40-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6a40-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6a40-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6a40-114">Not supported.</span></span> |
|<span data-ttu-id="e6a40-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6a40-115">Application</span></span>                            | <span data-ttu-id="e6a40-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6a40-116">Not supported.</span></span> |

<span data-ttu-id="e6a40-117">O usuário inscreveu também deve estar em uma função de diretório que permita que ele atualize um programa.</span><span class="sxs-lookup"><span data-stu-id="e6a40-117">The signed in user must also be in a directory role that permits them to update a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="e6a40-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6a40-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs/{programId}
```
## <a name="request-headers"></a><span data-ttu-id="e6a40-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6a40-119">Request headers</span></span>
| <span data-ttu-id="e6a40-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e6a40-120">Name</span></span>         | <span data-ttu-id="e6a40-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6a40-121">Type</span></span>        | <span data-ttu-id="e6a40-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6a40-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e6a40-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6a40-123">Authorization</span></span> | <span data-ttu-id="e6a40-124">string</span><span class="sxs-lookup"><span data-stu-id="e6a40-124">string</span></span> | <span data-ttu-id="e6a40-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6a40-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6a40-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6a40-127">Request body</span></span>
<span data-ttu-id="e6a40-128">No corpo da solicitação, fornece uma representação JSON de um [objeto program.](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="e6a40-128">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="e6a40-129">A tabela a seguir mostra as propriedades que podem ser fornecidas quando você atualiza um programa.</span><span class="sxs-lookup"><span data-stu-id="e6a40-129">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="e6a40-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6a40-130">Property</span></span>     | <span data-ttu-id="e6a40-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6a40-131">Type</span></span>        | <span data-ttu-id="e6a40-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6a40-132">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="e6a40-133">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="e6a40-133">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="e6a40-134">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="e6a40-134">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="e6a40-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6a40-135">Response</span></span>
<span data-ttu-id="e6a40-136">Se tiver êxito, este método retornará `204, Accepted` um código de resposta e um objeto [program](../resources/program.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6a40-136">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6a40-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6a40-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6a40-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6a40-138">Request</span></span>
<span data-ttu-id="e6a40-139">No corpo da solicitação, fornece uma representação JSON dos parâmetros de objeto do [programa](../resources/program.md) a ser alterado.</span><span class="sxs-lookup"><span data-stu-id="e6a40-139">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>


# <a name="http"></a>[<span data-ttu-id="e6a40-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6a40-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e6a40-141">C#</span><span class="sxs-lookup"><span data-stu-id="e6a40-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6a40-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6a40-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6a40-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6a40-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6a40-144">Java</span><span class="sxs-lookup"><span data-stu-id="e6a40-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-program-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e6a40-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6a40-145">Response</span></span>
><span data-ttu-id="e6a40-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6a40-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="e6a40-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="e6a40-148">See also</span></span>

| <span data-ttu-id="e6a40-149">Método</span><span class="sxs-lookup"><span data-stu-id="e6a40-149">Method</span></span>           | <span data-ttu-id="e6a40-150">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e6a40-150">Return Type</span></span>    |<span data-ttu-id="e6a40-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6a40-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e6a40-152">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="e6a40-152">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="e6a40-153">[Coleção programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="e6a40-153">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="e6a40-154">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="e6a40-154">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="e6a40-155">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="e6a40-155">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="e6a40-156">programControl</span><span class="sxs-lookup"><span data-stu-id="e6a40-156">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="e6a40-157">Adicione um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="e6a40-157">Add a programControl to a program.</span></span>|

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


