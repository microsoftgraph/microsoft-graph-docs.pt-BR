---
title: tipo de recurso do programa
description: 'No Windows Azure AD access analisa o recurso, um programa é um contêiner, mantendo os controles de programa. Um locatário pode ter um ou mais programas.  Cada controle vincula uma revisão de acesso a um programa, para torná-la mais fáceis de localizar relacionados access analisa.  '
localization_priority: Normal
ms.openlocfilehash: 2498279f27f5859eadcfa1d70662e3d8f3b5246c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515185"
---
# <a name="program-resource-type"></a><span data-ttu-id="58d5d-105">tipo de recurso do programa</span><span class="sxs-lookup"><span data-stu-id="58d5d-105">program resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58d5d-106">No recurso de [acesso analisa](accessreviews-root.md) Azure AD, um programa é um contêiner, mantendo os controles de programa.</span><span class="sxs-lookup"><span data-stu-id="58d5d-106">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="58d5d-107">Um locatário pode ter um ou mais programas.</span><span class="sxs-lookup"><span data-stu-id="58d5d-107">A tenant can have one or more programs.</span></span>  <span data-ttu-id="58d5d-108">Cada controle vincula uma revisão de acesso a um programa, para torná-la mais fáceis de localizar relacionados access analisa.</span><span class="sxs-lookup"><span data-stu-id="58d5d-108">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="58d5d-109">Cada locatário que tem em-hospedados Azure AD avaliações de acesso tem um programa, `Default program`.</span><span class="sxs-lookup"><span data-stu-id="58d5d-109">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="58d5d-110">Um administrador global pode criar programas adicionais, por exemplo representar as iniciativas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="58d5d-110">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="58d5d-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="58d5d-111">Methods</span></span>

| <span data-ttu-id="58d5d-112">Método</span><span class="sxs-lookup"><span data-stu-id="58d5d-112">Method</span></span>           | <span data-ttu-id="58d5d-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="58d5d-113">Return Type</span></span>    |<span data-ttu-id="58d5d-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="58d5d-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="58d5d-115">Criação de programa</span><span class="sxs-lookup"><span data-stu-id="58d5d-115">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="58d5d-116">programa</span><span class="sxs-lookup"><span data-stu-id="58d5d-116">program</span></span>](program.md)   |   <span data-ttu-id="58d5d-117">Crie um novo programa.</span><span class="sxs-lookup"><span data-stu-id="58d5d-117">Create a new program.</span></span>|
|[<span data-ttu-id="58d5d-118">Excluir programa</span><span class="sxs-lookup"><span data-stu-id="58d5d-118">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="58d5d-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="58d5d-119">None.</span></span>   |   <span data-ttu-id="58d5d-120">Exclua um programa.</span><span class="sxs-lookup"><span data-stu-id="58d5d-120">Delete a program.</span></span>|
|[<span data-ttu-id="58d5d-121">Lista de programas</span><span class="sxs-lookup"><span data-stu-id="58d5d-121">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="58d5d-122">coleção de [programa](program.md)</span><span class="sxs-lookup"><span data-stu-id="58d5d-122">[program](program.md) collection</span></span>|   <span data-ttu-id="58d5d-123">Obtenha uma coleção de todos os programas.</span><span class="sxs-lookup"><span data-stu-id="58d5d-123">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="58d5d-124">Lista programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="58d5d-124">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="58d5d-125">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="58d5d-125">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="58d5d-126">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="58d5d-126">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="58d5d-127">Programa de atualização</span><span class="sxs-lookup"><span data-stu-id="58d5d-127">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="58d5d-128">programa</span><span class="sxs-lookup"><span data-stu-id="58d5d-128">program</span></span>](program.md)|  <span data-ttu-id="58d5d-129">Atualize um programa.</span><span class="sxs-lookup"><span data-stu-id="58d5d-129">Update a program.</span></span>|

## <a name="permissions"></a><span data-ttu-id="58d5d-130">Permissões</span><span class="sxs-lookup"><span data-stu-id="58d5d-130">Permissions</span></span>

|<span data-ttu-id="58d5d-131">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58d5d-131">Permission type</span></span>                        | <span data-ttu-id="58d5d-132">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58d5d-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="58d5d-133">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58d5d-133">Delegated (work or school account)</span></span>     | <span data-ttu-id="58d5d-134">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58d5d-134">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="58d5d-135">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58d5d-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58d5d-136">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58d5d-136">Not supported.</span></span> |
|<span data-ttu-id="58d5d-137">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58d5d-137">Application</span></span>                            | <span data-ttu-id="58d5d-138">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58d5d-138">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="58d5d-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="58d5d-139">Properties</span></span>
| <span data-ttu-id="58d5d-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58d5d-140">Property</span></span>     | <span data-ttu-id="58d5d-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="58d5d-141">Type</span></span>   |<span data-ttu-id="58d5d-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="58d5d-142">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="58d5d-143">O identificador atribuído pelo recurso do programa.</span><span class="sxs-lookup"><span data-stu-id="58d5d-143">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="58d5d-144">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="58d5d-144">The name of the program.</span></span>  <span data-ttu-id="58d5d-145">Necessários na criação.</span><span class="sxs-lookup"><span data-stu-id="58d5d-145">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="58d5d-146">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="58d5d-146">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="58d5d-147">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="58d5d-147">Relationships</span></span>
| <span data-ttu-id="58d5d-148">Relação</span><span class="sxs-lookup"><span data-stu-id="58d5d-148">Relationship</span></span> | <span data-ttu-id="58d5d-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="58d5d-149">Type</span></span>   |<span data-ttu-id="58d5d-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="58d5d-150">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="58d5d-151">programControl</span><span class="sxs-lookup"><span data-stu-id="58d5d-151">programControl</span></span>](programcontrol.md) | <span data-ttu-id="58d5d-152">Controles associados com o programa.</span><span class="sxs-lookup"><span data-stu-id="58d5d-152">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="58d5d-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="58d5d-153">JSON representation</span></span>

<span data-ttu-id="58d5d-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="58d5d-154">Here is a JSON representation of the resource.</span></span>

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
