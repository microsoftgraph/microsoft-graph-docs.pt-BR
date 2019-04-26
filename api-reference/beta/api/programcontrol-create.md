---
title: Criar programControl
description: No recurso de revisões do Azure AD Access, crie um novo objeto programControl.  Isso vincula uma revisão do Access a um programa.
localization_priority: Normal
ms.openlocfilehash: d7a48b45049c2268856a3ec238114cfa9bf834f5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332026"
---
# <a name="create-programcontrol"></a><span data-ttu-id="a6c39-104">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="a6c39-104">Create programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6c39-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , crie um novo objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="a6c39-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="a6c39-106">Isso vincula uma revisão do Access a um programa.</span><span class="sxs-lookup"><span data-stu-id="a6c39-106">This links an access review to a program.</span></span>

<span data-ttu-id="a6c39-107">Antes de fazer essa solicitação, o chamador deve ter sido</span><span class="sxs-lookup"><span data-stu-id="a6c39-107">Prior to making this request, the caller must have previously</span></span>

 - <span data-ttu-id="a6c39-108">[criou um programa](program-create.md) ou [recuperou um programa](program-list.md), para que o valor `programId` de a ser incluído na solicitação,</span><span class="sxs-lookup"><span data-stu-id="a6c39-108">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
 - <span data-ttu-id="a6c39-109">[criou uma revisão do Access](accessreview-create.md) ou [recuperou uma revisão do Access](accessreview-get.md), para que `controlId` o valor de seja incluído na solicitação e</span><span class="sxs-lookup"><span data-stu-id="a6c39-109">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
 - <span data-ttu-id="a6c39-110">[recuperada a lista de tipos de controle de programa](programcontroltype-list.md)para que o `controlTypeId` valor de seja incluído na solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6c39-110">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="a6c39-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="a6c39-111">Permissions</span></span>
<span data-ttu-id="a6c39-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6c39-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6c39-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6c39-114">Permission type</span></span>                        | <span data-ttu-id="a6c39-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6c39-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6c39-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6c39-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6c39-117">ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a6c39-117">ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="a6c39-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6c39-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6c39-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6c39-119">Not supported.</span></span> |
|<span data-ttu-id="a6c39-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6c39-120">Application</span></span>                            |  <span data-ttu-id="a6c39-121">ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a6c39-121">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="a6c39-122">O usuário conectado também deve estar em uma função de diretório que permite que eles criem um **programControl**.</span><span class="sxs-lookup"><span data-stu-id="a6c39-122">The signed in user must also be in a directory role that permits them to create a **programControl**.</span></span> 

## <a name="http-request"></a><span data-ttu-id="a6c39-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6c39-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="a6c39-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6c39-124">Request headers</span></span>
| <span data-ttu-id="a6c39-125">Nome</span><span class="sxs-lookup"><span data-stu-id="a6c39-125">Name</span></span>         | <span data-ttu-id="a6c39-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6c39-126">Type</span></span>        | <span data-ttu-id="a6c39-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6c39-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a6c39-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6c39-128">Authorization</span></span> | <span data-ttu-id="a6c39-129">string</span><span class="sxs-lookup"><span data-stu-id="a6c39-129">string</span></span> | <span data-ttu-id="a6c39-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6c39-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6c39-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6c39-132">Request body</span></span>
<span data-ttu-id="a6c39-133">No corpo da solicitação, forneça uma representação JSON de um objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="a6c39-133">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="a6c39-134">A tabela a seguir mostra as propriedades que são necessárias ao criar um controle de programa.</span><span class="sxs-lookup"><span data-stu-id="a6c39-134">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="a6c39-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6c39-135">Property</span></span>     | <span data-ttu-id="a6c39-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6c39-136">Type</span></span>        | <span data-ttu-id="a6c39-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6c39-137">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="a6c39-138">O ProgramId do programa para o qual esse controle se tornará parte.</span><span class="sxs-lookup"><span data-stu-id="a6c39-138">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="a6c39-139">O controlId do controle, em particular, o identificador de uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="a6c39-139">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="a6c39-140">O programControlType identifica o tipo de controle de programa-por exemplo, um controle vinculando a revisões de acesso de convidados.</span><span class="sxs-lookup"><span data-stu-id="a6c39-140">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="a6c39-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6c39-141">Response</span></span>
<span data-ttu-id="a6c39-142">Se tiver êxito, este método retornará `201, Created` um código de resposta e um objeto [programControl](../resources/programcontrol.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6c39-142">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="a6c39-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6c39-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a6c39-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6c39-144">Request</span></span>
<span data-ttu-id="a6c39-145">No corpo da solicitação, forneça uma representação JSON do objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="a6c39-145">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_programControl_from_programControls"
}-->
```http
POST https://graph.microsoft.com/beta/programControls
Content-type: application/json

{
    "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"
}
```

##### <a name="response"></a><span data-ttu-id="a6c39-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6c39-146">Response</span></span>
><span data-ttu-id="a6c39-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6c39-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "63b2302c-7e62-43b7-aefb-063ba5bdb853",
  "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
  "displayName": "test",
  "status": "Active",
  "createdDateTime": "2018-05-18T20:26:05.2976279Z"
}
```

## <a name="see-also"></a><span data-ttu-id="a6c39-149">Confira também</span><span class="sxs-lookup"><span data-stu-id="a6c39-149">See also</span></span>

| <span data-ttu-id="a6c39-150">Método</span><span class="sxs-lookup"><span data-stu-id="a6c39-150">Method</span></span>           | <span data-ttu-id="a6c39-151">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a6c39-151">Return Type</span></span>    |<span data-ttu-id="a6c39-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6c39-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a6c39-153">Listar programControlTypes</span><span class="sxs-lookup"><span data-stu-id="a6c39-153">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="a6c39-154">coleção [programControlType](../resources/programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="a6c39-154">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="a6c39-155">Listar tipos de controle de programa.</span><span class="sxs-lookup"><span data-stu-id="a6c39-155">List program control types.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
