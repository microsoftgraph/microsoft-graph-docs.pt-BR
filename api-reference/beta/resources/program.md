---
title: tipo de recurso de programa
description: 'No recurso de revisões do Azure AD Access, um programa é um contêiner, contendo controles de programa. Um locatário pode ter um ou mais programas.  Cada controle vincula uma revisão do Access a um programa, para facilitar a localização de revisões relacionadas do Access.  '
localization_priority: Normal
ms.openlocfilehash: 2498279f27f5859eadcfa1d70662e3d8f3b5246c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563369"
---
# <a name="program-resource-type"></a><span data-ttu-id="51821-105">tipo de recurso de programa</span><span class="sxs-lookup"><span data-stu-id="51821-105">program resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51821-106">No recurso de revisões do Azure AD [Access](accessreviews-root.md) , um programa é um contêiner, contendo controles de programa.</span><span class="sxs-lookup"><span data-stu-id="51821-106">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="51821-107">Um locatário pode ter um ou mais programas.</span><span class="sxs-lookup"><span data-stu-id="51821-107">A tenant can have one or more programs.</span></span>  <span data-ttu-id="51821-108">Cada controle vincula uma revisão do Access a um programa, para facilitar a localização de revisões relacionadas do Access.</span><span class="sxs-lookup"><span data-stu-id="51821-108">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="51821-109">Cada locatário que tem revisões de acesso do Azure AD integradas tem um programa, `Default program`.</span><span class="sxs-lookup"><span data-stu-id="51821-109">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="51821-110">Um administrador global pode criar programas adicionais, por exemplo, para representar iniciativas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="51821-110">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="51821-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="51821-111">Methods</span></span>

| <span data-ttu-id="51821-112">Método</span><span class="sxs-lookup"><span data-stu-id="51821-112">Method</span></span>           | <span data-ttu-id="51821-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="51821-113">Return Type</span></span>    |<span data-ttu-id="51821-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="51821-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="51821-115">Criar programa</span><span class="sxs-lookup"><span data-stu-id="51821-115">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="51821-116">programa</span><span class="sxs-lookup"><span data-stu-id="51821-116">program</span></span>](program.md)   |   <span data-ttu-id="51821-117">Criar um novo programa.</span><span class="sxs-lookup"><span data-stu-id="51821-117">Create a new program.</span></span>|
|[<span data-ttu-id="51821-118">Excluir programa</span><span class="sxs-lookup"><span data-stu-id="51821-118">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="51821-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="51821-119">None.</span></span>   |   <span data-ttu-id="51821-120">Excluir um programa.</span><span class="sxs-lookup"><span data-stu-id="51821-120">Delete a program.</span></span>|
|[<span data-ttu-id="51821-121">Listar programas</span><span class="sxs-lookup"><span data-stu-id="51821-121">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="51821-122">coleção [Program](program.md)</span><span class="sxs-lookup"><span data-stu-id="51821-122">[program](program.md) collection</span></span>|   <span data-ttu-id="51821-123">Obtenha uma coleção de todos os programas.</span><span class="sxs-lookup"><span data-stu-id="51821-123">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="51821-124">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="51821-124">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="51821-125">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="51821-125">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="51821-126">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="51821-126">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="51821-127">Programa de atualização</span><span class="sxs-lookup"><span data-stu-id="51821-127">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="51821-128">programa</span><span class="sxs-lookup"><span data-stu-id="51821-128">program</span></span>](program.md)|  <span data-ttu-id="51821-129">Atualizar um programa.</span><span class="sxs-lookup"><span data-stu-id="51821-129">Update a program.</span></span>|

## <a name="permissions"></a><span data-ttu-id="51821-130">Permissões</span><span class="sxs-lookup"><span data-stu-id="51821-130">Permissions</span></span>

|<span data-ttu-id="51821-131">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51821-131">Permission type</span></span>                        | <span data-ttu-id="51821-132">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="51821-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="51821-133">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51821-133">Delegated (work or school account)</span></span>     | <span data-ttu-id="51821-134">ProgramControl. Read. All, ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="51821-134">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="51821-135">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51821-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51821-136">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51821-136">Not supported.</span></span> |
|<span data-ttu-id="51821-137">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51821-137">Application</span></span>                            | <span data-ttu-id="51821-138">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51821-138">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="51821-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51821-139">Properties</span></span>
| <span data-ttu-id="51821-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51821-140">Property</span></span>     | <span data-ttu-id="51821-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="51821-141">Type</span></span>   |<span data-ttu-id="51821-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="51821-142">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="51821-143">O identificador do programa atribuído ao recurso.</span><span class="sxs-lookup"><span data-stu-id="51821-143">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="51821-144">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="51821-144">The name of the program.</span></span>  <span data-ttu-id="51821-145">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="51821-145">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="51821-146">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="51821-146">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="51821-147">Relações</span><span class="sxs-lookup"><span data-stu-id="51821-147">Relationships</span></span>
| <span data-ttu-id="51821-148">Relação</span><span class="sxs-lookup"><span data-stu-id="51821-148">Relationship</span></span> | <span data-ttu-id="51821-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="51821-149">Type</span></span>   |<span data-ttu-id="51821-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="51821-150">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="51821-151">programControl</span><span class="sxs-lookup"><span data-stu-id="51821-151">programControl</span></span>](programcontrol.md) | <span data-ttu-id="51821-152">Controles associados ao programa.</span><span class="sxs-lookup"><span data-stu-id="51821-152">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="51821-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51821-153">JSON representation</span></span>

<span data-ttu-id="51821-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51821-154">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.program"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "description": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "program resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/program.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
