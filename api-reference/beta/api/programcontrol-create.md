---
title: Criar programControl
description: No Windows Azure AD para acessar o recurso de revisões, crie um novo objeto programControl.  Isso vincula uma revisão de acesso a um programa.
ms.openlocfilehash: fa6a93b13391fd4b9e3c5816bb2a27259e730c0d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038698"
---
# <a name="create-programcontrol"></a><span data-ttu-id="a6c73-104">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="a6c73-104">Create programControl</span></span>

> <span data-ttu-id="a6c73-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a6c73-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6c73-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a6c73-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6c73-107">O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, cria um novo objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="a6c73-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="a6c73-108">Isso vincula uma revisão de acesso a um programa.</span><span class="sxs-lookup"><span data-stu-id="a6c73-108">This links an access review to a program.</span></span>

<span data-ttu-id="a6c73-109">Antes de fazer essa solicitação, o chamador deve ter anteriormente</span><span class="sxs-lookup"><span data-stu-id="a6c73-109">Prior to making this request, the caller must have previously</span></span>

 - <span data-ttu-id="a6c73-110">[criado um programa](program-create.md) ou [recuperados de um programa](program-list.md), para que o valor de `programId` para incluir na solicitação,</span><span class="sxs-lookup"><span data-stu-id="a6c73-110">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
 - <span data-ttu-id="a6c73-111">[criada uma revisão de acesso](accessreview-create.md) ou [recuperado uma revisão de acesso](accessreview-get.md), para que o valor de `controlId` para incluir na solicitação, e</span><span class="sxs-lookup"><span data-stu-id="a6c73-111">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
 - <span data-ttu-id="a6c73-112">[recuperou a lista de tipos de controle de programas](programcontroltype-list.md), para que o valor de `controlTypeId` para incluir na solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6c73-112">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="a6c73-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="a6c73-113">Permissions</span></span>
<span data-ttu-id="a6c73-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6c73-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6c73-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6c73-116">Permission type</span></span>                        | <span data-ttu-id="a6c73-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6c73-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6c73-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6c73-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6c73-119">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="a6c73-119"></span></span>  <span data-ttu-id="a6c73-120">O usuário conectado também deve ser uma função de diretório que permite a atualização-los para criar um programControl.</span><span class="sxs-lookup"><span data-stu-id="a6c73-120">The signed in user must also be in a directory role which permits them to create a programControl.</span></span> |
|<span data-ttu-id="a6c73-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6c73-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6c73-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6c73-122">Not supported.</span></span> |
|<span data-ttu-id="a6c73-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6c73-123">Application</span></span>                            | <span data-ttu-id="a6c73-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6c73-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6c73-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6c73-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="a6c73-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6c73-126">Request headers</span></span>
| <span data-ttu-id="a6c73-127">Nome</span><span class="sxs-lookup"><span data-stu-id="a6c73-127">Name</span></span>         | <span data-ttu-id="a6c73-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6c73-128">Type</span></span>        | <span data-ttu-id="a6c73-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6c73-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a6c73-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6c73-130">Authorization</span></span> | <span data-ttu-id="a6c73-131">string</span><span class="sxs-lookup"><span data-stu-id="a6c73-131">string</span></span> | <span data-ttu-id="a6c73-132">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="a6c73-132">Bearer \{token\}.</span></span> <span data-ttu-id="a6c73-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6c73-133">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6c73-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6c73-134">Request body</span></span>
<span data-ttu-id="a6c73-135">No corpo da solicitação, fornece uma representação JSON de um objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="a6c73-135">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="a6c73-136">A tabela a seguir mostra as propriedades que são necessárias quando você criar um controle de programa.</span><span class="sxs-lookup"><span data-stu-id="a6c73-136">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="a6c73-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6c73-137">Property</span></span>     | <span data-ttu-id="a6c73-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6c73-138">Type</span></span>        | <span data-ttu-id="a6c73-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6c73-139">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="a6c73-140">O programId do programa esse controle vai se tornar uma parte do.</span><span class="sxs-lookup"><span data-stu-id="a6c73-140">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="a6c73-141">ControlId do controle, em especial o identificador de uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="a6c73-141">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="a6c73-142">O programControlType identifica o tipo de controle do programa - por exemplo, um controle de vinculação para o acesso de convidado analisa.</span><span class="sxs-lookup"><span data-stu-id="a6c73-142">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="a6c73-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6c73-143">Response</span></span>
<span data-ttu-id="a6c73-144">Se tiver êxito, este método retornará um `201, Created` código de resposta e um objeto [programControl](../resources/programcontrol.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6c73-144">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="a6c73-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6c73-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a6c73-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6c73-146">Request</span></span>
<span data-ttu-id="a6c73-147">No corpo da solicitação, fornece uma representação JSON do objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="a6c73-147">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="a6c73-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6c73-148">Response</span></span>
><span data-ttu-id="a6c73-p107">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6c73-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="a6c73-151">Confira também</span><span class="sxs-lookup"><span data-stu-id="a6c73-151">See also</span></span>

| <span data-ttu-id="a6c73-152">Método</span><span class="sxs-lookup"><span data-stu-id="a6c73-152">Method</span></span>           | <span data-ttu-id="a6c73-153">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a6c73-153">Return Type</span></span>    |<span data-ttu-id="a6c73-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6c73-154">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a6c73-155">Lista programControlTypes</span><span class="sxs-lookup"><span data-stu-id="a6c73-155">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="a6c73-156">coleção [programControlType](../resources/programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="a6c73-156">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="a6c73-157">Lista os tipos de controle do programa.</span><span class="sxs-lookup"><span data-stu-id="a6c73-157">List program control types.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
