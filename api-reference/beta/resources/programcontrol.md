---
title: tipo de recurso programControl
description: No recurso de revisões do Azure AD Access, o objeto de controle do programa representa um controle, vinculando uma revisão do Access a um programa.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ee374108cdebca2e6ae06ee18a245f5c9eeebf74
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521443"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="0bed3-103">tipo de recurso programControl</span><span class="sxs-lookup"><span data-stu-id="0bed3-103">programControl resource type</span></span>

<span data-ttu-id="0bed3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0bed3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bed3-105">No recurso de revisões do Azure AD [Access](accessreviews-root.md) , o objeto de controle do programa representa um controle, vinculando uma revisão do Access a um programa.</span><span class="sxs-lookup"><span data-stu-id="0bed3-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="0bed3-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="0bed3-106">Methods</span></span>

| <span data-ttu-id="0bed3-107">Método</span><span class="sxs-lookup"><span data-stu-id="0bed3-107">Method</span></span>           | <span data-ttu-id="0bed3-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0bed3-108">Return Type</span></span>    |<span data-ttu-id="0bed3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bed3-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0bed3-110">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="0bed3-110">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="0bed3-111">programControl</span><span class="sxs-lookup"><span data-stu-id="0bed3-111">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="0bed3-112">Adicionar um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="0bed3-112">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="0bed3-113">Excluir programControl</span><span class="sxs-lookup"><span data-stu-id="0bed3-113">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="0bed3-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0bed3-114">None.</span></span>   |   <span data-ttu-id="0bed3-115">Remover um programControl de um programa.</span><span class="sxs-lookup"><span data-stu-id="0bed3-115">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="0bed3-116">Listar programControls</span><span class="sxs-lookup"><span data-stu-id="0bed3-116">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="0bed3-117">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="0bed3-117">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="0bed3-118">Listar controles em todos os programas no locatário.</span><span class="sxs-lookup"><span data-stu-id="0bed3-118">List controls across all programs in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="0bed3-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0bed3-119">Properties</span></span>
| <span data-ttu-id="0bed3-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bed3-120">Property</span></span>     | <span data-ttu-id="0bed3-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bed3-121">Type</span></span>   |<span data-ttu-id="0bed3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bed3-122">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="0bed3-123">O identificador atribuído ao recurso do link entre o programa e o controle</span><span class="sxs-lookup"><span data-stu-id="0bed3-123">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="0bed3-124">O ProgramId do programa do qual esse controle faz parte.</span><span class="sxs-lookup"><span data-stu-id="0bed3-124">The programId of the program this control is a part of.</span></span> <span data-ttu-id="0bed3-125">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="0bed3-125">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="0bed3-126">O controlId do controle, em particular, o identificador de uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="0bed3-126">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="0bed3-127">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="0bed3-127">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="0bed3-128">O programControlType identifica o tipo de controle de programa-por exemplo, um controle vinculando a revisões de acesso de convidados.</span><span class="sxs-lookup"><span data-stu-id="0bed3-128">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="0bed3-129">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="0bed3-129">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="0bed3-130">O nome do controle.</span><span class="sxs-lookup"><span data-stu-id="0bed3-130">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="0bed3-131">O status do ciclo de vida do controle.</span><span class="sxs-lookup"><span data-stu-id="0bed3-131">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="0bed3-132">A data e hora de criação do controle de programa.</span><span class="sxs-lookup"><span data-stu-id="0bed3-132">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="0bed3-133">userIdentity</span><span class="sxs-lookup"><span data-stu-id="0bed3-133">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="0bed3-134">O usuário que criou o controle de programa.</span><span class="sxs-lookup"><span data-stu-id="0bed3-134">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="0bed3-135">O recurso, um grupo ou um aplicativo, direcionado por essa revisão de acesso de controle de programa.</span><span class="sxs-lookup"><span data-stu-id="0bed3-135">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="0bed3-136">Relações</span><span class="sxs-lookup"><span data-stu-id="0bed3-136">Relationships</span></span>
| <span data-ttu-id="0bed3-137">Relação</span><span class="sxs-lookup"><span data-stu-id="0bed3-137">Relationship</span></span> | <span data-ttu-id="0bed3-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bed3-138">Type</span></span>   |<span data-ttu-id="0bed3-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bed3-139">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="0bed3-140">programa</span><span class="sxs-lookup"><span data-stu-id="0bed3-140">program</span></span>](program.md)               | <span data-ttu-id="0bed3-141">O programa do qual esse controle faz parte.</span><span class="sxs-lookup"><span data-stu-id="0bed3-141">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="0bed3-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="0bed3-142">See also</span></span>

| <span data-ttu-id="0bed3-143">Método</span><span class="sxs-lookup"><span data-stu-id="0bed3-143">Method</span></span>           | <span data-ttu-id="0bed3-144">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0bed3-144">Return Type</span></span>    |<span data-ttu-id="0bed3-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bed3-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0bed3-146">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="0bed3-146">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="0bed3-147">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="0bed3-147">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="0bed3-148">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="0bed3-148">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="0bed3-149">Listar programControlTypes</span><span class="sxs-lookup"><span data-stu-id="0bed3-149">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="0bed3-150">coleção [programControlType](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="0bed3-150">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="0bed3-151">Listar tipos de controle de programa.</span><span class="sxs-lookup"><span data-stu-id="0bed3-151">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0bed3-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0bed3-152">JSON representation</span></span>

<span data-ttu-id="0bed3-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0bed3-153">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-programresource-complex-type"></a><span data-ttu-id="0bed3-154">O tipo complexo programResource</span><span class="sxs-lookup"><span data-stu-id="0bed3-154">The programResource complex type</span></span>

<span data-ttu-id="0bed3-155">O recurso de programa, contido em um objeto de controle de programa, é uma representação de uma referência a um objeto que é o destino da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="0bed3-155">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="0bed3-156">Este tipo herda de `microsoft.graph.identity` e tem uma propriedade adicional:</span><span class="sxs-lookup"><span data-stu-id="0bed3-156">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="0bed3-157">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bed3-157">Property</span></span>     | <span data-ttu-id="0bed3-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bed3-158">Type</span></span>   |<span data-ttu-id="0bed3-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bed3-159">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="0bed3-160">Tipo do recurso, indicando se é um grupo ou um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0bed3-160">Type of the resource, indicating whether it is a group or an app.</span></span> |     

## <a name="json-representation"></a><span data-ttu-id="0bed3-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0bed3-161">JSON representation</span></span>

<span data-ttu-id="0bed3-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0bed3-162">Here is a JSON representation of the resource.</span></span>

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
