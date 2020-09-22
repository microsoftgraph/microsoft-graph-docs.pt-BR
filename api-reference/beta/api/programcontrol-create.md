---
title: Criar programControl
description: No recurso de revisões do Azure AD Access, crie um novo objeto programControl.  Isso vincula uma revisão do Access a um programa.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: f27094a28423137eb6c8e9661b42449f9cf7ac6c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986228"
---
# <a name="create-programcontrol"></a><span data-ttu-id="f2dc9-104">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="f2dc9-104">Create programControl</span></span>

<span data-ttu-id="f2dc9-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2dc9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2dc9-106">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , crie um novo objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="f2dc9-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="f2dc9-107">Isso vincula uma revisão do Access a um programa.</span><span class="sxs-lookup"><span data-stu-id="f2dc9-107">This links an access review to a program.</span></span>

<span data-ttu-id="f2dc9-108">Antes de fazer essa solicitação, o chamador deve ter sido</span><span class="sxs-lookup"><span data-stu-id="f2dc9-108">Prior to making this request, the caller must have previously</span></span>

- <span data-ttu-id="f2dc9-109">[criou um programa](program-create.md) ou [recuperou um programa](program-list.md), para que o valor de `programId` a ser incluído na solicitação,</span><span class="sxs-lookup"><span data-stu-id="f2dc9-109">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
- <span data-ttu-id="f2dc9-110">[criou uma revisão do Access](accessreview-create.md) ou [recuperou uma revisão do Access](accessreview-get.md), para que o valor de `controlId` seja incluído na solicitação e</span><span class="sxs-lookup"><span data-stu-id="f2dc9-110">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
- <span data-ttu-id="f2dc9-111">[recuperada a lista de tipos de controle de programa](programcontroltype-list.md)para que o valor de `controlTypeId` seja incluído na solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2dc9-111">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="f2dc9-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2dc9-112">Permissions</span></span>
<span data-ttu-id="f2dc9-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2dc9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2dc9-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2dc9-115">Permission type</span></span>                        | <span data-ttu-id="f2dc9-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2dc9-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2dc9-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2dc9-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2dc9-118">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2dc9-118">ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="f2dc9-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2dc9-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2dc9-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2dc9-120">Not supported.</span></span> |
|<span data-ttu-id="f2dc9-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2dc9-121">Application</span></span>                            |  <span data-ttu-id="f2dc9-122">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2dc9-122">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="f2dc9-123">O usuário conectado também deve estar em uma função de diretório que permite que eles criem um **programControl**.</span><span class="sxs-lookup"><span data-stu-id="f2dc9-123">The signed in user must also be in a directory role that permits them to create a **programControl**.</span></span> 

## <a name="http-request"></a><span data-ttu-id="f2dc9-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2dc9-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="f2dc9-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2dc9-125">Request headers</span></span>
| <span data-ttu-id="f2dc9-126">Nome</span><span class="sxs-lookup"><span data-stu-id="f2dc9-126">Name</span></span>         | <span data-ttu-id="f2dc9-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2dc9-127">Type</span></span>        | <span data-ttu-id="f2dc9-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2dc9-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f2dc9-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2dc9-129">Authorization</span></span> | <span data-ttu-id="f2dc9-130">string</span><span class="sxs-lookup"><span data-stu-id="f2dc9-130">string</span></span> | <span data-ttu-id="f2dc9-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2dc9-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2dc9-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2dc9-133">Request body</span></span>
<span data-ttu-id="f2dc9-134">No corpo da solicitação, forneça uma representação JSON de um objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="f2dc9-134">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="f2dc9-135">A tabela a seguir mostra as propriedades que são necessárias ao criar um controle de programa.</span><span class="sxs-lookup"><span data-stu-id="f2dc9-135">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="f2dc9-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2dc9-136">Property</span></span>     | <span data-ttu-id="f2dc9-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2dc9-137">Type</span></span>        | <span data-ttu-id="f2dc9-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2dc9-138">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="f2dc9-139">O ProgramId do programa para o qual esse controle se tornará parte.</span><span class="sxs-lookup"><span data-stu-id="f2dc9-139">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="f2dc9-140">O controlId do controle, em particular, o identificador de uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="f2dc9-140">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="f2dc9-141">O programControlType identifica o tipo de controle de programa-por exemplo, um controle vinculando a revisões de acesso de convidados.</span><span class="sxs-lookup"><span data-stu-id="f2dc9-141">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="f2dc9-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2dc9-142">Response</span></span>
<span data-ttu-id="f2dc9-143">Se tiver êxito, este método retornará um `201, Created` código de resposta e um objeto [programControl](../resources/programcontrol.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2dc9-143">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="f2dc9-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2dc9-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2dc9-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2dc9-145">Request</span></span>
<span data-ttu-id="f2dc9-146">No corpo da solicitação, forneça uma representação JSON do objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="f2dc9-146">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="f2dc9-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2dc9-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f2dc9-148">C#</span><span class="sxs-lookup"><span data-stu-id="f2dc9-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-programcontrol-from-programcontrols-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2dc9-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2dc9-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-programcontrol-from-programcontrols-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2dc9-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2dc9-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-programcontrol-from-programcontrols-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f2dc9-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2dc9-151">Response</span></span>
><span data-ttu-id="f2dc9-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2dc9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="f2dc9-154">Confira também</span><span class="sxs-lookup"><span data-stu-id="f2dc9-154">See also</span></span>

| <span data-ttu-id="f2dc9-155">Método</span><span class="sxs-lookup"><span data-stu-id="f2dc9-155">Method</span></span>           | <span data-ttu-id="f2dc9-156">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f2dc9-156">Return Type</span></span>    |<span data-ttu-id="f2dc9-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2dc9-157">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f2dc9-158">Listar programControlTypes</span><span class="sxs-lookup"><span data-stu-id="f2dc9-158">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="f2dc9-159">coleção [programControlType](../resources/programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="f2dc9-159">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="f2dc9-160">Listar tipos de controle de programa.</span><span class="sxs-lookup"><span data-stu-id="f2dc9-160">List program control types.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


