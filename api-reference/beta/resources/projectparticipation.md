---
title: tipo de recurso projectParticipation
description: tipo de recurso projectParticipation
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 465a45a2ba8a607d0537e66b96207b3d60626517
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950469"
---
# <a name="projectparticipation-resource-type"></a><span data-ttu-id="3267a-103">tipo de recurso projectParticipation</span><span class="sxs-lookup"><span data-stu-id="3267a-103">projectParticipation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3267a-104">Representa informações detalhadas sobre os projetos associados a um usuário.</span><span class="sxs-lookup"><span data-stu-id="3267a-104">Represents detailed information about projects associated with a user.</span></span>

<span data-ttu-id="3267a-105">Herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="3267a-105">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3267a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="3267a-106">Methods</span></span>

| <span data-ttu-id="3267a-107">Método</span><span class="sxs-lookup"><span data-stu-id="3267a-107">Method</span></span>                                                         | <span data-ttu-id="3267a-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3267a-108">Return Type</span></span>                                     | <span data-ttu-id="3267a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3267a-109">Description</span></span>                                                       |
|:---------------------------------------------------------------|:------------------------------------------------|:------------------------------------------------------------------|
| [<span data-ttu-id="3267a-110">Obter projectParticipation</span><span class="sxs-lookup"><span data-stu-id="3267a-110">Get projectParticipation</span></span>](../api/projectparticipation-get.md) | [<span data-ttu-id="3267a-111">projectParticipation</span><span class="sxs-lookup"><span data-stu-id="3267a-111">projectParticipation</span></span>](projectparticipation.md) | <span data-ttu-id="3267a-112">Leia as propriedades e os relacionamentos de um objeto **projectParticipation** .</span><span class="sxs-lookup"><span data-stu-id="3267a-112">Read the properties and relationships of a **projectParticipation** object.</span></span> |
| [<span data-ttu-id="3267a-113">Atualizar projectParticipation</span><span class="sxs-lookup"><span data-stu-id="3267a-113">Update projectParticipation</span></span>](../api/projectparticipation-update.md)                | [<span data-ttu-id="3267a-114">projectParticipation</span><span class="sxs-lookup"><span data-stu-id="3267a-114">projectParticipation</span></span>](projectparticipation.md) | <span data-ttu-id="3267a-115">Atualizar um objeto **projectParticipation** .</span><span class="sxs-lookup"><span data-stu-id="3267a-115">Update a **projectParticipation** object.</span></span>                               |
| [<span data-ttu-id="3267a-116">Excluir projectParticipation</span><span class="sxs-lookup"><span data-stu-id="3267a-116">Delete projectParticipation</span></span>](../api/projectparticipation-delete.md)                | <span data-ttu-id="3267a-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3267a-117">None.</span></span>                                            | <span data-ttu-id="3267a-118">Excluir um objeto **projectParticipation** .</span><span class="sxs-lookup"><span data-stu-id="3267a-118">Delete a **projectParticipation** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="3267a-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3267a-119">Properties</span></span>

| <span data-ttu-id="3267a-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3267a-120">Property</span></span>     | <span data-ttu-id="3267a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3267a-121">Type</span></span>                                        | <span data-ttu-id="3267a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3267a-122">Description</span></span>                                                                                      |
|:-------------|:--------------------------------------------|:-------------------------------------------------------------------------------------------------|
|<span data-ttu-id="3267a-123">categories</span><span class="sxs-lookup"><span data-stu-id="3267a-123">categories</span></span>    | <span data-ttu-id="3267a-124">String collection</span><span class="sxs-lookup"><span data-stu-id="3267a-124">String collection</span></span>                           | <span data-ttu-id="3267a-125">Contém categorias que um usuário associou ao projeto (por exemplo, transformação digital, Rig óleo).</span><span class="sxs-lookup"><span data-stu-id="3267a-125">Contains categories a user has associated with the project (for example, digital transformation, oil rig).</span></span> |
|<span data-ttu-id="3267a-126">clientes</span><span class="sxs-lookup"><span data-stu-id="3267a-126">client</span></span>        |[<span data-ttu-id="3267a-127">companyDetail</span><span class="sxs-lookup"><span data-stu-id="3267a-127">companyDetail</span></span>](companydetail.md)            | <span data-ttu-id="3267a-128">Contém informações detalhadas sobre o cliente para o qual o projeto foi.</span><span class="sxs-lookup"><span data-stu-id="3267a-128">Contains detailed information about the client the project was for.</span></span>                              |
|<span data-ttu-id="3267a-129">conhecidos</span><span class="sxs-lookup"><span data-stu-id="3267a-129">colleagues</span></span>    |<span data-ttu-id="3267a-130">coleção [relatedPerson](relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="3267a-130">[relatedPerson](relatedperson.md) collection</span></span> | <span data-ttu-id="3267a-131">Lista as pessoas que também trabalharam no projeto.</span><span class="sxs-lookup"><span data-stu-id="3267a-131">Lists people that also worked on the project.</span></span>                                                          |
|<span data-ttu-id="3267a-132">detalhada</span><span class="sxs-lookup"><span data-stu-id="3267a-132">detail</span></span>        |[<span data-ttu-id="3267a-133">positionDetail</span><span class="sxs-lookup"><span data-stu-id="3267a-133">positionDetail</span></span>](positiondetail.md)          | <span data-ttu-id="3267a-134">Contém detalhes sobre a função do usuário no projeto.</span><span class="sxs-lookup"><span data-stu-id="3267a-134">Contains detail about the user's role on the project.</span></span>                                             |
|<span data-ttu-id="3267a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="3267a-135">displayName</span></span>   |<span data-ttu-id="3267a-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3267a-136">String</span></span>                                       |<span data-ttu-id="3267a-137">Contém um nome amigável para o projeto.</span><span class="sxs-lookup"><span data-stu-id="3267a-137">Contains a friendly name for the project.</span></span>                                                         |
|<span data-ttu-id="3267a-138">responsáveis</span><span class="sxs-lookup"><span data-stu-id="3267a-138">sponsors</span></span>      |<span data-ttu-id="3267a-139">coleção [relatedPerson](relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="3267a-139">[relatedPerson](relatedperson.md) collection</span></span> | <span data-ttu-id="3267a-140">A pessoa ou as pessoas que patrocinaram o projeto.</span><span class="sxs-lookup"><span data-stu-id="3267a-140">The Person or people who sponsored the project.</span></span>                                                         |

## <a name="relationships"></a><span data-ttu-id="3267a-141">Relações</span><span class="sxs-lookup"><span data-stu-id="3267a-141">Relationships</span></span>

<span data-ttu-id="3267a-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3267a-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3267a-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3267a-143">JSON representation</span></span>

<span data-ttu-id="3267a-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3267a-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.projectParticipation",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "client": {"@odata.type": "microsoft.graph.companyDetail"},
  "colleagues": [{"@odata.type": "microsoft.graph.relatedPerson"}],
  "detail": {"@odata.type": "microsoft.graph.positionDetail"},
  "displayName": "String",
  "sponsors": [{"@odata.type": "microsoft.graph.relatedPerson"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "projectParticipation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
