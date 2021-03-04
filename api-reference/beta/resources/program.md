---
title: tipo de recurso de programa
description: 'No recurso de revisões de acesso do Azure AD, um programa é um contêiner, mantendo controles de programa. Um locatário pode ter um ou mais programas.  Cada controle vincula uma revisão de acesso a um programa, para facilitar a localização de avaliações de acesso relacionadas.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: f10ee2a54a310018d87500e5dd4f939d1fe38a0e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443983"
---
# <a name="program-resource-type"></a><span data-ttu-id="b46fe-105">tipo de recurso de programa</span><span class="sxs-lookup"><span data-stu-id="b46fe-105">program resource type</span></span>

<span data-ttu-id="b46fe-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b46fe-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b46fe-107">No recurso de revisões de acesso do Azure AD, um programa é um contêiner, mantendo [controles](accessreviews-root.md) de programa.</span><span class="sxs-lookup"><span data-stu-id="b46fe-107">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="b46fe-108">Um locatário pode ter um ou mais programas.</span><span class="sxs-lookup"><span data-stu-id="b46fe-108">A tenant can have one or more programs.</span></span>  <span data-ttu-id="b46fe-109">Cada controle vincula uma revisão de acesso a um programa, para facilitar a localização de avaliações de acesso relacionadas.</span><span class="sxs-lookup"><span data-stu-id="b46fe-109">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="b46fe-110">Cada locatário que tenha avaliações de acesso do Azure AD no Azure tem um programa, `Default program` .</span><span class="sxs-lookup"><span data-stu-id="b46fe-110">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="b46fe-111">Um administrador global pode criar programas adicionais, por exemplo, para representar iniciativas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="b46fe-111">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="b46fe-112">Methods</span><span class="sxs-lookup"><span data-stu-id="b46fe-112">Methods</span></span>

| <span data-ttu-id="b46fe-113">Método</span><span class="sxs-lookup"><span data-stu-id="b46fe-113">Method</span></span>           | <span data-ttu-id="b46fe-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b46fe-114">Return Type</span></span>    |<span data-ttu-id="b46fe-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="b46fe-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b46fe-116">Criar programa</span><span class="sxs-lookup"><span data-stu-id="b46fe-116">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="b46fe-117">program</span><span class="sxs-lookup"><span data-stu-id="b46fe-117">program</span></span>](program.md)   |   <span data-ttu-id="b46fe-118">Crie um novo programa.</span><span class="sxs-lookup"><span data-stu-id="b46fe-118">Create a new program.</span></span>|
|[<span data-ttu-id="b46fe-119">Excluir programa</span><span class="sxs-lookup"><span data-stu-id="b46fe-119">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="b46fe-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b46fe-120">None.</span></span>   |   <span data-ttu-id="b46fe-121">Excluir um programa.</span><span class="sxs-lookup"><span data-stu-id="b46fe-121">Delete a program.</span></span>|
|[<span data-ttu-id="b46fe-122">Listar programas</span><span class="sxs-lookup"><span data-stu-id="b46fe-122">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="b46fe-123">[conjunto de](program.md) programas</span><span class="sxs-lookup"><span data-stu-id="b46fe-123">[program](program.md) collection</span></span>|   <span data-ttu-id="b46fe-124">Obter uma coleção de todos os programas.</span><span class="sxs-lookup"><span data-stu-id="b46fe-124">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="b46fe-125">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="b46fe-125">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="b46fe-126">[Coleção programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="b46fe-126">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="b46fe-127">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="b46fe-127">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="b46fe-128">Atualizar programa</span><span class="sxs-lookup"><span data-stu-id="b46fe-128">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="b46fe-129">program</span><span class="sxs-lookup"><span data-stu-id="b46fe-129">program</span></span>](program.md)|  <span data-ttu-id="b46fe-130">Atualize um programa.</span><span class="sxs-lookup"><span data-stu-id="b46fe-130">Update a program.</span></span>|

## <a name="properties"></a><span data-ttu-id="b46fe-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b46fe-131">Properties</span></span>
| <span data-ttu-id="b46fe-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b46fe-132">Property</span></span>     | <span data-ttu-id="b46fe-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="b46fe-133">Type</span></span>   |<span data-ttu-id="b46fe-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="b46fe-134">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="b46fe-135">O identificador atribuído ao recurso do programa.</span><span class="sxs-lookup"><span data-stu-id="b46fe-135">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="b46fe-136">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="b46fe-136">The name of the program.</span></span>  <span data-ttu-id="b46fe-137">Obrigatório durante a criação.</span><span class="sxs-lookup"><span data-stu-id="b46fe-137">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="b46fe-138">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="b46fe-138">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="b46fe-139">Relações</span><span class="sxs-lookup"><span data-stu-id="b46fe-139">Relationships</span></span>
| <span data-ttu-id="b46fe-140">Relação</span><span class="sxs-lookup"><span data-stu-id="b46fe-140">Relationship</span></span> | <span data-ttu-id="b46fe-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="b46fe-141">Type</span></span>   |<span data-ttu-id="b46fe-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="b46fe-142">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="b46fe-143">programControl</span><span class="sxs-lookup"><span data-stu-id="b46fe-143">programControl</span></span>](programcontrol.md) | <span data-ttu-id="b46fe-144">Controles associados ao programa.</span><span class="sxs-lookup"><span data-stu-id="b46fe-144">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b46fe-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b46fe-145">JSON representation</span></span>

<span data-ttu-id="b46fe-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b46fe-146">Here is a JSON representation of the resource.</span></span>

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


