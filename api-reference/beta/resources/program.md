---
title: tipo de recurso de programa
description: 'No recurso de revisões do Azure AD Access, um programa é um contêiner, contendo controles de programa. Um locatário pode ter um ou mais programas.  Cada controle vincula uma revisão do Access a um programa, para facilitar a localização de revisões relacionadas do Access.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a44c084b6f6d2da23290d3e962e2868f0c4c7ac0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521450"
---
# <a name="program-resource-type"></a><span data-ttu-id="83ae4-105">tipo de recurso de programa</span><span class="sxs-lookup"><span data-stu-id="83ae4-105">program resource type</span></span>

<span data-ttu-id="83ae4-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="83ae4-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83ae4-107">No recurso de revisões do Azure AD [Access](accessreviews-root.md) , um programa é um contêiner, contendo controles de programa.</span><span class="sxs-lookup"><span data-stu-id="83ae4-107">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="83ae4-108">Um locatário pode ter um ou mais programas.</span><span class="sxs-lookup"><span data-stu-id="83ae4-108">A tenant can have one or more programs.</span></span>  <span data-ttu-id="83ae4-109">Cada controle vincula uma revisão do Access a um programa, para facilitar a localização de revisões relacionadas do Access.</span><span class="sxs-lookup"><span data-stu-id="83ae4-109">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="83ae4-110">Cada locatário que tem revisões de acesso do Azure AD integradas tem um programa, `Default program`.</span><span class="sxs-lookup"><span data-stu-id="83ae4-110">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="83ae4-111">Um administrador global pode criar programas adicionais, por exemplo, para representar iniciativas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="83ae4-111">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="83ae4-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="83ae4-112">Methods</span></span>

| <span data-ttu-id="83ae4-113">Método</span><span class="sxs-lookup"><span data-stu-id="83ae4-113">Method</span></span>           | <span data-ttu-id="83ae4-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="83ae4-114">Return Type</span></span>    |<span data-ttu-id="83ae4-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="83ae4-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="83ae4-116">Criar programa</span><span class="sxs-lookup"><span data-stu-id="83ae4-116">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="83ae4-117">programa</span><span class="sxs-lookup"><span data-stu-id="83ae4-117">program</span></span>](program.md)   |   <span data-ttu-id="83ae4-118">Criar um novo programa.</span><span class="sxs-lookup"><span data-stu-id="83ae4-118">Create a new program.</span></span>|
|[<span data-ttu-id="83ae4-119">Excluir programa</span><span class="sxs-lookup"><span data-stu-id="83ae4-119">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="83ae4-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="83ae4-120">None.</span></span>   |   <span data-ttu-id="83ae4-121">Excluir um programa.</span><span class="sxs-lookup"><span data-stu-id="83ae4-121">Delete a program.</span></span>|
|[<span data-ttu-id="83ae4-122">Listar programas</span><span class="sxs-lookup"><span data-stu-id="83ae4-122">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="83ae4-123">coleção [Program](program.md)</span><span class="sxs-lookup"><span data-stu-id="83ae4-123">[program](program.md) collection</span></span>|   <span data-ttu-id="83ae4-124">Obtenha uma coleção de todos os programas.</span><span class="sxs-lookup"><span data-stu-id="83ae4-124">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="83ae4-125">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="83ae4-125">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="83ae4-126">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="83ae4-126">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="83ae4-127">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="83ae4-127">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="83ae4-128">Programa de atualização</span><span class="sxs-lookup"><span data-stu-id="83ae4-128">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="83ae4-129">programa</span><span class="sxs-lookup"><span data-stu-id="83ae4-129">program</span></span>](program.md)|  <span data-ttu-id="83ae4-130">Atualizar um programa.</span><span class="sxs-lookup"><span data-stu-id="83ae4-130">Update a program.</span></span>|

## <a name="properties"></a><span data-ttu-id="83ae4-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83ae4-131">Properties</span></span>
| <span data-ttu-id="83ae4-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83ae4-132">Property</span></span>     | <span data-ttu-id="83ae4-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="83ae4-133">Type</span></span>   |<span data-ttu-id="83ae4-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="83ae4-134">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="83ae4-135">O identificador do programa atribuído ao recurso.</span><span class="sxs-lookup"><span data-stu-id="83ae4-135">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="83ae4-136">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="83ae4-136">The name of the program.</span></span>  <span data-ttu-id="83ae4-137">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="83ae4-137">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="83ae4-138">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="83ae4-138">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="83ae4-139">Relações</span><span class="sxs-lookup"><span data-stu-id="83ae4-139">Relationships</span></span>
| <span data-ttu-id="83ae4-140">Relação</span><span class="sxs-lookup"><span data-stu-id="83ae4-140">Relationship</span></span> | <span data-ttu-id="83ae4-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="83ae4-141">Type</span></span>   |<span data-ttu-id="83ae4-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="83ae4-142">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="83ae4-143">programControl</span><span class="sxs-lookup"><span data-stu-id="83ae4-143">programControl</span></span>](programcontrol.md) | <span data-ttu-id="83ae4-144">Controles associados ao programa.</span><span class="sxs-lookup"><span data-stu-id="83ae4-144">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="83ae4-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83ae4-145">JSON representation</span></span>

<span data-ttu-id="83ae4-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83ae4-146">Here is a JSON representation of the resource.</span></span>

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
