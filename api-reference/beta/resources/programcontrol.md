---
title: tipo de recurso programControl
description: No recurso de revisões do Azure AD Access, o objeto de controle do programa representa um controle, vinculando uma revisão do Access a um programa.
localization_priority: Normal
ms.openlocfilehash: 7d194f3e80f44eb57be0deb7d2ffd71624c385d7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344004"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="5add7-103">tipo de recurso programControl</span><span class="sxs-lookup"><span data-stu-id="5add7-103">programControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5add7-104">No recurso de revisões do Azure AD [Access](accessreviews-root.md) , o objeto de controle do programa representa um controle, vinculando uma revisão do Access a um programa.</span><span class="sxs-lookup"><span data-stu-id="5add7-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="5add7-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="5add7-105">Methods</span></span>

| <span data-ttu-id="5add7-106">Método</span><span class="sxs-lookup"><span data-stu-id="5add7-106">Method</span></span>           | <span data-ttu-id="5add7-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5add7-107">Return Type</span></span>    |<span data-ttu-id="5add7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5add7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5add7-109">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="5add7-109">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="5add7-110">programControl</span><span class="sxs-lookup"><span data-stu-id="5add7-110">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="5add7-111">Adicionar um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="5add7-111">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="5add7-112">Excluir programControl</span><span class="sxs-lookup"><span data-stu-id="5add7-112">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="5add7-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5add7-113">None.</span></span>   |   <span data-ttu-id="5add7-114">Remover um programControl de um programa.</span><span class="sxs-lookup"><span data-stu-id="5add7-114">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="5add7-115">Listar programControls</span><span class="sxs-lookup"><span data-stu-id="5add7-115">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="5add7-116">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="5add7-116">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="5add7-117">Listar controles em todos os programas no locatário.</span><span class="sxs-lookup"><span data-stu-id="5add7-117">List controls across all programs in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="5add7-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5add7-118">Properties</span></span>
| <span data-ttu-id="5add7-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5add7-119">Property</span></span>     | <span data-ttu-id="5add7-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="5add7-120">Type</span></span>   |<span data-ttu-id="5add7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5add7-121">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="5add7-122">O identificador atribuído ao recurso do link entre o programa e o controle</span><span class="sxs-lookup"><span data-stu-id="5add7-122">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="5add7-123">O ProgramId do programa do qual esse controle faz parte.</span><span class="sxs-lookup"><span data-stu-id="5add7-123">The programId of the program this control is a part of.</span></span> <span data-ttu-id="5add7-124">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="5add7-124">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="5add7-125">O controlId do controle, em particular, o identificador de uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="5add7-125">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="5add7-126">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="5add7-126">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="5add7-127">O programControlType identifica o tipo de controle de programa-por exemplo, um controle vinculando a revisões de acesso de convidados.</span><span class="sxs-lookup"><span data-stu-id="5add7-127">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="5add7-128">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="5add7-128">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="5add7-129">O nome do controle.</span><span class="sxs-lookup"><span data-stu-id="5add7-129">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="5add7-130">O status do ciclo de vida do controle.</span><span class="sxs-lookup"><span data-stu-id="5add7-130">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="5add7-131">A data e hora de criação do controle de programa.</span><span class="sxs-lookup"><span data-stu-id="5add7-131">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="5add7-132">userIdentity</span><span class="sxs-lookup"><span data-stu-id="5add7-132">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="5add7-133">O usuário que criou o controle de programa.</span><span class="sxs-lookup"><span data-stu-id="5add7-133">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="5add7-134">O recurso, um grupo ou um aplicativo, direcionado por essa revisão de acesso de controle de programa.</span><span class="sxs-lookup"><span data-stu-id="5add7-134">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="5add7-135">Relações</span><span class="sxs-lookup"><span data-stu-id="5add7-135">Relationships</span></span>
| <span data-ttu-id="5add7-136">Relação</span><span class="sxs-lookup"><span data-stu-id="5add7-136">Relationship</span></span> | <span data-ttu-id="5add7-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="5add7-137">Type</span></span>   |<span data-ttu-id="5add7-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="5add7-138">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="5add7-139">programa</span><span class="sxs-lookup"><span data-stu-id="5add7-139">program</span></span>](program.md)               | <span data-ttu-id="5add7-140">O programa do qual esse controle faz parte.</span><span class="sxs-lookup"><span data-stu-id="5add7-140">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="5add7-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="5add7-141">See also</span></span>

| <span data-ttu-id="5add7-142">Método</span><span class="sxs-lookup"><span data-stu-id="5add7-142">Method</span></span>           | <span data-ttu-id="5add7-143">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5add7-143">Return Type</span></span>    |<span data-ttu-id="5add7-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="5add7-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5add7-145">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="5add7-145">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="5add7-146">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="5add7-146">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="5add7-147">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="5add7-147">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="5add7-148">Listar programControlTypes</span><span class="sxs-lookup"><span data-stu-id="5add7-148">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="5add7-149">coleção [programControlType](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="5add7-149">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="5add7-150">Listar tipos de controle de programa.</span><span class="sxs-lookup"><span data-stu-id="5add7-150">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5add7-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5add7-151">JSON representation</span></span>

<span data-ttu-id="5add7-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5add7-152">Here is a JSON representation of the resource.</span></span>

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
 "owner": {"@odata.type":"microsoft.graph.userIdentity"},
 "resource":{"@odata.type":"microsoft.graph.programResource"}
}

```

## <a name="the-programresource-complex-type"></a><span data-ttu-id="5add7-153">O tipo complexo programResource</span><span class="sxs-lookup"><span data-stu-id="5add7-153">The programResource complex type</span></span>

<span data-ttu-id="5add7-154">O recurso de programa, contido em um objeto de controle de programa, é uma representação de uma referência a um objeto que é o destino da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="5add7-154">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="5add7-155">Este tipo herda de `microsoft.graph.identity` e tem uma propriedade adicional:</span><span class="sxs-lookup"><span data-stu-id="5add7-155">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="5add7-156">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5add7-156">Property</span></span>     | <span data-ttu-id="5add7-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="5add7-157">Type</span></span>   |<span data-ttu-id="5add7-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="5add7-158">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="5add7-159">Tipo do recurso, indicando se é um grupo ou um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5add7-159">Type of the resource, indicating whether it is a group or an app.</span></span> |     

## <a name="json-representation"></a><span data-ttu-id="5add7-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5add7-160">JSON representation</span></span>

<span data-ttu-id="5add7-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5add7-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programResource"
}-->

```json
{
 "type": "string"
}

```
<!--
{
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
