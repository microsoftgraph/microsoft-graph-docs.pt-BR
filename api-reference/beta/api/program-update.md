---
title: Programa de atualização
description: No Windows Azure AD para acessar o recurso de revisões, atualização de um objeto existente do programa.
localization_priority: Normal
ms.openlocfilehash: 75562aac5a7b3f3aaef0c8a1251d32a7728813aa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529919"
---
# <a name="update-program"></a><span data-ttu-id="bce4b-103">Programa de atualização</span><span class="sxs-lookup"><span data-stu-id="bce4b-103">Update program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bce4b-104">O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, atualize um objeto existente do [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="bce4b-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bce4b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bce4b-105">Permissions</span></span>
<span data-ttu-id="bce4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bce4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bce4b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bce4b-108">Permission type</span></span>                        | <span data-ttu-id="bce4b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bce4b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bce4b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bce4b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bce4b-111">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="bce4b-111"></span></span>  <span data-ttu-id="bce4b-112">O usuário conectado também deve ser em uma função de diretório que permite que eles atualizem o programa.</span><span class="sxs-lookup"><span data-stu-id="bce4b-112">The signed in user must also be in a directory role which permits them to update a program.</span></span> |
|<span data-ttu-id="bce4b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bce4b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bce4b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bce4b-114">Not supported.</span></span> |
|<span data-ttu-id="bce4b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bce4b-115">Application</span></span>                            | <span data-ttu-id="bce4b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bce4b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bce4b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bce4b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="bce4b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bce4b-118">Request headers</span></span>
| <span data-ttu-id="bce4b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bce4b-119">Name</span></span>         | <span data-ttu-id="bce4b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="bce4b-120">Type</span></span>        | <span data-ttu-id="bce4b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bce4b-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bce4b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bce4b-122">Authorization</span></span> | <span data-ttu-id="bce4b-123">string</span><span class="sxs-lookup"><span data-stu-id="bce4b-123">string</span></span> | <span data-ttu-id="bce4b-124">Token de portador</span><span class="sxs-lookup"><span data-stu-id="bce4b-124">Bearer \{token\}.</span></span> <span data-ttu-id="bce4b-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bce4b-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bce4b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bce4b-126">Request body</span></span>
<span data-ttu-id="bce4b-127">No corpo da solicitação, fornece uma representação JSON de um objeto de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="bce4b-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="bce4b-128">A tabela a seguir mostra as propriedades que podem ser fornecidas quando você atualiza um programa.</span><span class="sxs-lookup"><span data-stu-id="bce4b-128">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="bce4b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bce4b-129">Property</span></span>     | <span data-ttu-id="bce4b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bce4b-130">Type</span></span>        | <span data-ttu-id="bce4b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bce4b-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="bce4b-132">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="bce4b-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="bce4b-133">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="bce4b-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="bce4b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bce4b-134">Response</span></span>
<span data-ttu-id="bce4b-135">Se tiver êxito, este método retornará um `204, Accepted` objeto de [programa](../resources/program.md) e código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bce4b-135">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bce4b-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bce4b-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bce4b-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bce4b-137">Request</span></span>
<span data-ttu-id="bce4b-138">No corpo da solicitação, fornece uma representação JSON dos parâmetros de objeto do [programa](../resources/program.md) para alterar.</span><span class="sxs-lookup"><span data-stu-id="bce4b-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_program"
}-->
```http
PATCH https://graph.microsoft.com/beta/programs('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
Content-type: application/json

{
    "displayName": "testprogram3 new name"
}
```

##### <a name="response"></a><span data-ttu-id="bce4b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="bce4b-139">Response</span></span>
><span data-ttu-id="bce4b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bce4b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="bce4b-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="bce4b-142">See also</span></span>

| <span data-ttu-id="bce4b-143">Método</span><span class="sxs-lookup"><span data-stu-id="bce4b-143">Method</span></span>           | <span data-ttu-id="bce4b-144">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bce4b-144">Return Type</span></span>    |<span data-ttu-id="bce4b-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="bce4b-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bce4b-146">Lista programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="bce4b-146">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="bce4b-147">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="bce4b-147">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="bce4b-148">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="bce4b-148">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="bce4b-149">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="bce4b-149">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="bce4b-150">programControl</span><span class="sxs-lookup"><span data-stu-id="bce4b-150">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="bce4b-151">Adicione um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="bce4b-151">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
