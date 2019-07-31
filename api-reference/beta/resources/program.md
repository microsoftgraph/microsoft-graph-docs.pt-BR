---
title: tipo de recurso de programa
description: 'No recurso de revisões do Azure AD Access, um programa é um contêiner, contendo controles de programa. Um locatário pode ter um ou mais programas.  Cada controle vincula uma revisão do Access a um programa, para facilitar a localização de revisões relacionadas do Access.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c6a978ef4bb68c09b2f5659e255d16681c9c805d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965667"
---
# <a name="program-resource-type"></a><span data-ttu-id="3b7f0-105">tipo de recurso de programa</span><span class="sxs-lookup"><span data-stu-id="3b7f0-105">program resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b7f0-106">No recurso de revisões do Azure AD [Access](accessreviews-root.md) , um programa é um contêiner, contendo controles de programa.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-106">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="3b7f0-107">Um locatário pode ter um ou mais programas.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-107">A tenant can have one or more programs.</span></span>  <span data-ttu-id="3b7f0-108">Cada controle vincula uma revisão do Access a um programa, para facilitar a localização de revisões relacionadas do Access.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-108">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="3b7f0-109">Cada locatário que tem revisões de acesso do Azure AD integradas tem um programa, `Default program`.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-109">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="3b7f0-110">Um administrador global pode criar programas adicionais, por exemplo, para representar iniciativas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-110">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="3b7f0-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="3b7f0-111">Methods</span></span>

| <span data-ttu-id="3b7f0-112">Método</span><span class="sxs-lookup"><span data-stu-id="3b7f0-112">Method</span></span>           | <span data-ttu-id="3b7f0-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3b7f0-113">Return Type</span></span>    |<span data-ttu-id="3b7f0-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b7f0-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3b7f0-115">Criar programa</span><span class="sxs-lookup"><span data-stu-id="3b7f0-115">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="3b7f0-116">programa</span><span class="sxs-lookup"><span data-stu-id="3b7f0-116">program</span></span>](program.md)   |   <span data-ttu-id="3b7f0-117">Criar um novo programa.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-117">Create a new program.</span></span>|
|[<span data-ttu-id="3b7f0-118">Excluir programa</span><span class="sxs-lookup"><span data-stu-id="3b7f0-118">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="3b7f0-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-119">None.</span></span>   |   <span data-ttu-id="3b7f0-120">Excluir um programa.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-120">Delete a program.</span></span>|
|[<span data-ttu-id="3b7f0-121">Listar programas</span><span class="sxs-lookup"><span data-stu-id="3b7f0-121">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="3b7f0-122">coleção [Program](program.md)</span><span class="sxs-lookup"><span data-stu-id="3b7f0-122">[program](program.md) collection</span></span>|   <span data-ttu-id="3b7f0-123">Obtenha uma coleção de todos os programas.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-123">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="3b7f0-124">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="3b7f0-124">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="3b7f0-125">coleção [programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="3b7f0-125">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="3b7f0-126">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-126">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="3b7f0-127">Programa de atualização</span><span class="sxs-lookup"><span data-stu-id="3b7f0-127">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="3b7f0-128">programa</span><span class="sxs-lookup"><span data-stu-id="3b7f0-128">program</span></span>](program.md)|  <span data-ttu-id="3b7f0-129">Atualizar um programa.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-129">Update a program.</span></span>|

## <a name="properties"></a><span data-ttu-id="3b7f0-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b7f0-130">Properties</span></span>
| <span data-ttu-id="3b7f0-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b7f0-131">Property</span></span>     | <span data-ttu-id="3b7f0-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b7f0-132">Type</span></span>   |<span data-ttu-id="3b7f0-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b7f0-133">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="3b7f0-134">O identificador do programa atribuído ao recurso.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-134">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="3b7f0-135">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-135">The name of the program.</span></span>  <span data-ttu-id="3b7f0-136">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-136">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="3b7f0-137">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-137">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="3b7f0-138">Relações</span><span class="sxs-lookup"><span data-stu-id="3b7f0-138">Relationships</span></span>
| <span data-ttu-id="3b7f0-139">Relação</span><span class="sxs-lookup"><span data-stu-id="3b7f0-139">Relationship</span></span> | <span data-ttu-id="3b7f0-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b7f0-140">Type</span></span>   |<span data-ttu-id="3b7f0-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b7f0-141">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="3b7f0-142">programControl</span><span class="sxs-lookup"><span data-stu-id="3b7f0-142">programControl</span></span>](programcontrol.md) | <span data-ttu-id="3b7f0-143">Controles associados ao programa.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-143">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3b7f0-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b7f0-144">JSON representation</span></span>

<span data-ttu-id="3b7f0-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3b7f0-145">Here is a JSON representation of the resource.</span></span>

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
