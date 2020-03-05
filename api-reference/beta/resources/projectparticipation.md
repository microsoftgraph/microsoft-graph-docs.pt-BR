---
title: tipo de recurso projectParticipation
description: tipo de recurso projectParticipation
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 1aa9188f40175ba0f52f143081004d8c3cbc4797
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521429"
---
# <a name="projectparticipation-resource-type"></a><span data-ttu-id="4343a-103">tipo de recurso projectParticipation</span><span class="sxs-lookup"><span data-stu-id="4343a-103">projectParticipation resource type</span></span>

<span data-ttu-id="4343a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4343a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4343a-105">Representa informações detalhadas sobre os projetos associados a um usuário.</span><span class="sxs-lookup"><span data-stu-id="4343a-105">Represents detailed information about projects associated with a user.</span></span>

<span data-ttu-id="4343a-106">Herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="4343a-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4343a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="4343a-107">Methods</span></span>

| <span data-ttu-id="4343a-108">Método</span><span class="sxs-lookup"><span data-stu-id="4343a-108">Method</span></span>                                                         | <span data-ttu-id="4343a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4343a-109">Return Type</span></span>                                     | <span data-ttu-id="4343a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4343a-110">Description</span></span>                                                       |
|:---------------------------------------------------------------|:------------------------------------------------|:------------------------------------------------------------------|
| [<span data-ttu-id="4343a-111">Obter projectParticipation</span><span class="sxs-lookup"><span data-stu-id="4343a-111">Get projectParticipation</span></span>](../api/projectparticipation-get.md) | [<span data-ttu-id="4343a-112">projectParticipation</span><span class="sxs-lookup"><span data-stu-id="4343a-112">projectParticipation</span></span>](projectparticipation.md) | <span data-ttu-id="4343a-113">Leia as propriedades e os relacionamentos de um objeto **projectParticipation** .</span><span class="sxs-lookup"><span data-stu-id="4343a-113">Read the properties and relationships of a **projectParticipation** object.</span></span> |
| [<span data-ttu-id="4343a-114">Atualizar projectParticipation</span><span class="sxs-lookup"><span data-stu-id="4343a-114">Update projectParticipation</span></span>](../api/projectparticipation-update.md)                | [<span data-ttu-id="4343a-115">projectParticipation</span><span class="sxs-lookup"><span data-stu-id="4343a-115">projectParticipation</span></span>](projectparticipation.md) | <span data-ttu-id="4343a-116">Atualizar um objeto **projectParticipation** .</span><span class="sxs-lookup"><span data-stu-id="4343a-116">Update a **projectParticipation** object.</span></span>                               |
| [<span data-ttu-id="4343a-117">Excluir projectParticipation</span><span class="sxs-lookup"><span data-stu-id="4343a-117">Delete projectParticipation</span></span>](../api/projectparticipation-delete.md)                | <span data-ttu-id="4343a-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4343a-118">None.</span></span>                                            | <span data-ttu-id="4343a-119">Excluir um objeto **projectParticipation** .</span><span class="sxs-lookup"><span data-stu-id="4343a-119">Delete a **projectParticipation** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="4343a-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4343a-120">Properties</span></span>

| <span data-ttu-id="4343a-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4343a-121">Property</span></span>     | <span data-ttu-id="4343a-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="4343a-122">Type</span></span>                                        | <span data-ttu-id="4343a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4343a-123">Description</span></span>                                                                                      |
|:-------------|:--------------------------------------------|:-------------------------------------------------------------------------------------------------|
|<span data-ttu-id="4343a-124">categories</span><span class="sxs-lookup"><span data-stu-id="4343a-124">categories</span></span>    | <span data-ttu-id="4343a-125">String collection</span><span class="sxs-lookup"><span data-stu-id="4343a-125">String collection</span></span>                           | <span data-ttu-id="4343a-126">Contém categorias que um usuário associou ao projeto (por exemplo, transformação digital, Rig óleo).</span><span class="sxs-lookup"><span data-stu-id="4343a-126">Contains categories a user has associated with the project (for example, digital transformation, oil rig).</span></span> |
|<span data-ttu-id="4343a-127">clientes</span><span class="sxs-lookup"><span data-stu-id="4343a-127">client</span></span>        |[<span data-ttu-id="4343a-128">companyDetail</span><span class="sxs-lookup"><span data-stu-id="4343a-128">companyDetail</span></span>](companydetail.md)            | <span data-ttu-id="4343a-129">Contém informações detalhadas sobre o cliente para o qual o projeto foi.</span><span class="sxs-lookup"><span data-stu-id="4343a-129">Contains detailed information about the client the project was for.</span></span>                              |
|<span data-ttu-id="4343a-130">conhecidos</span><span class="sxs-lookup"><span data-stu-id="4343a-130">colleagues</span></span>    |<span data-ttu-id="4343a-131">coleção [relatedPerson](relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="4343a-131">[relatedPerson](relatedperson.md) collection</span></span> | <span data-ttu-id="4343a-132">Lista as pessoas que também trabalharam no projeto.</span><span class="sxs-lookup"><span data-stu-id="4343a-132">Lists people that also worked on the project.</span></span>                                                          |
|<span data-ttu-id="4343a-133">detalhada</span><span class="sxs-lookup"><span data-stu-id="4343a-133">detail</span></span>        |[<span data-ttu-id="4343a-134">positionDetail</span><span class="sxs-lookup"><span data-stu-id="4343a-134">positionDetail</span></span>](positiondetail.md)          | <span data-ttu-id="4343a-135">Contém detalhes sobre a função do usuário no projeto.</span><span class="sxs-lookup"><span data-stu-id="4343a-135">Contains detail about the user's role on the project.</span></span>                                             |
|<span data-ttu-id="4343a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4343a-136">displayName</span></span>   |<span data-ttu-id="4343a-137">String</span><span class="sxs-lookup"><span data-stu-id="4343a-137">String</span></span>                                       |<span data-ttu-id="4343a-138">Contém um nome amigável para o projeto.</span><span class="sxs-lookup"><span data-stu-id="4343a-138">Contains a friendly name for the project.</span></span>                                                         |
|<span data-ttu-id="4343a-139">responsáveis</span><span class="sxs-lookup"><span data-stu-id="4343a-139">sponsors</span></span>      |<span data-ttu-id="4343a-140">coleção [relatedPerson](relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="4343a-140">[relatedPerson](relatedperson.md) collection</span></span> | <span data-ttu-id="4343a-141">A pessoa ou as pessoas que patrocinaram o projeto.</span><span class="sxs-lookup"><span data-stu-id="4343a-141">The Person or people who sponsored the project.</span></span>                                                         |

## <a name="relationships"></a><span data-ttu-id="4343a-142">Relações</span><span class="sxs-lookup"><span data-stu-id="4343a-142">Relationships</span></span>

<span data-ttu-id="4343a-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4343a-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4343a-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4343a-144">JSON representation</span></span>

<span data-ttu-id="4343a-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4343a-145">The following is a JSON representation of the resource.</span></span>

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
