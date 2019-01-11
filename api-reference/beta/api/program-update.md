---
title: Programa de atualização
description: No Windows Azure AD para acessar o recurso de revisões, atualização de um objeto existente do programa.
localization_priority: Normal
ms.openlocfilehash: a9abe10a2a672984d14f1da821b7ae6244cbdf39
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840331"
---
# <a name="update-program"></a><span data-ttu-id="0084b-103">Programa de atualização</span><span class="sxs-lookup"><span data-stu-id="0084b-103">Update program</span></span>

> <span data-ttu-id="0084b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0084b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0084b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0084b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0084b-106">O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, atualize um objeto existente do [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="0084b-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0084b-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="0084b-107">Permissions</span></span>
<span data-ttu-id="0084b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0084b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0084b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0084b-110">Permission type</span></span>                        | <span data-ttu-id="0084b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0084b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0084b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0084b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0084b-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="0084b-113"></span></span>  <span data-ttu-id="0084b-114">O usuário conectado também deve ser em uma função de diretório que permite que eles atualizem o programa.</span><span class="sxs-lookup"><span data-stu-id="0084b-114">The signed in user must also be in a directory role which permits them to update a program.</span></span> |
|<span data-ttu-id="0084b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0084b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0084b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0084b-116">Not supported.</span></span> |
|<span data-ttu-id="0084b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0084b-117">Application</span></span>                            | <span data-ttu-id="0084b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0084b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0084b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0084b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="0084b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0084b-120">Request headers</span></span>
| <span data-ttu-id="0084b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0084b-121">Name</span></span>         | <span data-ttu-id="0084b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="0084b-122">Type</span></span>        | <span data-ttu-id="0084b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0084b-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0084b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0084b-124">Authorization</span></span> | <span data-ttu-id="0084b-125">string</span><span class="sxs-lookup"><span data-stu-id="0084b-125">string</span></span> | <span data-ttu-id="0084b-126">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="0084b-126">Bearer \{token\}.</span></span> <span data-ttu-id="0084b-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0084b-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0084b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0084b-128">Request body</span></span>
<span data-ttu-id="0084b-129">No corpo da solicitação, fornece uma representação JSON de um objeto de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="0084b-129">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="0084b-130">A tabela a seguir mostra as propriedades que podem ser fornecidas quando você atualiza um programa.</span><span class="sxs-lookup"><span data-stu-id="0084b-130">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="0084b-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0084b-131">Property</span></span>     | <span data-ttu-id="0084b-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="0084b-132">Type</span></span>        | <span data-ttu-id="0084b-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="0084b-133">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="0084b-134">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="0084b-134">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="0084b-135">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="0084b-135">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="0084b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0084b-136">Response</span></span>
<span data-ttu-id="0084b-137">Se tiver êxito, este método retornará um `204, Accepted` objeto de [programa](../resources/program.md) e código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0084b-137">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0084b-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0084b-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0084b-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0084b-139">Request</span></span>
<span data-ttu-id="0084b-140">No corpo da solicitação, fornece uma representação JSON dos parâmetros de objeto do [programa](../resources/program.md) para alterar.</span><span class="sxs-lookup"><span data-stu-id="0084b-140">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>

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

##### <a name="response"></a><span data-ttu-id="0084b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0084b-141">Response</span></span>
><span data-ttu-id="0084b-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0084b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="0084b-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="0084b-144">See also</span></span>

| <span data-ttu-id="0084b-145">Método</span><span class="sxs-lookup"><span data-stu-id="0084b-145">Method</span></span>           | <span data-ttu-id="0084b-146">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0084b-146">Return Type</span></span>    |<span data-ttu-id="0084b-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="0084b-147">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0084b-148">Lista programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="0084b-148">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="0084b-149">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="0084b-149">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="0084b-150">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="0084b-150">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="0084b-151">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="0084b-151">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="0084b-152">programControl</span><span class="sxs-lookup"><span data-stu-id="0084b-152">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="0084b-153">Adicione um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="0084b-153">Add a programControl to a program.</span></span>|

<!-- {
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
