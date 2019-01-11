---
title: Criação de programa
description: No Windows Azure AD para acessar o recurso de revisões, crie um novo objeto de programa.
localization_priority: Normal
ms.openlocfilehash: b982242bbdddb9769d64c9757d9041fddc215d53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844013"
---
# <a name="create-program"></a><span data-ttu-id="1e76d-103">Criação de programa</span><span class="sxs-lookup"><span data-stu-id="1e76d-103">Create program</span></span>

> <span data-ttu-id="1e76d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1e76d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e76d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1e76d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1e76d-106">O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, cria um novo objeto de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="1e76d-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1e76d-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="1e76d-107">Permissions</span></span>
<span data-ttu-id="1e76d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e76d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e76d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e76d-110">Permission type</span></span>                        | <span data-ttu-id="1e76d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1e76d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e76d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e76d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1e76d-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="1e76d-113"></span></span>  <span data-ttu-id="1e76d-114">O usuário conectado também deve ser uma função de diretório que permite a atualização-los para criar um programa.</span><span class="sxs-lookup"><span data-stu-id="1e76d-114">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="1e76d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e76d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e76d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e76d-116">Not supported.</span></span> |
|<span data-ttu-id="1e76d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e76d-117">Application</span></span>                            | <span data-ttu-id="1e76d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e76d-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e76d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e76d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="1e76d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e76d-120">Request headers</span></span>
| <span data-ttu-id="1e76d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1e76d-121">Name</span></span>         | <span data-ttu-id="1e76d-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e76d-122">Type</span></span>        | <span data-ttu-id="1e76d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e76d-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1e76d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e76d-124">Authorization</span></span> | <span data-ttu-id="1e76d-125">string</span><span class="sxs-lookup"><span data-stu-id="1e76d-125">string</span></span> | <span data-ttu-id="1e76d-126">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="1e76d-126">Bearer \{token\}.</span></span> <span data-ttu-id="1e76d-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e76d-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e76d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e76d-128">Request body</span></span>
<span data-ttu-id="1e76d-129">No corpo da solicitação, fornece uma representação JSON de um objeto de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="1e76d-129">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="1e76d-130">A tabela a seguir mostra as propriedades que são necessárias quando você criar um programa.</span><span class="sxs-lookup"><span data-stu-id="1e76d-130">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="1e76d-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e76d-131">Property</span></span>     | <span data-ttu-id="1e76d-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e76d-132">Type</span></span>        | <span data-ttu-id="1e76d-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e76d-133">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="1e76d-134">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="1e76d-134">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="1e76d-135">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="1e76d-135">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="1e76d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e76d-136">Response</span></span>
<span data-ttu-id="1e76d-137">Se tiver êxito, este método retornará um `201, Created` objeto de [programa](../resources/program.md) e código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e76d-137">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e76d-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e76d-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e76d-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e76d-139">Request</span></span>
<span data-ttu-id="1e76d-140">No corpo da solicitação, fornece uma representação JSON do objeto de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="1e76d-140">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="1e76d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e76d-141">Response</span></span>
><span data-ttu-id="1e76d-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e76d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="1e76d-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="1e76d-144">See also</span></span>

| <span data-ttu-id="1e76d-145">Método</span><span class="sxs-lookup"><span data-stu-id="1e76d-145">Method</span></span>           | <span data-ttu-id="1e76d-146">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1e76d-146">Return Type</span></span>    |<span data-ttu-id="1e76d-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e76d-147">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1e76d-148">Lista de programas</span><span class="sxs-lookup"><span data-stu-id="1e76d-148">List programs</span></span>](program-list.md) | <span data-ttu-id="1e76d-149">coleção de [programa](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="1e76d-149">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="1e76d-150">Obtenha uma coleção de todos os programas.</span><span class="sxs-lookup"><span data-stu-id="1e76d-150">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="1e76d-151">Lista programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="1e76d-151">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="1e76d-152">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="1e76d-152">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="1e76d-153">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="1e76d-153">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="1e76d-154">Programa de atualização</span><span class="sxs-lookup"><span data-stu-id="1e76d-154">Update program</span></span>](program-update.md) |  [<span data-ttu-id="1e76d-155">programa</span><span class="sxs-lookup"><span data-stu-id="1e76d-155">program</span></span>](../resources/program.md)| <span data-ttu-id="1e76d-156">Atualize um programa.</span><span class="sxs-lookup"><span data-stu-id="1e76d-156">Update a program.</span></span>|
|[<span data-ttu-id="1e76d-157">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="1e76d-157">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="1e76d-158">programControl</span><span class="sxs-lookup"><span data-stu-id="1e76d-158">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="1e76d-159">Adicione um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="1e76d-159">Add a programControl to a program.</span></span>|

<!-- {
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
