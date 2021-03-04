---
title: Tipo de recurso programControl
description: No recurso de revisões de acesso do Azure AD, o objeto de controle do programa representa um controle, vinculando uma revisão de acesso a um programa.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 492dc57bfa332472cb7565580ffaa8a5260234c0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443976"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="6e6ec-103">Tipo de recurso programControl</span><span class="sxs-lookup"><span data-stu-id="6e6ec-103">programControl resource type</span></span>

<span data-ttu-id="6e6ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e6ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e6ec-105">No recurso de revisões de acesso do Azure [AD,](accessreviews-root.md) o objeto de controle do programa representa um controle, vinculando uma revisão de acesso a um programa.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="6e6ec-106">Methods</span><span class="sxs-lookup"><span data-stu-id="6e6ec-106">Methods</span></span>

| <span data-ttu-id="6e6ec-107">Método</span><span class="sxs-lookup"><span data-stu-id="6e6ec-107">Method</span></span> | <span data-ttu-id="6e6ec-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6e6ec-108">Return Type</span></span> | <span data-ttu-id="6e6ec-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e6ec-109">Description</span></span> |
|:------ |:----------- |:----------- |
| [<span data-ttu-id="6e6ec-110">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="6e6ec-110">Create programControl</span></span>](../api/programcontrol-create.md) |    [<span data-ttu-id="6e6ec-111">programControl</span><span class="sxs-lookup"><span data-stu-id="6e6ec-111">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="6e6ec-112">Adicione um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-112">Add a programControl to a program.</span></span> |
| [<span data-ttu-id="6e6ec-113">Excluir programControl</span><span class="sxs-lookup"><span data-stu-id="6e6ec-113">Delete programControl</span></span>](../api/programcontrol-delete.md) | <span data-ttu-id="6e6ec-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-114">None.</span></span> | <span data-ttu-id="6e6ec-115">Remova um programControl de um programa.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-115">Remove a programControl from a program.</span></span> |
| [<span data-ttu-id="6e6ec-116">Listar programControls</span><span class="sxs-lookup"><span data-stu-id="6e6ec-116">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="6e6ec-117">[Coleção programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="6e6ec-117">[programControl](programcontrol.md) collection</span></span> | <span data-ttu-id="6e6ec-118">Listar controles em todos os programas no locatário.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-118">List controls across all programs in the tenant.</span></span> |
| [<span data-ttu-id="6e6ec-119">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="6e6ec-119">List programControls of a program</span></span>](../api/program-listcontrols.md) | <span data-ttu-id="6e6ec-120">[Coleção programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="6e6ec-120">[programControl](programcontrol.md) collection</span></span> |    <span data-ttu-id="6e6ec-121">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-121">Get a collection of the controls of a program.</span></span> |
| [<span data-ttu-id="6e6ec-122">Listar programControlTypes</span><span class="sxs-lookup"><span data-stu-id="6e6ec-122">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="6e6ec-123">[Coleção programControlType](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="6e6ec-123">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="6e6ec-124">Listar tipos de controle de programa.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-124">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="6e6ec-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e6ec-125">Properties</span></span>

| <span data-ttu-id="6e6ec-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e6ec-126">Property</span></span> | <span data-ttu-id="6e6ec-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e6ec-127">Type</span></span>   | <span data-ttu-id="6e6ec-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e6ec-128">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="6e6ec-129">id</span><span class="sxs-lookup"><span data-stu-id="6e6ec-129">id</span></span> | <span data-ttu-id="6e6ec-130">String</span><span class="sxs-lookup"><span data-stu-id="6e6ec-130">String</span></span> | <span data-ttu-id="6e6ec-131">O identificador atribuído ao recurso do link entre o programa e o controle.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-131">The feature-assigned identifier of the link between program and control.</span></span> |
| <span data-ttu-id="6e6ec-132">programId</span><span class="sxs-lookup"><span data-stu-id="6e6ec-132">programId</span></span> | <span data-ttu-id="6e6ec-133">String</span><span class="sxs-lookup"><span data-stu-id="6e6ec-133">String</span></span> | <span data-ttu-id="6e6ec-134">O programId do programa do que esse controle faz parte.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-134">The programId of the program this control is a part of.</span></span> <span data-ttu-id="6e6ec-135">Obrigatório durante a criação.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-135">Required on create.</span></span> |
| <span data-ttu-id="6e6ec-136">controlId</span><span class="sxs-lookup"><span data-stu-id="6e6ec-136">controlId</span></span> | <span data-ttu-id="6e6ec-137">String</span><span class="sxs-lookup"><span data-stu-id="6e6ec-137">String</span></span> | <span data-ttu-id="6e6ec-138">ControlId do controle, em particular o identificador de uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-138">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="6e6ec-139">Obrigatório durante a criação.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-139">Required on create.</span></span> |
| <span data-ttu-id="6e6ec-140">controlTypeId</span><span class="sxs-lookup"><span data-stu-id="6e6ec-140">controlTypeId</span></span> | <span data-ttu-id="6e6ec-141">String</span><span class="sxs-lookup"><span data-stu-id="6e6ec-141">String</span></span> | <span data-ttu-id="6e6ec-142">O programControlType identifica o tipo de controle de programa - por exemplo, um controle que vincula a avaliações de acesso de convidados.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-142">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="6e6ec-143">Obrigatório durante a criação.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-143">Required on create.</span></span> |
| <span data-ttu-id="6e6ec-144">displayName</span><span class="sxs-lookup"><span data-stu-id="6e6ec-144">displayName</span></span> | <span data-ttu-id="6e6ec-145">String</span><span class="sxs-lookup"><span data-stu-id="6e6ec-145">String</span></span> | <span data-ttu-id="6e6ec-146">O nome do controle.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-146">The name of the control.</span></span> |
| <span data-ttu-id="6e6ec-147">status</span><span class="sxs-lookup"><span data-stu-id="6e6ec-147">status</span></span> | <span data-ttu-id="6e6ec-148">String</span><span class="sxs-lookup"><span data-stu-id="6e6ec-148">String</span></span> | <span data-ttu-id="6e6ec-149">O status do ciclo de vida do controle.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-149">The life cycle status of the control.</span></span> |
| <span data-ttu-id="6e6ec-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e6ec-150">createdDateTime</span></span> | <span data-ttu-id="6e6ec-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e6ec-151">DateTimeOffset</span></span> | <span data-ttu-id="6e6ec-152">A data e a hora de criação do controle do programa.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-152">The creation date and time of the program control.</span></span> |
| <span data-ttu-id="6e6ec-153">owner</span><span class="sxs-lookup"><span data-stu-id="6e6ec-153">owner</span></span> | [<span data-ttu-id="6e6ec-154">userIdentity</span><span class="sxs-lookup"><span data-stu-id="6e6ec-154">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="6e6ec-155">O usuário que criou o controle do programa.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-155">The user who created the program control.</span></span> |
| <span data-ttu-id="6e6ec-156">recurso</span><span class="sxs-lookup"><span data-stu-id="6e6ec-156">resource</span></span> | [<span data-ttu-id="6e6ec-157">programResource</span><span class="sxs-lookup"><span data-stu-id="6e6ec-157">programResource</span></span>](programresource.md) | <span data-ttu-id="6e6ec-158">O recurso, um grupo ou um aplicativo, direcionado pela revisão de acesso desse controle de programa.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-158">The resource, a group or an app, targeted by this program control's access review.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6e6ec-159">Relações</span><span class="sxs-lookup"><span data-stu-id="6e6ec-159">Relationships</span></span>

| <span data-ttu-id="6e6ec-160">Relação</span><span class="sxs-lookup"><span data-stu-id="6e6ec-160">Relationship</span></span> | <span data-ttu-id="6e6ec-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e6ec-161">Type</span></span>   | <span data-ttu-id="6e6ec-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e6ec-162">Description</span></span> |
|:------------ |:---- |:----------- |
| <span data-ttu-id="6e6ec-163">program</span><span class="sxs-lookup"><span data-stu-id="6e6ec-163">program</span></span> | [<span data-ttu-id="6e6ec-164">program</span><span class="sxs-lookup"><span data-stu-id="6e6ec-164">program</span></span>](program.md) | <span data-ttu-id="6e6ec-165">O programa do que esse controle faz parte.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-165">The program this control is part of.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6e6ec-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e6ec-166">JSON representation</span></span>

<span data-ttu-id="6e6ec-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e6ec-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
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


