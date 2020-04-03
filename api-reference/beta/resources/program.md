---
title: tipo de recurso de programa
description: 'No recurso de revisões do Azure AD Access, um programa é um contêiner, contendo controles de programa. Um locatário pode ter um ou mais programas.  Cada controle vincula uma revisão do Access a um programa, para facilitar a localização de revisões relacionadas do Access.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: cc2ce31742cd4a02efbefebc85283c8d784ad16e
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125033"
---
# <a name="program-resource-type"></a><span data-ttu-id="35cf9-105">tipo de recurso de programa</span><span class="sxs-lookup"><span data-stu-id="35cf9-105">program resource type</span></span>

<span data-ttu-id="35cf9-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35cf9-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35cf9-107">No recurso de revisões do Azure AD [Access](accessreviews-root.md) , um programa é um contêiner, contendo controles de programa.</span><span class="sxs-lookup"><span data-stu-id="35cf9-107">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="35cf9-108">Um locatário pode ter um ou mais programas.</span><span class="sxs-lookup"><span data-stu-id="35cf9-108">A tenant can have one or more programs.</span></span>  <span data-ttu-id="35cf9-109">Cada controle vincula uma revisão do Access a um programa, para facilitar a localização de revisões relacionadas do Access.</span><span class="sxs-lookup"><span data-stu-id="35cf9-109">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="35cf9-110">Cada locatário que tem revisões de acesso do Azure AD integradas tem um programa, `Default program`.</span><span class="sxs-lookup"><span data-stu-id="35cf9-110">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="35cf9-111">Um administrador global pode criar programas adicionais, por exemplo, para representar iniciativas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="35cf9-111">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="35cf9-112">Methods</span><span class="sxs-lookup"><span data-stu-id="35cf9-112">Methods</span></span>

| <span data-ttu-id="35cf9-113">Método</span><span class="sxs-lookup"><span data-stu-id="35cf9-113">Method</span></span>           | <span data-ttu-id="35cf9-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="35cf9-114">Return Type</span></span>    |<span data-ttu-id="35cf9-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="35cf9-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35cf9-116">Criar programa</span><span class="sxs-lookup"><span data-stu-id="35cf9-116">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="35cf9-117">programa</span><span class="sxs-lookup"><span data-stu-id="35cf9-117">program</span></span>](program.md)   |   <span data-ttu-id="35cf9-118">Criar um novo programa.</span><span class="sxs-lookup"><span data-stu-id="35cf9-118">Create a new program.</span></span>|
|[<span data-ttu-id="35cf9-119">Excluir programa</span><span class="sxs-lookup"><span data-stu-id="35cf9-119">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="35cf9-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="35cf9-120">None.</span></span>   |   <span data-ttu-id="35cf9-121">Excluir um programa.</span><span class="sxs-lookup"><span data-stu-id="35cf9-121">Delete a program.</span></span>|
|[<span data-ttu-id="35cf9-122">Listar programas</span><span class="sxs-lookup"><span data-stu-id="35cf9-122">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="35cf9-123">coleção [Program](program.md)</span><span class="sxs-lookup"><span data-stu-id="35cf9-123">[program](program.md) collection</span></span>|   <span data-ttu-id="35cf9-124">Obtenha uma coleção de todos os programas.</span><span class="sxs-lookup"><span data-stu-id="35cf9-124">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="35cf9-125">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="35cf9-125">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="35cf9-126">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="35cf9-126">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="35cf9-127">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="35cf9-127">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="35cf9-128">Programa de atualização</span><span class="sxs-lookup"><span data-stu-id="35cf9-128">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="35cf9-129">programa</span><span class="sxs-lookup"><span data-stu-id="35cf9-129">program</span></span>](program.md)|  <span data-ttu-id="35cf9-130">Atualizar um programa.</span><span class="sxs-lookup"><span data-stu-id="35cf9-130">Update a program.</span></span>|

## <a name="properties"></a><span data-ttu-id="35cf9-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35cf9-131">Properties</span></span>
| <span data-ttu-id="35cf9-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35cf9-132">Property</span></span>     | <span data-ttu-id="35cf9-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="35cf9-133">Type</span></span>   |<span data-ttu-id="35cf9-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="35cf9-134">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="35cf9-135">O identificador do programa atribuído ao recurso.</span><span class="sxs-lookup"><span data-stu-id="35cf9-135">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="35cf9-136">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="35cf9-136">The name of the program.</span></span>  <span data-ttu-id="35cf9-137">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="35cf9-137">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="35cf9-138">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="35cf9-138">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="35cf9-139">Relações</span><span class="sxs-lookup"><span data-stu-id="35cf9-139">Relationships</span></span>
| <span data-ttu-id="35cf9-140">Relação</span><span class="sxs-lookup"><span data-stu-id="35cf9-140">Relationship</span></span> | <span data-ttu-id="35cf9-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="35cf9-141">Type</span></span>   |<span data-ttu-id="35cf9-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="35cf9-142">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="35cf9-143">programControl</span><span class="sxs-lookup"><span data-stu-id="35cf9-143">programControl</span></span>](programcontrol.md) | <span data-ttu-id="35cf9-144">Controles associados ao programa.</span><span class="sxs-lookup"><span data-stu-id="35cf9-144">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="35cf9-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35cf9-145">JSON representation</span></span>

<span data-ttu-id="35cf9-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35cf9-146">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
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
  "suppressions": []
}
-->
