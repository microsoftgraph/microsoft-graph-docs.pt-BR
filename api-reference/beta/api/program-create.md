---
title: Criar programa
description: No recurso de revisões do Azure AD Access, crie um novo objeto de programa.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 003576935dd2f963879f2fa70e741c3d3f44a885
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087982"
---
# <a name="create-program"></a><span data-ttu-id="82ca7-103">Criar programa</span><span class="sxs-lookup"><span data-stu-id="82ca7-103">Create program</span></span>

<span data-ttu-id="82ca7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82ca7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82ca7-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , crie um novo objeto de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="82ca7-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="82ca7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="82ca7-106">Permissions</span></span>
<span data-ttu-id="82ca7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82ca7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82ca7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82ca7-109">Permission type</span></span>                        | <span data-ttu-id="82ca7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="82ca7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="82ca7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82ca7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="82ca7-112">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82ca7-112">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="82ca7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82ca7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82ca7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82ca7-114">Not supported.</span></span> |
|<span data-ttu-id="82ca7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82ca7-115">Application</span></span>                            | <span data-ttu-id="82ca7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82ca7-116">Not supported.</span></span> |

<span data-ttu-id="82ca7-117">O usuário conectado também deve estar em uma função de diretório que permite que eles criem um programa.</span><span class="sxs-lookup"><span data-stu-id="82ca7-117">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="82ca7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82ca7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="82ca7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82ca7-119">Request headers</span></span>
| <span data-ttu-id="82ca7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="82ca7-120">Name</span></span>         | <span data-ttu-id="82ca7-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="82ca7-121">Type</span></span>        | <span data-ttu-id="82ca7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="82ca7-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="82ca7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="82ca7-123">Authorization</span></span> | <span data-ttu-id="82ca7-124">string</span><span class="sxs-lookup"><span data-stu-id="82ca7-124">string</span></span> | <span data-ttu-id="82ca7-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82ca7-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82ca7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82ca7-127">Request body</span></span>
<span data-ttu-id="82ca7-128">No corpo da solicitação, forneça uma representação JSON de um objeto [Program](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="82ca7-128">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="82ca7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar um programa.</span><span class="sxs-lookup"><span data-stu-id="82ca7-129">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="82ca7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82ca7-130">Property</span></span>     | <span data-ttu-id="82ca7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="82ca7-131">Type</span></span>        | <span data-ttu-id="82ca7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="82ca7-132">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="82ca7-133">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="82ca7-133">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="82ca7-134">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="82ca7-134">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="82ca7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="82ca7-135">Response</span></span>
<span data-ttu-id="82ca7-136">Se bem-sucedido, este método retorna um `201, Created` código de resposta e um objeto [Program](../resources/program.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82ca7-136">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82ca7-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82ca7-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82ca7-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82ca7-138">Request</span></span>
<span data-ttu-id="82ca7-139">No corpo da solicitação, forneça uma representação JSON do objeto [Program](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="82ca7-139">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="82ca7-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="82ca7-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="82ca7-141">C#</span><span class="sxs-lookup"><span data-stu-id="82ca7-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-program-from-programs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82ca7-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82ca7-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-program-from-programs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82ca7-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82ca7-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-program-from-programs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="82ca7-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="82ca7-144">Response</span></span>
><span data-ttu-id="82ca7-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82ca7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="82ca7-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="82ca7-147">See also</span></span>

| <span data-ttu-id="82ca7-148">Método</span><span class="sxs-lookup"><span data-stu-id="82ca7-148">Method</span></span>           | <span data-ttu-id="82ca7-149">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="82ca7-149">Return Type</span></span>    |<span data-ttu-id="82ca7-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="82ca7-150">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="82ca7-151">Listar programas</span><span class="sxs-lookup"><span data-stu-id="82ca7-151">List programs</span></span>](program-list.md) | <span data-ttu-id="82ca7-152">coleção [Program](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="82ca7-152">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="82ca7-153">Obtenha uma coleção de todos os programas.</span><span class="sxs-lookup"><span data-stu-id="82ca7-153">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="82ca7-154">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="82ca7-154">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="82ca7-155">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="82ca7-155">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="82ca7-156">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="82ca7-156">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="82ca7-157">Programa de atualização</span><span class="sxs-lookup"><span data-stu-id="82ca7-157">Update program</span></span>](program-update.md) |  [<span data-ttu-id="82ca7-158">programa</span><span class="sxs-lookup"><span data-stu-id="82ca7-158">program</span></span>](../resources/program.md)| <span data-ttu-id="82ca7-159">Atualizar um programa.</span><span class="sxs-lookup"><span data-stu-id="82ca7-159">Update a program.</span></span>|
|[<span data-ttu-id="82ca7-160">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="82ca7-160">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="82ca7-161">programControl</span><span class="sxs-lookup"><span data-stu-id="82ca7-161">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="82ca7-162">Adicionar um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="82ca7-162">Add a programControl to a program.</span></span>|

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


