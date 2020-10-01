---
title: tipo de recurso programControl
description: No recurso de revisões do Azure AD Access, o objeto de controle do programa representa um controle, vinculando uma revisão do Access a um programa.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 9837f160015dedb0f37cce65b8209ff9a6ec5331
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330159"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="bacb9-103">tipo de recurso programControl</span><span class="sxs-lookup"><span data-stu-id="bacb9-103">programControl resource type</span></span>

<span data-ttu-id="bacb9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bacb9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bacb9-105">No recurso de revisões do Azure AD [Access](accessreviews-root.md) , o objeto de controle do programa representa um controle, vinculando uma revisão do Access a um programa.</span><span class="sxs-lookup"><span data-stu-id="bacb9-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="bacb9-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="bacb9-106">Methods</span></span>

| <span data-ttu-id="bacb9-107">Método</span><span class="sxs-lookup"><span data-stu-id="bacb9-107">Method</span></span> | <span data-ttu-id="bacb9-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bacb9-108">Return Type</span></span> | <span data-ttu-id="bacb9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bacb9-109">Description</span></span> |
|:------ |:----------- |:----------- |
| [<span data-ttu-id="bacb9-110">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="bacb9-110">Create programControl</span></span>](../api/programcontrol-create.md) |    [<span data-ttu-id="bacb9-111">programControl</span><span class="sxs-lookup"><span data-stu-id="bacb9-111">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="bacb9-112">Adicionar um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="bacb9-112">Add a programControl to a program.</span></span> |
| [<span data-ttu-id="bacb9-113">Excluir programControl</span><span class="sxs-lookup"><span data-stu-id="bacb9-113">Delete programControl</span></span>](../api/programcontrol-delete.md) | <span data-ttu-id="bacb9-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bacb9-114">None.</span></span> | <span data-ttu-id="bacb9-115">Remover um programControl de um programa.</span><span class="sxs-lookup"><span data-stu-id="bacb9-115">Remove a programControl from a program.</span></span> |
| [<span data-ttu-id="bacb9-116">Listar programControls</span><span class="sxs-lookup"><span data-stu-id="bacb9-116">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="bacb9-117">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="bacb9-117">[programControl](programcontrol.md) collection</span></span> | <span data-ttu-id="bacb9-118">Listar controles em todos os programas no locatário.</span><span class="sxs-lookup"><span data-stu-id="bacb9-118">List controls across all programs in the tenant.</span></span> |
| [<span data-ttu-id="bacb9-119">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="bacb9-119">List programControls of a program</span></span>](../api/program-listcontrols.md) | <span data-ttu-id="bacb9-120">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="bacb9-120">[programControl](programcontrol.md) collection</span></span> |    <span data-ttu-id="bacb9-121">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="bacb9-121">Get a collection of the controls of a program.</span></span> |
| [<span data-ttu-id="bacb9-122">Listar programControlTypes</span><span class="sxs-lookup"><span data-stu-id="bacb9-122">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="bacb9-123">coleção [programControlType](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="bacb9-123">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="bacb9-124">Listar tipos de controle de programa.</span><span class="sxs-lookup"><span data-stu-id="bacb9-124">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="bacb9-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bacb9-125">Properties</span></span>

| <span data-ttu-id="bacb9-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bacb9-126">Property</span></span> | <span data-ttu-id="bacb9-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="bacb9-127">Type</span></span>   | <span data-ttu-id="bacb9-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="bacb9-128">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="bacb9-129">id</span><span class="sxs-lookup"><span data-stu-id="bacb9-129">id</span></span> | <span data-ttu-id="bacb9-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bacb9-130">String</span></span> | <span data-ttu-id="bacb9-131">O identificador atribuído ao recurso do link entre o programa e o controle.</span><span class="sxs-lookup"><span data-stu-id="bacb9-131">The feature-assigned identifier of the link between program and control.</span></span> |
| <span data-ttu-id="bacb9-132">ProgramId</span><span class="sxs-lookup"><span data-stu-id="bacb9-132">programId</span></span> | <span data-ttu-id="bacb9-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bacb9-133">String</span></span> | <span data-ttu-id="bacb9-134">O ProgramId do programa do qual esse controle faz parte.</span><span class="sxs-lookup"><span data-stu-id="bacb9-134">The programId of the program this control is a part of.</span></span> <span data-ttu-id="bacb9-135">Obrigatório durante a criação.</span><span class="sxs-lookup"><span data-stu-id="bacb9-135">Required on create.</span></span> |
| <span data-ttu-id="bacb9-136">controlId</span><span class="sxs-lookup"><span data-stu-id="bacb9-136">controlId</span></span> | <span data-ttu-id="bacb9-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bacb9-137">String</span></span> | <span data-ttu-id="bacb9-138">O controlId do controle, em particular, o identificador de uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="bacb9-138">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="bacb9-139">Obrigatório durante a criação.</span><span class="sxs-lookup"><span data-stu-id="bacb9-139">Required on create.</span></span> |
| <span data-ttu-id="bacb9-140">controlTypeid</span><span class="sxs-lookup"><span data-stu-id="bacb9-140">controlTypeId</span></span> | <span data-ttu-id="bacb9-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bacb9-141">String</span></span> | <span data-ttu-id="bacb9-142">O programControlType identifica o tipo de controle de programa-por exemplo, um controle vinculando a revisões de acesso de convidados.</span><span class="sxs-lookup"><span data-stu-id="bacb9-142">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="bacb9-143">Obrigatório durante a criação.</span><span class="sxs-lookup"><span data-stu-id="bacb9-143">Required on create.</span></span> |
| <span data-ttu-id="bacb9-144">displayName</span><span class="sxs-lookup"><span data-stu-id="bacb9-144">displayName</span></span> | <span data-ttu-id="bacb9-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bacb9-145">String</span></span> | <span data-ttu-id="bacb9-146">O nome do controle.</span><span class="sxs-lookup"><span data-stu-id="bacb9-146">The name of the control.</span></span> |
| <span data-ttu-id="bacb9-147">status</span><span class="sxs-lookup"><span data-stu-id="bacb9-147">status</span></span> | <span data-ttu-id="bacb9-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bacb9-148">String</span></span> | <span data-ttu-id="bacb9-149">O status do ciclo de vida do controle.</span><span class="sxs-lookup"><span data-stu-id="bacb9-149">The life cycle status of the control.</span></span> |
| <span data-ttu-id="bacb9-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bacb9-150">createdDateTime</span></span> | <span data-ttu-id="bacb9-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bacb9-151">DateTimeOffset</span></span> | <span data-ttu-id="bacb9-152">A data e hora de criação do controle de programa.</span><span class="sxs-lookup"><span data-stu-id="bacb9-152">The creation date and time of the program control.</span></span> |
| <span data-ttu-id="bacb9-153">owner</span><span class="sxs-lookup"><span data-stu-id="bacb9-153">owner</span></span> | [<span data-ttu-id="bacb9-154">userIdentity</span><span class="sxs-lookup"><span data-stu-id="bacb9-154">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="bacb9-155">O usuário que criou o controle de programa.</span><span class="sxs-lookup"><span data-stu-id="bacb9-155">The user who created the program control.</span></span> |
| <span data-ttu-id="bacb9-156">recurso</span><span class="sxs-lookup"><span data-stu-id="bacb9-156">resource</span></span> | [<span data-ttu-id="bacb9-157">programResource</span><span class="sxs-lookup"><span data-stu-id="bacb9-157">programResource</span></span>](programresource.md) | <span data-ttu-id="bacb9-158">O recurso, um grupo ou um aplicativo, direcionado por essa revisão de acesso de controle de programa.</span><span class="sxs-lookup"><span data-stu-id="bacb9-158">The resource, a group or an app, targeted by this program control's access review.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bacb9-159">Relações</span><span class="sxs-lookup"><span data-stu-id="bacb9-159">Relationships</span></span>

| <span data-ttu-id="bacb9-160">Relação</span><span class="sxs-lookup"><span data-stu-id="bacb9-160">Relationship</span></span> | <span data-ttu-id="bacb9-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="bacb9-161">Type</span></span>   | <span data-ttu-id="bacb9-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="bacb9-162">Description</span></span> |
|:------------ |:---- |:----------- |
| <span data-ttu-id="bacb9-163">programa</span><span class="sxs-lookup"><span data-stu-id="bacb9-163">program</span></span> | [<span data-ttu-id="bacb9-164">programa</span><span class="sxs-lookup"><span data-stu-id="bacb9-164">program</span></span>](program.md) | <span data-ttu-id="bacb9-165">O programa do qual esse controle faz parte.</span><span class="sxs-lookup"><span data-stu-id="bacb9-165">The program this control is part of.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bacb9-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bacb9-166">JSON representation</span></span>

<span data-ttu-id="bacb9-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bacb9-167">Here is a JSON representation of the resource.</span></span>

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


