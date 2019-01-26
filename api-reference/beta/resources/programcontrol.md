---
title: tipo de recurso de programControl
description: No Windows Azure AD access analisa o recurso, o objeto de controle do programa representa um controle, vinculando uma revisão de acesso a um programa.
localization_priority: Normal
ms.openlocfilehash: 82d9263a909fb11e688ffa6b27f0cf92601ae9e9
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576553"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="8586a-103">tipo de recurso de programControl</span><span class="sxs-lookup"><span data-stu-id="8586a-103">programControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8586a-104">No recurso de [acesso analisa](accessreviews-root.md) Azure AD, o objeto de controle do programa representa um controle, vinculando uma revisão de acesso a um programa.</span><span class="sxs-lookup"><span data-stu-id="8586a-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="8586a-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="8586a-105">Methods</span></span>

| <span data-ttu-id="8586a-106">Método</span><span class="sxs-lookup"><span data-stu-id="8586a-106">Method</span></span>           | <span data-ttu-id="8586a-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8586a-107">Return Type</span></span>    |<span data-ttu-id="8586a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8586a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8586a-109">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="8586a-109">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="8586a-110">programControl</span><span class="sxs-lookup"><span data-stu-id="8586a-110">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="8586a-111">Adicione um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="8586a-111">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="8586a-112">Excluir programControl</span><span class="sxs-lookup"><span data-stu-id="8586a-112">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="8586a-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8586a-113">None.</span></span>   |   <span data-ttu-id="8586a-114">Remova um programControl de um programa.</span><span class="sxs-lookup"><span data-stu-id="8586a-114">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="8586a-115">Lista programControls</span><span class="sxs-lookup"><span data-stu-id="8586a-115">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="8586a-116">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="8586a-116">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="8586a-117">Controles de lista com todos os programas no inquilino.</span><span class="sxs-lookup"><span data-stu-id="8586a-117">List controls across all programs in the tenant.</span></span>|

## <a name="permissions"></a><span data-ttu-id="8586a-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="8586a-118">Permissions</span></span>

|<span data-ttu-id="8586a-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8586a-119">Permission type</span></span>                        | <span data-ttu-id="8586a-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8586a-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8586a-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8586a-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="8586a-122">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8586a-122">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="8586a-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8586a-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8586a-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8586a-124">Not supported.</span></span> |
|<span data-ttu-id="8586a-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8586a-125">Application</span></span>                            | <span data-ttu-id="8586a-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8586a-126">Not supported.</span></span> |

