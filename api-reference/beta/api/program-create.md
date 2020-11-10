---
title: Criar programa
description: No recurso de revisões do Azure AD Access, crie um novo objeto de programa.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 0d062b35ad5fc9e47b3a4dc89914c4c896e53a60
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977910"
---
# <a name="create-program"></a><span data-ttu-id="bd310-103">Criar programa</span><span class="sxs-lookup"><span data-stu-id="bd310-103">Create program</span></span>

<span data-ttu-id="bd310-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd310-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd310-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , crie um novo objeto de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="bd310-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bd310-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bd310-106">Permissions</span></span>
<span data-ttu-id="bd310-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd310-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd310-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd310-109">Permission type</span></span>                        | <span data-ttu-id="bd310-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd310-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd310-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd310-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd310-112">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd310-112">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="bd310-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd310-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd310-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd310-114">Not supported.</span></span> |
|<span data-ttu-id="bd310-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd310-115">Application</span></span>                            | <span data-ttu-id="bd310-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd310-116">Not supported.</span></span> |

<span data-ttu-id="bd310-117">O usuário conectado também deve estar em uma função de diretório que permite que eles criem um programa.</span><span class="sxs-lookup"><span data-stu-id="bd310-117">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="bd310-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd310-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="bd310-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd310-119">Request headers</span></span>
| <span data-ttu-id="bd310-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bd310-120">Name</span></span>         | <span data-ttu-id="bd310-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd310-121">Type</span></span>        | <span data-ttu-id="bd310-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd310-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bd310-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd310-123">Authorization</span></span> | <span data-ttu-id="bd310-124">string</span><span class="sxs-lookup"><span data-stu-id="bd310-124">string</span></span> | <span data-ttu-id="bd310-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd310-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd310-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd310-127">Request body</span></span>
<span data-ttu-id="bd310-128">No corpo da solicitação, forneça uma representação JSON de um objeto [Program](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="bd310-128">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="bd310-129">A tabela a seguir mostra as propriedades que são necessárias ao criar um programa.</span><span class="sxs-lookup"><span data-stu-id="bd310-129">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="bd310-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd310-130">Property</span></span>     | <span data-ttu-id="bd310-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd310-131">Type</span></span>        | <span data-ttu-id="bd310-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd310-132">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="bd310-133">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="bd310-133">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="bd310-134">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="bd310-134">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="bd310-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd310-135">Response</span></span>
<span data-ttu-id="bd310-136">Se bem-sucedido, este método retorna um `201, Created` código de resposta e um objeto [Program](../resources/program.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd310-136">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd310-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd310-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bd310-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd310-138">Request</span></span>
<span data-ttu-id="bd310-139">No corpo da solicitação, forneça uma representação JSON do objeto [Program](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="bd310-139">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="bd310-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd310-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bd310-141">C#</span><span class="sxs-lookup"><span data-stu-id="bd310-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-program-from-programs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd310-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd310-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-program-from-programs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd310-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd310-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-program-from-programs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bd310-144">Java</span><span class="sxs-lookup"><span data-stu-id="bd310-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-program-from-programs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bd310-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd310-145">Response</span></span>
><span data-ttu-id="bd310-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bd310-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="bd310-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="bd310-148">See also</span></span>

| <span data-ttu-id="bd310-149">Método</span><span class="sxs-lookup"><span data-stu-id="bd310-149">Method</span></span>           | <span data-ttu-id="bd310-150">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bd310-150">Return Type</span></span>    |<span data-ttu-id="bd310-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd310-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bd310-152">Listar programas</span><span class="sxs-lookup"><span data-stu-id="bd310-152">List programs</span></span>](program-list.md) | <span data-ttu-id="bd310-153">coleção [Program](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="bd310-153">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="bd310-154">Obtenha uma coleção de todos os programas.</span><span class="sxs-lookup"><span data-stu-id="bd310-154">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="bd310-155">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="bd310-155">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="bd310-156">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="bd310-156">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="bd310-157">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="bd310-157">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="bd310-158">Programa de atualização</span><span class="sxs-lookup"><span data-stu-id="bd310-158">Update program</span></span>](program-update.md) |  [<span data-ttu-id="bd310-159">programa</span><span class="sxs-lookup"><span data-stu-id="bd310-159">program</span></span>](../resources/program.md)| <span data-ttu-id="bd310-160">Atualizar um programa.</span><span class="sxs-lookup"><span data-stu-id="bd310-160">Update a program.</span></span>|
|[<span data-ttu-id="bd310-161">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="bd310-161">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="bd310-162">programControl</span><span class="sxs-lookup"><span data-stu-id="bd310-162">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="bd310-163">Adicionar um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="bd310-163">Add a programControl to a program.</span></span>|

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


