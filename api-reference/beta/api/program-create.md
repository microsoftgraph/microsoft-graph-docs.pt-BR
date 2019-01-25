---
title: Criação de programa
description: No Windows Azure AD para acessar o recurso de revisões, crie um novo objeto de programa.
localization_priority: Normal
ms.openlocfilehash: a6e9ab300cf44a2f3973c468679af7fa48262680
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521296"
---
# <a name="create-program"></a><span data-ttu-id="08686-103">Criação de programa</span><span class="sxs-lookup"><span data-stu-id="08686-103">Create program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08686-104">O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, cria um novo objeto de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="08686-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="08686-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="08686-105">Permissions</span></span>
<span data-ttu-id="08686-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08686-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08686-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08686-108">Permission type</span></span>                        | <span data-ttu-id="08686-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08686-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="08686-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08686-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="08686-111">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="08686-111"></span></span>  <span data-ttu-id="08686-112">O usuário conectado também deve ser uma função de diretório que permite a atualização-los para criar um programa.</span><span class="sxs-lookup"><span data-stu-id="08686-112">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="08686-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08686-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08686-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08686-114">Not supported.</span></span> |
|<span data-ttu-id="08686-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08686-115">Application</span></span>                            | <span data-ttu-id="08686-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08686-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08686-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08686-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="08686-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08686-118">Request headers</span></span>
| <span data-ttu-id="08686-119">Nome</span><span class="sxs-lookup"><span data-stu-id="08686-119">Name</span></span>         | <span data-ttu-id="08686-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="08686-120">Type</span></span>        | <span data-ttu-id="08686-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="08686-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="08686-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="08686-122">Authorization</span></span> | <span data-ttu-id="08686-123">string</span><span class="sxs-lookup"><span data-stu-id="08686-123">string</span></span> | <span data-ttu-id="08686-124">Token de portador</span><span class="sxs-lookup"><span data-stu-id="08686-124">Bearer \{token\}.</span></span> <span data-ttu-id="08686-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08686-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08686-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08686-126">Request body</span></span>
<span data-ttu-id="08686-127">No corpo da solicitação, fornece uma representação JSON de um objeto de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="08686-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="08686-128">A tabela a seguir mostra as propriedades que são necessárias quando você criar um programa.</span><span class="sxs-lookup"><span data-stu-id="08686-128">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="08686-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08686-129">Property</span></span>     | <span data-ttu-id="08686-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="08686-130">Type</span></span>        | <span data-ttu-id="08686-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="08686-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="08686-132">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="08686-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="08686-133">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="08686-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="08686-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="08686-134">Response</span></span>
<span data-ttu-id="08686-135">Se tiver êxito, este método retornará um `201, Created` objeto de [programa](../resources/program.md) e código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08686-135">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08686-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08686-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08686-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08686-137">Request</span></span>
<span data-ttu-id="08686-138">No corpo da solicitação, fornece uma representação JSON do objeto de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="08686-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="08686-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="08686-139">Response</span></span>
><span data-ttu-id="08686-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08686-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="08686-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="08686-142">See also</span></span>

| <span data-ttu-id="08686-143">Método</span><span class="sxs-lookup"><span data-stu-id="08686-143">Method</span></span>           | <span data-ttu-id="08686-144">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="08686-144">Return Type</span></span>    |<span data-ttu-id="08686-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="08686-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="08686-146">Lista de programas</span><span class="sxs-lookup"><span data-stu-id="08686-146">List programs</span></span>](program-list.md) | <span data-ttu-id="08686-147">coleção de [programa](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="08686-147">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="08686-148">Obtenha uma coleção de todos os programas.</span><span class="sxs-lookup"><span data-stu-id="08686-148">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="08686-149">Lista programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="08686-149">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="08686-150">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="08686-150">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="08686-151">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="08686-151">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="08686-152">Programa de atualização</span><span class="sxs-lookup"><span data-stu-id="08686-152">Update program</span></span>](program-update.md) |  [<span data-ttu-id="08686-153">programa</span><span class="sxs-lookup"><span data-stu-id="08686-153">program</span></span>](../resources/program.md)| <span data-ttu-id="08686-154">Atualize um programa.</span><span class="sxs-lookup"><span data-stu-id="08686-154">Update a program.</span></span>|
|[<span data-ttu-id="08686-155">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="08686-155">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="08686-156">programControl</span><span class="sxs-lookup"><span data-stu-id="08686-156">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="08686-157">Adicione um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="08686-157">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
