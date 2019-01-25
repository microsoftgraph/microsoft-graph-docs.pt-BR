---
title: Criar programControl
description: No Windows Azure AD para acessar o recurso de revisões, crie um novo objeto programControl.  Isso vincula uma revisão de acesso a um programa.
localization_priority: Normal
ms.openlocfilehash: 89e31994ea91dba68e2f4563c64eeab53dd4db93
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511111"
---
# <a name="create-programcontrol"></a><span data-ttu-id="d0944-104">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="d0944-104">Create programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0944-105">O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, cria um novo objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="d0944-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="d0944-106">Isso vincula uma revisão de acesso a um programa.</span><span class="sxs-lookup"><span data-stu-id="d0944-106">This links an access review to a program.</span></span>

<span data-ttu-id="d0944-107">Antes de fazer essa solicitação, o chamador deve ter anteriormente</span><span class="sxs-lookup"><span data-stu-id="d0944-107">Prior to making this request, the caller must have previously</span></span>

 - <span data-ttu-id="d0944-108">[criado um programa](program-create.md) ou [recuperados de um programa](program-list.md), para que o valor de `programId` para incluir na solicitação,</span><span class="sxs-lookup"><span data-stu-id="d0944-108">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
 - <span data-ttu-id="d0944-109">[criada uma revisão de acesso](accessreview-create.md) ou [recuperado uma revisão de acesso](accessreview-get.md), para que o valor de `controlId` para incluir na solicitação, e</span><span class="sxs-lookup"><span data-stu-id="d0944-109">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
 - <span data-ttu-id="d0944-110">[recuperou a lista de tipos de controle de programas](programcontroltype-list.md), para que o valor de `controlTypeId` para incluir na solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0944-110">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="d0944-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0944-111">Permissions</span></span>
<span data-ttu-id="d0944-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0944-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0944-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0944-114">Permission type</span></span>                        | <span data-ttu-id="d0944-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0944-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0944-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0944-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="d0944-117">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="d0944-117"></span></span>  <span data-ttu-id="d0944-118">O usuário conectado também deve ser uma função de diretório que permite a atualização-los para criar um programControl.</span><span class="sxs-lookup"><span data-stu-id="d0944-118">The signed in user must also be in a directory role which permits them to create a programControl.</span></span> |
|<span data-ttu-id="d0944-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0944-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0944-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0944-120">Not supported.</span></span> |
|<span data-ttu-id="d0944-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0944-121">Application</span></span>                            | <span data-ttu-id="d0944-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0944-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0944-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0944-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="d0944-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0944-124">Request headers</span></span>
| <span data-ttu-id="d0944-125">Nome</span><span class="sxs-lookup"><span data-stu-id="d0944-125">Name</span></span>         | <span data-ttu-id="d0944-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0944-126">Type</span></span>        | <span data-ttu-id="d0944-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0944-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d0944-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0944-128">Authorization</span></span> | <span data-ttu-id="d0944-129">string</span><span class="sxs-lookup"><span data-stu-id="d0944-129">string</span></span> | <span data-ttu-id="d0944-130">Token de portador</span><span class="sxs-lookup"><span data-stu-id="d0944-130">Bearer \{token\}.</span></span> <span data-ttu-id="d0944-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0944-131">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0944-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0944-132">Request body</span></span>
<span data-ttu-id="d0944-133">No corpo da solicitação, fornece uma representação JSON de um objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="d0944-133">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="d0944-134">A tabela a seguir mostra as propriedades que são necessárias quando você criar um controle de programa.</span><span class="sxs-lookup"><span data-stu-id="d0944-134">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="d0944-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0944-135">Property</span></span>     | <span data-ttu-id="d0944-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0944-136">Type</span></span>        | <span data-ttu-id="d0944-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0944-137">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="d0944-138">O programId do programa esse controle vai se tornar uma parte do.</span><span class="sxs-lookup"><span data-stu-id="d0944-138">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="d0944-139">ControlId do controle, em especial o identificador de uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="d0944-139">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="d0944-140">O programControlType identifica o tipo de controle do programa - por exemplo, um controle de vinculação para o acesso de convidado analisa.</span><span class="sxs-lookup"><span data-stu-id="d0944-140">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="d0944-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0944-141">Response</span></span>
<span data-ttu-id="d0944-142">Se tiver êxito, este método retornará um `201, Created` código de resposta e um objeto [programControl](../resources/programcontrol.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0944-142">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="d0944-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0944-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0944-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0944-144">Request</span></span>
<span data-ttu-id="d0944-145">No corpo da solicitação, fornece uma representação JSON do objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="d0944-145">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="d0944-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0944-146">Response</span></span>
><span data-ttu-id="d0944-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0944-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d0944-149">Confira também</span><span class="sxs-lookup"><span data-stu-id="d0944-149">See also</span></span>

| <span data-ttu-id="d0944-150">Método</span><span class="sxs-lookup"><span data-stu-id="d0944-150">Method</span></span>           | <span data-ttu-id="d0944-151">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d0944-151">Return Type</span></span>    |<span data-ttu-id="d0944-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0944-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d0944-153">Lista programControlTypes</span><span class="sxs-lookup"><span data-stu-id="d0944-153">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="d0944-154">coleção [programControlType](../resources/programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="d0944-154">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="d0944-155">Lista os tipos de controle do programa.</span><span class="sxs-lookup"><span data-stu-id="d0944-155">List program control types.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