## <a name="properties"></a><span data-ttu-id="8586a-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8586a-127">Properties</span></span>
| <span data-ttu-id="8586a-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8586a-128">Property</span></span>     | <span data-ttu-id="8586a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8586a-129">Type</span></span>   |<span data-ttu-id="8586a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8586a-130">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="8586a-131">O identificador atribuído pelo recurso do vínculo entre o programa e controle</span><span class="sxs-lookup"><span data-stu-id="8586a-131">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="8586a-132">O programId do programa esse controle é parte do.</span><span class="sxs-lookup"><span data-stu-id="8586a-132">The programId of the program this control is a part of.</span></span> <span data-ttu-id="8586a-133">Necessários na criação.</span><span class="sxs-lookup"><span data-stu-id="8586a-133">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="8586a-134">ControlId do controle, em especial o identificador de uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="8586a-134">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="8586a-135">Necessários na criação.</span><span class="sxs-lookup"><span data-stu-id="8586a-135">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="8586a-136">O programControlType identifica o tipo de controle do programa - por exemplo, um controle de vinculação para o acesso de convidado analisa.</span><span class="sxs-lookup"><span data-stu-id="8586a-136">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="8586a-137">Necessários na criação.</span><span class="sxs-lookup"><span data-stu-id="8586a-137">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="8586a-138">O nome do controle.</span><span class="sxs-lookup"><span data-stu-id="8586a-138">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="8586a-139">O status do ciclo de vida do controle.</span><span class="sxs-lookup"><span data-stu-id="8586a-139">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="8586a-140">A data de criação e a hora do controle programa.</span><span class="sxs-lookup"><span data-stu-id="8586a-140">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="8586a-141">userIdentity</span><span class="sxs-lookup"><span data-stu-id="8586a-141">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="8586a-142">O usuário que criou o controle de programa.</span><span class="sxs-lookup"><span data-stu-id="8586a-142">The user who created the program control.</span></span>                                               |
| `resource`               | [<span data-ttu-id="8586a-143">programResource</span><span class="sxs-lookup"><span data-stu-id="8586a-143">programResource</span></span>](programresource.md)       | <span data-ttu-id="8586a-144">O recurso, um grupo ou um aplicativo alvo de revisão de acesso do controle este programa.</span><span class="sxs-lookup"><span data-stu-id="8586a-144">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="8586a-145">Relações</span><span class="sxs-lookup"><span data-stu-id="8586a-145">Relationships</span></span>
| <span data-ttu-id="8586a-146">Relação</span><span class="sxs-lookup"><span data-stu-id="8586a-146">Relationship</span></span> | <span data-ttu-id="8586a-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="8586a-147">Type</span></span>   |<span data-ttu-id="8586a-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="8586a-148">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="8586a-149">programa</span><span class="sxs-lookup"><span data-stu-id="8586a-149">program</span></span>](program.md)               | <span data-ttu-id="8586a-150">O programa esse controle faz parte do.</span><span class="sxs-lookup"><span data-stu-id="8586a-150">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="8586a-151">Confira também</span><span class="sxs-lookup"><span data-stu-id="8586a-151">See also</span></span>

| <span data-ttu-id="8586a-152">Método</span><span class="sxs-lookup"><span data-stu-id="8586a-152">Method</span></span>           | <span data-ttu-id="8586a-153">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8586a-153">Return Type</span></span>    |<span data-ttu-id="8586a-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="8586a-154">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8586a-155">Lista programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="8586a-155">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="8586a-156">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="8586a-156">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="8586a-157">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="8586a-157">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="8586a-158">Lista programControlTypes</span><span class="sxs-lookup"><span data-stu-id="8586a-158">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="8586a-159">coleção [programControlType](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="8586a-159">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="8586a-160">Lista os tipos de controle do programa.</span><span class="sxs-lookup"><span data-stu-id="8586a-160">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8586a-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8586a-161">JSON representation</span></span>

<span data-ttu-id="8586a-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8586a-162">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControl"
}-->

```json
{
 "id": "string (identifier)",
 "programId": "string (identifier)",
 "controlId": "string (identifier)",
 "controlTypeId": "string (identifier)",
 "displayName": "string",
 "status": "string",
 "createdDateTime": "string (timestamp)",
 "owner": "microsoft.graph.userIdentity",
 "resource":"microsoft.graph.programResource"
}

```

## <a name="the-programresource-complex-type"></a><span data-ttu-id="8586a-163">O tipo de programResource complexo</span><span class="sxs-lookup"><span data-stu-id="8586a-163">The programResource complex type</span></span>

<span data-ttu-id="8586a-164">O recurso de programa, contido em um objeto de controle de programa, é uma representação de uma referência a um objeto que é o destino da revisão acesso.</span><span class="sxs-lookup"><span data-stu-id="8586a-164">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="8586a-165">Esse tipo de herda de `microsoft.graph.identity` e tem uma propriedade adicional:</span><span class="sxs-lookup"><span data-stu-id="8586a-165">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="8586a-166">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8586a-166">Property</span></span>     | <span data-ttu-id="8586a-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="8586a-167">Type</span></span>   |<span data-ttu-id="8586a-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="8586a-168">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="8586a-169">Tipo de recurso, indicando se ele é um grupo ou um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8586a-169">Type of the resource, indicating whether it is a group or an app.</span></span> |     


<!--
{
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/programcontrol.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
