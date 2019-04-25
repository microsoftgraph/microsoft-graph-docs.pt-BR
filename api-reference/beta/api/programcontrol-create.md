---
title: Criar programControl
description: No recurso de revisões do Azure AD Access, crie um novo objeto programControl.  Isso vincula uma revisão do Access a um programa.
localization_priority: Normal
ms.openlocfilehash: 89e31994ea91dba68e2f4563c64eeab53dd4db93
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546418"
---
# <a name="create-programcontrol"></a><span data-ttu-id="8d9d8-104">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="8d9d8-104">Create programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d9d8-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , crie um novo objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="8d9d8-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="8d9d8-106">Isso vincula uma revisão do Access a um programa.</span><span class="sxs-lookup"><span data-stu-id="8d9d8-106">This links an access review to a program.</span></span>

<span data-ttu-id="8d9d8-107">Antes de fazer essa solicitação, o chamador deve ter sido</span><span class="sxs-lookup"><span data-stu-id="8d9d8-107">Prior to making this request, the caller must have previously</span></span>

 - <span data-ttu-id="8d9d8-108">[criou um programa](program-create.md) ou [recuperou um programa](program-list.md), para que o valor `programId` de a ser incluído na solicitação,</span><span class="sxs-lookup"><span data-stu-id="8d9d8-108">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
 - <span data-ttu-id="8d9d8-109">[criou uma revisão do Access](accessreview-create.md) ou [recuperou uma revisão do Access](accessreview-get.md), para que `controlId` o valor de seja incluído na solicitação e</span><span class="sxs-lookup"><span data-stu-id="8d9d8-109">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
 - <span data-ttu-id="8d9d8-110">[recuperada a lista de tipos de controle de programa](programcontroltype-list.md)para que o `controlTypeId` valor de seja incluído na solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d9d8-110">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="8d9d8-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d9d8-111">Permissions</span></span>
<span data-ttu-id="8d9d8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d9d8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d9d8-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d9d8-114">Permission type</span></span>                        | <span data-ttu-id="8d9d8-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d9d8-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d9d8-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d9d8-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d9d8-117">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="8d9d8-117"></span></span>  <span data-ttu-id="8d9d8-118">O usuário conectado também deve estar em uma função de diretório que permite que eles criem um programControl.</span><span class="sxs-lookup"><span data-stu-id="8d9d8-118">The signed in user must also be in a directory role which permits them to create a programControl.</span></span> |
|<span data-ttu-id="8d9d8-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d9d8-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d9d8-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d9d8-120">Not supported.</span></span> |
|<span data-ttu-id="8d9d8-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d9d8-121">Application</span></span>                            | <span data-ttu-id="8d9d8-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d9d8-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d9d8-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d9d8-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="8d9d8-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d9d8-124">Request headers</span></span>
| <span data-ttu-id="8d9d8-125">Nome</span><span class="sxs-lookup"><span data-stu-id="8d9d8-125">Name</span></span>         | <span data-ttu-id="8d9d8-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d9d8-126">Type</span></span>        | <span data-ttu-id="8d9d8-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d9d8-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8d9d8-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d9d8-128">Authorization</span></span> | <span data-ttu-id="8d9d8-129">string</span><span class="sxs-lookup"><span data-stu-id="8d9d8-129">string</span></span> | <span data-ttu-id="8d9d8-p105">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d9d8-p105">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d9d8-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d9d8-132">Request body</span></span>
<span data-ttu-id="8d9d8-133">No corpo da solicitação, forneça uma representação JSON de um objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="8d9d8-133">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="8d9d8-134">A tabela a seguir mostra as propriedades que são necessárias ao criar um controle de programa.</span><span class="sxs-lookup"><span data-stu-id="8d9d8-134">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="8d9d8-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d9d8-135">Property</span></span>     | <span data-ttu-id="8d9d8-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d9d8-136">Type</span></span>        | <span data-ttu-id="8d9d8-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d9d8-137">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="8d9d8-138">O ProgramId do programa para o qual esse controle se tornará parte.</span><span class="sxs-lookup"><span data-stu-id="8d9d8-138">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="8d9d8-139">O controlId do controle, em particular, o identificador de uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="8d9d8-139">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="8d9d8-140">O programControlType identifica o tipo de controle de programa-por exemplo, um controle vinculando a revisões de acesso de convidados.</span><span class="sxs-lookup"><span data-stu-id="8d9d8-140">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="8d9d8-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d9d8-141">Response</span></span>
<span data-ttu-id="8d9d8-142">Se tiver êxito, este método retornará `201, Created` um código de resposta e um objeto [programControl](../resources/programcontrol.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d9d8-142">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="8d9d8-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d9d8-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d9d8-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d9d8-144">Request</span></span>
<span data-ttu-id="8d9d8-145">No corpo da solicitação, forneça uma representação JSON do objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="8d9d8-145">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="8d9d8-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d9d8-146">Response</span></span>
><span data-ttu-id="8d9d8-p106">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d9d8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="8d9d8-149">Confira também</span><span class="sxs-lookup"><span data-stu-id="8d9d8-149">See also</span></span>

| <span data-ttu-id="8d9d8-150">Método</span><span class="sxs-lookup"><span data-stu-id="8d9d8-150">Method</span></span>           | <span data-ttu-id="8d9d8-151">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8d9d8-151">Return Type</span></span>    |<span data-ttu-id="8d9d8-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d9d8-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8d9d8-153">Listar programControlTypes</span><span class="sxs-lookup"><span data-stu-id="8d9d8-153">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="8d9d8-154">coleção [programControlType](../resources/programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="8d9d8-154">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="8d9d8-155">Listar tipos de controle de programa.</span><span class="sxs-lookup"><span data-stu-id="8d9d8-155">List program control types.</span></span> |


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
