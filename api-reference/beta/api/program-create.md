---
title: Criação de programa
description: No Windows Azure AD para acessar o recurso de revisões, crie um novo objeto de programa.
ms.openlocfilehash: 1ac3fa1f0b555fc92449adf0e57217d0a7d50375
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039150"
---
# <a name="create-program"></a><span data-ttu-id="853b7-103">Criação de programa</span><span class="sxs-lookup"><span data-stu-id="853b7-103">Create program</span></span>

> <span data-ttu-id="853b7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="853b7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="853b7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="853b7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="853b7-106">O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, cria um novo objeto de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="853b7-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="853b7-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="853b7-107">Permissions</span></span>
<span data-ttu-id="853b7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="853b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="853b7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="853b7-110">Permission type</span></span>                        | <span data-ttu-id="853b7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="853b7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="853b7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="853b7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="853b7-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="853b7-113"></span></span>  <span data-ttu-id="853b7-114">O usuário conectado também deve ser uma função de diretório que permite a atualização-los para criar um programa.</span><span class="sxs-lookup"><span data-stu-id="853b7-114">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="853b7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="853b7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="853b7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="853b7-116">Not supported.</span></span> |
|<span data-ttu-id="853b7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="853b7-117">Application</span></span>                            | <span data-ttu-id="853b7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="853b7-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="853b7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="853b7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="853b7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="853b7-120">Request headers</span></span>
| <span data-ttu-id="853b7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="853b7-121">Name</span></span>         | <span data-ttu-id="853b7-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="853b7-122">Type</span></span>        | <span data-ttu-id="853b7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="853b7-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="853b7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="853b7-124">Authorization</span></span> | <span data-ttu-id="853b7-125">string</span><span class="sxs-lookup"><span data-stu-id="853b7-125">string</span></span> | <span data-ttu-id="853b7-126">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="853b7-126">Bearer \{token\}.</span></span> <span data-ttu-id="853b7-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="853b7-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="853b7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="853b7-128">Request body</span></span>
<span data-ttu-id="853b7-129">No corpo da solicitação, fornece uma representação JSON de um objeto de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="853b7-129">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="853b7-130">A tabela a seguir mostra as propriedades que são necessárias quando você criar um programa.</span><span class="sxs-lookup"><span data-stu-id="853b7-130">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="853b7-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="853b7-131">Property</span></span>     | <span data-ttu-id="853b7-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="853b7-132">Type</span></span>        | <span data-ttu-id="853b7-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="853b7-133">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="853b7-134">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="853b7-134">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="853b7-135">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="853b7-135">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="853b7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="853b7-136">Response</span></span>
<span data-ttu-id="853b7-137">Se tiver êxito, este método retornará um `201, Created` objeto de [programa](../resources/program.md) e código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="853b7-137">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="853b7-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="853b7-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="853b7-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="853b7-139">Request</span></span>
<span data-ttu-id="853b7-140">No corpo da solicitação, fornece uma representação JSON do objeto de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="853b7-140">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="853b7-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="853b7-141">Response</span></span>
><span data-ttu-id="853b7-p105">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="853b7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="853b7-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="853b7-144">See also</span></span>

| <span data-ttu-id="853b7-145">Método</span><span class="sxs-lookup"><span data-stu-id="853b7-145">Method</span></span>           | <span data-ttu-id="853b7-146">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="853b7-146">Return Type</span></span>    |<span data-ttu-id="853b7-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="853b7-147">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="853b7-148">Lista de programas</span><span class="sxs-lookup"><span data-stu-id="853b7-148">List programs</span></span>](program-list.md) | <span data-ttu-id="853b7-149">coleção de [programa](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="853b7-149">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="853b7-150">Obtenha uma coleção de todos os programas.</span><span class="sxs-lookup"><span data-stu-id="853b7-150">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="853b7-151">Lista programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="853b7-151">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="853b7-152">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="853b7-152">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="853b7-153">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="853b7-153">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="853b7-154">Programa de atualização</span><span class="sxs-lookup"><span data-stu-id="853b7-154">Update program</span></span>](program-update.md) |  [<span data-ttu-id="853b7-155">programa</span><span class="sxs-lookup"><span data-stu-id="853b7-155">program</span></span>](../resources/program.md)| <span data-ttu-id="853b7-156">Atualize um programa.</span><span class="sxs-lookup"><span data-stu-id="853b7-156">Update a program.</span></span>|
|[<span data-ttu-id="853b7-157">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="853b7-157">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="853b7-158">programControl</span><span class="sxs-lookup"><span data-stu-id="853b7-158">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="853b7-159">Adicione um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="853b7-159">Add a programControl to a program.</span></span>|

<!-- {
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
