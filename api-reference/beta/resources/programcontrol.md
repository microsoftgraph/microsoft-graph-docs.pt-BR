---
title: tipo de recurso programControl
description: No recurso de revisões do Azure AD Access, o objeto de controle do programa representa um controle, vinculando uma revisão do Access a um programa.
localization_priority: Normal
ms.openlocfilehash: 3d9829b8e2585d4deda95551021e2fd9b8d14c7a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563305"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="86769-103">tipo de recurso programControl</span><span class="sxs-lookup"><span data-stu-id="86769-103">programControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86769-104">No recurso de revisões do Azure AD [Access](accessreviews-root.md) , o objeto de controle do programa representa um controle, vinculando uma revisão do Access a um programa.</span><span class="sxs-lookup"><span data-stu-id="86769-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="86769-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="86769-105">Methods</span></span>

| <span data-ttu-id="86769-106">Método</span><span class="sxs-lookup"><span data-stu-id="86769-106">Method</span></span>           | <span data-ttu-id="86769-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="86769-107">Return Type</span></span>    |<span data-ttu-id="86769-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="86769-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="86769-109">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="86769-109">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="86769-110">programControl</span><span class="sxs-lookup"><span data-stu-id="86769-110">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="86769-111">Adicionar um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="86769-111">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="86769-112">Excluir programControl</span><span class="sxs-lookup"><span data-stu-id="86769-112">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="86769-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="86769-113">None.</span></span>   |   <span data-ttu-id="86769-114">Remover um programControl de um programa.</span><span class="sxs-lookup"><span data-stu-id="86769-114">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="86769-115">Listar programControls</span><span class="sxs-lookup"><span data-stu-id="86769-115">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="86769-116">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="86769-116">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="86769-117">Listar controles em todos os programas no locatário.</span><span class="sxs-lookup"><span data-stu-id="86769-117">List controls across all programs in the tenant.</span></span>|

## <a name="permissions"></a><span data-ttu-id="86769-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="86769-118">Permissions</span></span>

|<span data-ttu-id="86769-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86769-119">Permission type</span></span>                        | <span data-ttu-id="86769-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86769-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="86769-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86769-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="86769-122">ProgramControl. Read. All, ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="86769-122">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="86769-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86769-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86769-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86769-124">Not supported.</span></span> |
|<span data-ttu-id="86769-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86769-125">Application</span></span>                            | <span data-ttu-id="86769-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86769-126">Not supported.</span></span> |

## <a name="properties"></a><span data-ttu-id="86769-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86769-127">Properties</span></span>
| <span data-ttu-id="86769-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86769-128">Property</span></span>     | <span data-ttu-id="86769-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="86769-129">Type</span></span>   |<span data-ttu-id="86769-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="86769-130">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="86769-131">O identificador atribuído ao recurso do link entre o programa e o controle</span><span class="sxs-lookup"><span data-stu-id="86769-131">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="86769-132">O ProgramId do programa do qual esse controle faz parte.</span><span class="sxs-lookup"><span data-stu-id="86769-132">The programId of the program this control is a part of.</span></span> <span data-ttu-id="86769-133">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="86769-133">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="86769-134">O controlId do controle, em particular, o identificador de uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="86769-134">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="86769-135">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="86769-135">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="86769-136">O programControlType identifica o tipo de controle de programa-por exemplo, um controle vinculando a revisões de acesso de convidados.</span><span class="sxs-lookup"><span data-stu-id="86769-136">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="86769-137">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="86769-137">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="86769-138">O nome do controle.</span><span class="sxs-lookup"><span data-stu-id="86769-138">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="86769-139">O status do ciclo de vida do controle.</span><span class="sxs-lookup"><span data-stu-id="86769-139">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="86769-140">A data e hora de criação do controle de programa.</span><span class="sxs-lookup"><span data-stu-id="86769-140">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="86769-141">userIdentity</span><span class="sxs-lookup"><span data-stu-id="86769-141">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="86769-142">O usuário que criou o controle de programa.</span><span class="sxs-lookup"><span data-stu-id="86769-142">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="86769-143">O recurso, um grupo ou um aplicativo, direcionado por essa revisão de acesso de controle de programa.</span><span class="sxs-lookup"><span data-stu-id="86769-143">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="86769-144">Relações</span><span class="sxs-lookup"><span data-stu-id="86769-144">Relationships</span></span>
| <span data-ttu-id="86769-145">Relação</span><span class="sxs-lookup"><span data-stu-id="86769-145">Relationship</span></span> | <span data-ttu-id="86769-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="86769-146">Type</span></span>   |<span data-ttu-id="86769-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="86769-147">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="86769-148">programa</span><span class="sxs-lookup"><span data-stu-id="86769-148">program</span></span>](program.md)               | <span data-ttu-id="86769-149">O programa do qual esse controle faz parte.</span><span class="sxs-lookup"><span data-stu-id="86769-149">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="86769-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="86769-150">See also</span></span>

| <span data-ttu-id="86769-151">Método</span><span class="sxs-lookup"><span data-stu-id="86769-151">Method</span></span>           | <span data-ttu-id="86769-152">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="86769-152">Return Type</span></span>    |<span data-ttu-id="86769-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="86769-153">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="86769-154">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="86769-154">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="86769-155">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="86769-155">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="86769-156">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="86769-156">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="86769-157">Listar programControlTypes</span><span class="sxs-lookup"><span data-stu-id="86769-157">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="86769-158">coleção [programControlType](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="86769-158">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="86769-159">Listar tipos de controle de programa.</span><span class="sxs-lookup"><span data-stu-id="86769-159">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="86769-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86769-160">JSON representation</span></span>

<span data-ttu-id="86769-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="86769-161">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-programresource-complex-type"></a><span data-ttu-id="86769-162">O tipo complexo programResource</span><span class="sxs-lookup"><span data-stu-id="86769-162">The programResource complex type</span></span>

<span data-ttu-id="86769-163">O recurso de programa, contido em um objeto de controle de programa, é uma representação de uma referência a um objeto que é o destino da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="86769-163">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="86769-164">Este tipo herda de `microsoft.graph.identity` e tem uma propriedade adicional:</span><span class="sxs-lookup"><span data-stu-id="86769-164">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="86769-165">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86769-165">Property</span></span>     | <span data-ttu-id="86769-166">Tipo</span><span class="sxs-lookup"><span data-stu-id="86769-166">Type</span></span>   |<span data-ttu-id="86769-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="86769-167">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="86769-168">Tipo do recurso, indicando se é um grupo ou um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="86769-168">Type of the resource, indicating whether it is a group or an app.</span></span> |     


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
