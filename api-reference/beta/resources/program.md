---
title: tipo de recurso de programa
description: 'No recurso de revisões de acesso do Azure AD, um programa é um contêiner, mantendo controles de programa. Um locatário pode ter um ou mais programas.  Cada controle vincula uma revisão de acesso a um programa, para facilitar a localização de avaliações de acesso relacionadas.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: eb04c1e05c669758e282aebdcccfa4e55507e659
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960366"
---
# <a name="program-resource-type"></a><span data-ttu-id="02fe3-105">tipo de recurso de programa</span><span class="sxs-lookup"><span data-stu-id="02fe3-105">program resource type</span></span>

<span data-ttu-id="02fe3-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02fe3-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02fe3-107">No recurso de revisões de acesso do Azure AD, um programa é um contêiner, mantendo [controles](accessreviews-root.md) de programa.</span><span class="sxs-lookup"><span data-stu-id="02fe3-107">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="02fe3-108">Um locatário pode ter um ou mais programas.</span><span class="sxs-lookup"><span data-stu-id="02fe3-108">A tenant can have one or more programs.</span></span>  <span data-ttu-id="02fe3-109">Cada controle vincula uma revisão de acesso a um programa, para facilitar a localização de avaliações de acesso relacionadas.</span><span class="sxs-lookup"><span data-stu-id="02fe3-109">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="02fe3-110">Cada locatário que tenha avaliações de acesso do Azure AD no Azure tem um programa, `Default program` .</span><span class="sxs-lookup"><span data-stu-id="02fe3-110">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="02fe3-111">Um administrador global pode criar programas adicionais, por exemplo, para representar iniciativas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="02fe3-111">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="02fe3-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="02fe3-112">Methods</span></span>

| <span data-ttu-id="02fe3-113">Método</span><span class="sxs-lookup"><span data-stu-id="02fe3-113">Method</span></span>           | <span data-ttu-id="02fe3-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="02fe3-114">Return Type</span></span>    |<span data-ttu-id="02fe3-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="02fe3-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="02fe3-116">Criar programa</span><span class="sxs-lookup"><span data-stu-id="02fe3-116">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="02fe3-117">program</span><span class="sxs-lookup"><span data-stu-id="02fe3-117">program</span></span>](program.md)   |   <span data-ttu-id="02fe3-118">Crie um novo programa.</span><span class="sxs-lookup"><span data-stu-id="02fe3-118">Create a new program.</span></span>|
|[<span data-ttu-id="02fe3-119">Excluir programa</span><span class="sxs-lookup"><span data-stu-id="02fe3-119">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="02fe3-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="02fe3-120">None.</span></span>   |   <span data-ttu-id="02fe3-121">Excluir um programa.</span><span class="sxs-lookup"><span data-stu-id="02fe3-121">Delete a program.</span></span>|
|[<span data-ttu-id="02fe3-122">Listar programas</span><span class="sxs-lookup"><span data-stu-id="02fe3-122">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="02fe3-123">[conjunto de](program.md) programas</span><span class="sxs-lookup"><span data-stu-id="02fe3-123">[program](program.md) collection</span></span>|   <span data-ttu-id="02fe3-124">Obter uma coleção de todos os programas.</span><span class="sxs-lookup"><span data-stu-id="02fe3-124">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="02fe3-125">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="02fe3-125">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="02fe3-126">[Coleção programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="02fe3-126">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="02fe3-127">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="02fe3-127">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="02fe3-128">Atualizar programa</span><span class="sxs-lookup"><span data-stu-id="02fe3-128">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="02fe3-129">program</span><span class="sxs-lookup"><span data-stu-id="02fe3-129">program</span></span>](program.md)|  <span data-ttu-id="02fe3-130">Atualize um programa.</span><span class="sxs-lookup"><span data-stu-id="02fe3-130">Update a program.</span></span>|

## <a name="properties"></a><span data-ttu-id="02fe3-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="02fe3-131">Properties</span></span>
| <span data-ttu-id="02fe3-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02fe3-132">Property</span></span>     | <span data-ttu-id="02fe3-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="02fe3-133">Type</span></span>   |<span data-ttu-id="02fe3-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="02fe3-134">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="02fe3-135">id</span><span class="sxs-lookup"><span data-stu-id="02fe3-135">id</span></span>                        |<span data-ttu-id="02fe3-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02fe3-136">String</span></span>                              |  <span data-ttu-id="02fe3-137">O identificador atribuído ao recurso do programa.</span><span class="sxs-lookup"><span data-stu-id="02fe3-137">The feature-assigned identifier of the program.</span></span>                    |
| <span data-ttu-id="02fe3-138">displayName</span><span class="sxs-lookup"><span data-stu-id="02fe3-138">displayName</span></span>               |<span data-ttu-id="02fe3-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02fe3-139">String</span></span>                              |  <span data-ttu-id="02fe3-140">O nome do programa.</span><span class="sxs-lookup"><span data-stu-id="02fe3-140">The name of the program.</span></span>  <span data-ttu-id="02fe3-141">Obrigatório durante a criação.</span><span class="sxs-lookup"><span data-stu-id="02fe3-141">Required on create.</span></span>                  |
| <span data-ttu-id="02fe3-142">description</span><span class="sxs-lookup"><span data-stu-id="02fe3-142">description</span></span>               |<span data-ttu-id="02fe3-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02fe3-143">String</span></span>                              |  <span data-ttu-id="02fe3-144">A descrição do programa.</span><span class="sxs-lookup"><span data-stu-id="02fe3-144">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="02fe3-145">Relações</span><span class="sxs-lookup"><span data-stu-id="02fe3-145">Relationships</span></span>
| <span data-ttu-id="02fe3-146">Relação</span><span class="sxs-lookup"><span data-stu-id="02fe3-146">Relationship</span></span> | <span data-ttu-id="02fe3-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="02fe3-147">Type</span></span>   |<span data-ttu-id="02fe3-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="02fe3-148">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="02fe3-149">programControl</span><span class="sxs-lookup"><span data-stu-id="02fe3-149">programControl</span></span>](programcontrol.md) | <span data-ttu-id="02fe3-150">Controles associados ao programa.</span><span class="sxs-lookup"><span data-stu-id="02fe3-150">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="02fe3-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="02fe3-151">JSON representation</span></span>

<span data-ttu-id="02fe3-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="02fe3-152">Here is a JSON representation of the resource.</span></span>

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


