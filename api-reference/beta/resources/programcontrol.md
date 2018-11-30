---
title: tipo de recurso de programControl
description: No Windows Azure AD access analisa o recurso, o objeto de controle do programa representa um controle, vinculando uma revisão de acesso a um programa.
ms.openlocfilehash: 03e70ffdf0607eeb11abaf1b12065b4092294d23
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036146"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="8b4e0-103">tipo de recurso de programControl</span><span class="sxs-lookup"><span data-stu-id="8b4e0-103">programControl resource type</span></span>

> <span data-ttu-id="8b4e0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b4e0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8b4e0-106">No recurso de [acesso analisa](accessreviews-root.md) Azure AD, o objeto de controle do programa representa um controle, vinculando uma revisão de acesso a um programa.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="8b4e0-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="8b4e0-107">Methods</span></span>

| <span data-ttu-id="8b4e0-108">Método</span><span class="sxs-lookup"><span data-stu-id="8b4e0-108">Method</span></span>           | <span data-ttu-id="8b4e0-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8b4e0-109">Return Type</span></span>    |<span data-ttu-id="8b4e0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b4e0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8b4e0-111">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="8b4e0-111">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="8b4e0-112">programControl</span><span class="sxs-lookup"><span data-stu-id="8b4e0-112">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="8b4e0-113">Adicione um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-113">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="8b4e0-114">Excluir programControl</span><span class="sxs-lookup"><span data-stu-id="8b4e0-114">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="8b4e0-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-115">None.</span></span>   |   <span data-ttu-id="8b4e0-116">Remova um programControl de um programa.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-116">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="8b4e0-117">Lista programControls</span><span class="sxs-lookup"><span data-stu-id="8b4e0-117">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="8b4e0-118">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="8b4e0-118">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="8b4e0-119">Controles de lista com todos os programas no inquilino.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-119">List controls across all programs in the tenant.</span></span>|

## <a name="permissions"></a><span data-ttu-id="8b4e0-120">Permissions</span><span class="sxs-lookup"><span data-stu-id="8b4e0-120">Permissions</span></span>

|<span data-ttu-id="8b4e0-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b4e0-121">Permission type</span></span>                        | <span data-ttu-id="8b4e0-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b4e0-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b4e0-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b4e0-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b4e0-124">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b4e0-124">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="8b4e0-125">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b4e0-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b4e0-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-126">Not supported.</span></span> |
|<span data-ttu-id="8b4e0-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b4e0-127">Application</span></span>                            | <span data-ttu-id="8b4e0-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-128">Not supported.</span></span> |

## <a name="properties"></a><span data-ttu-id="8b4e0-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8b4e0-129">Properties</span></span>
| <span data-ttu-id="8b4e0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b4e0-130">Property</span></span>     | <span data-ttu-id="8b4e0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b4e0-131">Type</span></span>   |<span data-ttu-id="8b4e0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b4e0-132">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="8b4e0-133">O identificador atribuído pelo recurso do vínculo entre o programa e controle</span><span class="sxs-lookup"><span data-stu-id="8b4e0-133">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="8b4e0-134">O programId do programa esse controle é parte do.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-134">The programId of the program this control is a part of.</span></span> <span data-ttu-id="8b4e0-135">Necessários na criação.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-135">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="8b4e0-136">ControlId do controle, em especial o identificador de uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-136">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="8b4e0-137">Necessários na criação.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-137">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="8b4e0-138">O programControlType identifica o tipo de controle do programa - por exemplo, um controle de vinculação para o acesso de convidado analisa.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-138">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="8b4e0-139">Necessários na criação.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-139">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="8b4e0-140">O nome do controle.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-140">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="8b4e0-141">O status do ciclo de vida do controle.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-141">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="8b4e0-142">A data de criação e a hora do controle programa.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-142">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="8b4e0-143">userIdentity</span><span class="sxs-lookup"><span data-stu-id="8b4e0-143">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="8b4e0-144">O usuário que criou o controle de programa.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-144">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="8b4e0-145">O recurso, um grupo ou um aplicativo alvo de revisão de acesso do controle este programa.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-145">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="8b4e0-146">Relações</span><span class="sxs-lookup"><span data-stu-id="8b4e0-146">Relationships</span></span>
| <span data-ttu-id="8b4e0-147">Relação</span><span class="sxs-lookup"><span data-stu-id="8b4e0-147">Relationship</span></span> | <span data-ttu-id="8b4e0-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b4e0-148">Type</span></span>   |<span data-ttu-id="8b4e0-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b4e0-149">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="8b4e0-150">programa</span><span class="sxs-lookup"><span data-stu-id="8b4e0-150">program</span></span>](program.md)               | <span data-ttu-id="8b4e0-151">O programa esse controle faz parte do.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-151">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="8b4e0-152">Confira também</span><span class="sxs-lookup"><span data-stu-id="8b4e0-152">See also</span></span>

| <span data-ttu-id="8b4e0-153">Método</span><span class="sxs-lookup"><span data-stu-id="8b4e0-153">Method</span></span>           | <span data-ttu-id="8b4e0-154">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8b4e0-154">Return Type</span></span>    |<span data-ttu-id="8b4e0-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b4e0-155">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8b4e0-156">Lista programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="8b4e0-156">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="8b4e0-157">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="8b4e0-157">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="8b4e0-158">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-158">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="8b4e0-159">Lista programControlTypes</span><span class="sxs-lookup"><span data-stu-id="8b4e0-159">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="8b4e0-160">coleção [programControlType](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="8b4e0-160">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="8b4e0-161">Lista os tipos de controle do programa.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-161">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8b4e0-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8b4e0-162">JSON representation</span></span>

<span data-ttu-id="8b4e0-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-163">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-programresource-complex-type"></a><span data-ttu-id="8b4e0-164">O tipo de programResource complexo</span><span class="sxs-lookup"><span data-stu-id="8b4e0-164">The programResource complex type</span></span>

<span data-ttu-id="8b4e0-165">O recurso de programa, contido em um objeto de controle de programa, é uma representação de uma referência a um objeto que é o destino da revisão acesso.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-165">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="8b4e0-166">Esse tipo de herda de `microsoft.graph.identity` e tem uma propriedade adicional:</span><span class="sxs-lookup"><span data-stu-id="8b4e0-166">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="8b4e0-167">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b4e0-167">Property</span></span>     | <span data-ttu-id="8b4e0-168">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b4e0-168">Type</span></span>   |<span data-ttu-id="8b4e0-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b4e0-169">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="8b4e0-170">Tipo de recurso, indicando se ele é um grupo ou um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8b4e0-170">Type of the resource, indicating whether it is a group or an app.</span></span> |     


<!-- {
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->