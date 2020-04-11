---
title: tipo de recurso projectParticipation
description: tipo de recurso projectParticipation
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 2e292795eeccc25029063763c0e1a2c4883009d7
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227677"
---
# <a name="projectparticipation-resource-type"></a><span data-ttu-id="d5d55-103">tipo de recurso projectParticipation</span><span class="sxs-lookup"><span data-stu-id="d5d55-103">projectParticipation resource type</span></span>

<span data-ttu-id="d5d55-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5d55-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5d55-105">Representa informações detalhadas sobre os projetos associados a um usuário.</span><span class="sxs-lookup"><span data-stu-id="d5d55-105">Represents detailed information about projects associated with a user.</span></span>

<span data-ttu-id="d5d55-106">Herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d5d55-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d5d55-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d5d55-107">Methods</span></span>

| <span data-ttu-id="d5d55-108">Método</span><span class="sxs-lookup"><span data-stu-id="d5d55-108">Method</span></span>                                                                | <span data-ttu-id="d5d55-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d5d55-109">Return Type</span></span>                                     | <span data-ttu-id="d5d55-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5d55-110">Description</span></span>                                                                 |
|:----------------------------------------------------------------------|:------------------------------------------------|:----------------------------------------------------------------------------|
| [<span data-ttu-id="d5d55-111">Obter projectParticipation</span><span class="sxs-lookup"><span data-stu-id="d5d55-111">Get projectParticipation</span></span>](../api/projectparticipation-get.md)        | [<span data-ttu-id="d5d55-112">projectParticipation</span><span class="sxs-lookup"><span data-stu-id="d5d55-112">projectParticipation</span></span>](projectparticipation.md) | <span data-ttu-id="d5d55-113">Leia as propriedades e os relacionamentos de um objeto **projectParticipation** .</span><span class="sxs-lookup"><span data-stu-id="d5d55-113">Read the properties and relationships of a **projectParticipation** object.</span></span> |
| [<span data-ttu-id="d5d55-114">Atualizar projectParticipation</span><span class="sxs-lookup"><span data-stu-id="d5d55-114">Update projectParticipation</span></span>](../api/projectparticipation-update.md)  | [<span data-ttu-id="d5d55-115">projectParticipation</span><span class="sxs-lookup"><span data-stu-id="d5d55-115">projectParticipation</span></span>](projectparticipation.md) | <span data-ttu-id="d5d55-116">Atualizar um objeto **projectParticipation** .</span><span class="sxs-lookup"><span data-stu-id="d5d55-116">Update a **projectParticipation** object.</span></span>                                   |
| [<span data-ttu-id="d5d55-117">Excluir projectParticipation</span><span class="sxs-lookup"><span data-stu-id="d5d55-117">Delete projectParticipation</span></span>](../api/projectparticipation-delete.md)  | <span data-ttu-id="d5d55-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d5d55-118">None.</span></span>                                           | <span data-ttu-id="d5d55-119">Excluir um objeto **projectParticipation** .</span><span class="sxs-lookup"><span data-stu-id="d5d55-119">Delete a **projectParticipation** object.</span></span>                                   |

## <a name="properties"></a><span data-ttu-id="d5d55-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5d55-120">Properties</span></span>

| <span data-ttu-id="d5d55-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5d55-121">Property</span></span>     | <span data-ttu-id="d5d55-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5d55-122">Type</span></span>                                        | <span data-ttu-id="d5d55-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5d55-123">Description</span></span>                                                                                                |
|:-------------|:--------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="d5d55-124">categories</span><span class="sxs-lookup"><span data-stu-id="d5d55-124">categories</span></span>    | <span data-ttu-id="d5d55-125">String collection</span><span class="sxs-lookup"><span data-stu-id="d5d55-125">String collection</span></span>                           | <span data-ttu-id="d5d55-126">Contém categorias que um usuário associou ao projeto (por exemplo, transformação digital, Rig óleo).</span><span class="sxs-lookup"><span data-stu-id="d5d55-126">Contains categories a user has associated with the project (for example, digital transformation, oil rig).</span></span> |
|<span data-ttu-id="d5d55-127">clientes</span><span class="sxs-lookup"><span data-stu-id="d5d55-127">client</span></span>        |[<span data-ttu-id="d5d55-128">companyDetail</span><span class="sxs-lookup"><span data-stu-id="d5d55-128">companyDetail</span></span>](companydetail.md)            | <span data-ttu-id="d5d55-129">Contém informações detalhadas sobre o cliente para o qual o projeto foi.</span><span class="sxs-lookup"><span data-stu-id="d5d55-129">Contains detailed information about the client the project was for.</span></span>                                        |
|<span data-ttu-id="d5d55-130">conhecidos</span><span class="sxs-lookup"><span data-stu-id="d5d55-130">colleagues</span></span>    |<span data-ttu-id="d5d55-131">coleção [relatedPerson](relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="d5d55-131">[relatedPerson](relatedperson.md) collection</span></span> | <span data-ttu-id="d5d55-132">Lista as pessoas que também trabalharam no projeto.</span><span class="sxs-lookup"><span data-stu-id="d5d55-132">Lists people that also worked on the project.</span></span>                                                              |
|<span data-ttu-id="d5d55-133">detalhada</span><span class="sxs-lookup"><span data-stu-id="d5d55-133">detail</span></span>        |[<span data-ttu-id="d5d55-134">positionDetail</span><span class="sxs-lookup"><span data-stu-id="d5d55-134">positionDetail</span></span>](positiondetail.md)          | <span data-ttu-id="d5d55-135">Contém detalhes sobre a função do usuário no projeto.</span><span class="sxs-lookup"><span data-stu-id="d5d55-135">Contains detail about the user's role on the project.</span></span>                                                      |
|<span data-ttu-id="d5d55-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d5d55-136">displayName</span></span>   |<span data-ttu-id="d5d55-137">String</span><span class="sxs-lookup"><span data-stu-id="d5d55-137">String</span></span>                                       |<span data-ttu-id="d5d55-138">Contém um nome amigável para o projeto.</span><span class="sxs-lookup"><span data-stu-id="d5d55-138">Contains a friendly name for the project.</span></span>                                                                   |
|<span data-ttu-id="d5d55-139">responsáveis</span><span class="sxs-lookup"><span data-stu-id="d5d55-139">sponsors</span></span>      |<span data-ttu-id="d5d55-140">coleção [relatedPerson](relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="d5d55-140">[relatedPerson](relatedperson.md) collection</span></span> | <span data-ttu-id="d5d55-141">A pessoa ou as pessoas que patrocinaram o projeto.</span><span class="sxs-lookup"><span data-stu-id="d5d55-141">The Person or people who sponsored the project.</span></span>                                                            |

## <a name="relationships"></a><span data-ttu-id="d5d55-142">Relações</span><span class="sxs-lookup"><span data-stu-id="d5d55-142">Relationships</span></span>

<span data-ttu-id="d5d55-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5d55-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5d55-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5d55-144">JSON representation</span></span>

<span data-ttu-id="d5d55-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5d55-145">The following is a JSON representation of the resource.</span></span>

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
