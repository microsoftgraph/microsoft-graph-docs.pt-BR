---
title: tipo de recurso de programControl
description: No Windows Azure AD access analisa o recurso, o objeto de controle do programa representa um controle, vinculando uma revisão de acesso a um programa.
localization_priority: Normal
ms.openlocfilehash: 3d9829b8e2585d4deda95551021e2fd9b8d14c7a
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29644004"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="ccaf4-103">tipo de recurso de programControl</span><span class="sxs-lookup"><span data-stu-id="ccaf4-103">programControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccaf4-104">No recurso de [acesso analisa](accessreviews-root.md) Azure AD, o objeto de controle do programa representa um controle, vinculando uma revisão de acesso a um programa.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="ccaf4-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="ccaf4-105">Methods</span></span>

| <span data-ttu-id="ccaf4-106">Método</span><span class="sxs-lookup"><span data-stu-id="ccaf4-106">Method</span></span>           | <span data-ttu-id="ccaf4-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ccaf4-107">Return Type</span></span>    |<span data-ttu-id="ccaf4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccaf4-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ccaf4-109">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="ccaf4-109">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="ccaf4-110">programControl</span><span class="sxs-lookup"><span data-stu-id="ccaf4-110">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="ccaf4-111">Adicione um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-111">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="ccaf4-112">Excluir programControl</span><span class="sxs-lookup"><span data-stu-id="ccaf4-112">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="ccaf4-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-113">None.</span></span>   |   <span data-ttu-id="ccaf4-114">Remova um programControl de um programa.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-114">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="ccaf4-115">Lista programControls</span><span class="sxs-lookup"><span data-stu-id="ccaf4-115">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="ccaf4-116">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="ccaf4-116">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="ccaf4-117">Controles de lista com todos os programas no inquilino.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-117">List controls across all programs in the tenant.</span></span>|

## <a name="permissions"></a><span data-ttu-id="ccaf4-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="ccaf4-118">Permissions</span></span>

|<span data-ttu-id="ccaf4-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ccaf4-119">Permission type</span></span>                        | <span data-ttu-id="ccaf4-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ccaf4-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccaf4-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ccaf4-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="ccaf4-122">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccaf4-122">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="ccaf4-123">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ccaf4-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccaf4-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-124">Not supported.</span></span> |
|<span data-ttu-id="ccaf4-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ccaf4-125">Application</span></span>                            | <span data-ttu-id="ccaf4-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-126">Not supported.</span></span> |

## <a name="properties"></a><span data-ttu-id="ccaf4-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ccaf4-127">Properties</span></span>
| <span data-ttu-id="ccaf4-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ccaf4-128">Property</span></span>     | <span data-ttu-id="ccaf4-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccaf4-129">Type</span></span>   |<span data-ttu-id="ccaf4-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccaf4-130">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="ccaf4-131">O identificador atribuído pelo recurso do vínculo entre o programa e controle</span><span class="sxs-lookup"><span data-stu-id="ccaf4-131">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="ccaf4-132">O programId do programa esse controle é parte do.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-132">The programId of the program this control is a part of.</span></span> <span data-ttu-id="ccaf4-133">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-133">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="ccaf4-134">ControlId do controle, em especial o identificador de uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-134">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="ccaf4-135">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-135">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="ccaf4-136">O programControlType identifica o tipo de controle do programa - por exemplo, um controle de vinculação para o acesso de convidado analisa.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-136">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="ccaf4-137">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-137">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="ccaf4-138">O nome do controle.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-138">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="ccaf4-139">O status do ciclo de vida do controle.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-139">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="ccaf4-140">A data de criação e a hora do controle programa.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-140">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="ccaf4-141">userIdentity</span><span class="sxs-lookup"><span data-stu-id="ccaf4-141">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="ccaf4-142">O usuário que criou o controle de programa.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-142">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="ccaf4-143">O recurso, um grupo ou um aplicativo alvo de revisão de acesso do controle este programa.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-143">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="ccaf4-144">Relações</span><span class="sxs-lookup"><span data-stu-id="ccaf4-144">Relationships</span></span>
| <span data-ttu-id="ccaf4-145">Relação</span><span class="sxs-lookup"><span data-stu-id="ccaf4-145">Relationship</span></span> | <span data-ttu-id="ccaf4-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccaf4-146">Type</span></span>   |<span data-ttu-id="ccaf4-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccaf4-147">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="ccaf4-148">programa</span><span class="sxs-lookup"><span data-stu-id="ccaf4-148">program</span></span>](program.md)               | <span data-ttu-id="ccaf4-149">O programa esse controle faz parte do.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-149">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="ccaf4-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="ccaf4-150">See also</span></span>

| <span data-ttu-id="ccaf4-151">Método</span><span class="sxs-lookup"><span data-stu-id="ccaf4-151">Method</span></span>           | <span data-ttu-id="ccaf4-152">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ccaf4-152">Return Type</span></span>    |<span data-ttu-id="ccaf4-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccaf4-153">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ccaf4-154">Lista programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="ccaf4-154">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="ccaf4-155">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="ccaf4-155">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="ccaf4-156">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-156">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="ccaf4-157">Lista programControlTypes</span><span class="sxs-lookup"><span data-stu-id="ccaf4-157">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="ccaf4-158">coleção [programControlType](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="ccaf4-158">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="ccaf4-159">Lista os tipos de controle do programa.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-159">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ccaf4-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ccaf4-160">JSON representation</span></span>

<span data-ttu-id="ccaf4-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-161">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-programresource-complex-type"></a><span data-ttu-id="ccaf4-162">O tipo de programResource complexo</span><span class="sxs-lookup"><span data-stu-id="ccaf4-162">The programResource complex type</span></span>

<span data-ttu-id="ccaf4-163">O recurso de programa, contido em um objeto de controle de programa, é uma representação de uma referência a um objeto que é o destino da revisão acesso.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-163">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="ccaf4-164">Esse tipo de herda de `microsoft.graph.identity` e tem uma propriedade adicional:</span><span class="sxs-lookup"><span data-stu-id="ccaf4-164">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="ccaf4-165">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ccaf4-165">Property</span></span>     | <span data-ttu-id="ccaf4-166">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccaf4-166">Type</span></span>   |<span data-ttu-id="ccaf4-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccaf4-167">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="ccaf4-168">Tipo de recurso, indicando se ele é um grupo ou um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ccaf4-168">Type of the resource, indicating whether it is a group or an app.</span></span> |     


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
