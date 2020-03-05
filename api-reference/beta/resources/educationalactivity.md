---
title: tipo de recurso educationalActivity
description: tipo de recurso educationalActivity
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: e1f4ffd3154700f59ebdd26a2213755810b561ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502841"
---
# <a name="educationalactivity-resource-type"></a><span data-ttu-id="886d9-103">tipo de recurso educationalActivity</span><span class="sxs-lookup"><span data-stu-id="886d9-103">educationalActivity resource type</span></span>

<span data-ttu-id="886d9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="886d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="886d9-105">Representa os dados que um usuário forneceu relacionados ao Undergraduate, graduado, dograduação ou outras atividades educacionais.</span><span class="sxs-lookup"><span data-stu-id="886d9-105">Represents data that a user has supplied related to undergraduate, graduate, postgraduate or other educational activities.</span></span>

<span data-ttu-id="886d9-106">Herda as propriedades de metadados de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="886d9-106">Inherits metadata properties from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="886d9-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="886d9-107">Methods</span></span>

| <span data-ttu-id="886d9-108">Método</span><span class="sxs-lookup"><span data-stu-id="886d9-108">Method</span></span>                                                       | <span data-ttu-id="886d9-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="886d9-109">Return Type</span></span>                                   | <span data-ttu-id="886d9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="886d9-110">Description</span></span>                                                      |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="886d9-111">Obter educationalActivity</span><span class="sxs-lookup"><span data-stu-id="886d9-111">Get educationalActivity</span></span>](../api/educationalactivity-get.md) | [<span data-ttu-id="886d9-112">educationalActivity</span><span class="sxs-lookup"><span data-stu-id="886d9-112">educationalActivity</span></span>](educationalactivity.md) | <span data-ttu-id="886d9-113">Leia as propriedades e os relacionamentos do objeto educationalActivity.</span><span class="sxs-lookup"><span data-stu-id="886d9-113">Read properties and relationships of educationalActivity object.</span></span> |
| [<span data-ttu-id="886d9-114">Update</span><span class="sxs-lookup"><span data-stu-id="886d9-114">Update</span></span>](../api/educationalactivity-update.md)               | [<span data-ttu-id="886d9-115">educationalActivity</span><span class="sxs-lookup"><span data-stu-id="886d9-115">educationalActivity</span></span>](educationalactivity.md) | <span data-ttu-id="886d9-116">Atualize o objeto educationalActivity.</span><span class="sxs-lookup"><span data-stu-id="886d9-116">Update educationalActivity object.</span></span>                               |
| [<span data-ttu-id="886d9-117">Delete</span><span class="sxs-lookup"><span data-stu-id="886d9-117">Delete</span></span>](../api/educationalactivity-delete.md)               | <span data-ttu-id="886d9-118">None</span><span class="sxs-lookup"><span data-stu-id="886d9-118">None</span></span>                                          | <span data-ttu-id="886d9-119">Exclua o objeto educationalActivity.</span><span class="sxs-lookup"><span data-stu-id="886d9-119">Delete educationalActivity object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="886d9-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="886d9-120">Properties</span></span>

| <span data-ttu-id="886d9-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="886d9-121">Property</span></span>           | <span data-ttu-id="886d9-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="886d9-122">Type</span></span>                                                      | <span data-ttu-id="886d9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="886d9-123">Description</span></span>                                                                |
|:-------------------|:----------------------------------------------------------|:---------------------------------------------------------------------------|
|<span data-ttu-id="886d9-124">completionMonthYear</span><span class="sxs-lookup"><span data-stu-id="886d9-124">completionMonthYear</span></span> |<span data-ttu-id="886d9-125">Data</span><span class="sxs-lookup"><span data-stu-id="886d9-125">Date</span></span>                                                       |<span data-ttu-id="886d9-126">O mês e o ano em que o usuário formou ou concluiu a atividade.</span><span class="sxs-lookup"><span data-stu-id="886d9-126">The month and year the user graduated or completed the activity.</span></span>            |
|<span data-ttu-id="886d9-127">endMonthYear</span><span class="sxs-lookup"><span data-stu-id="886d9-127">endMonthYear</span></span>        |<span data-ttu-id="886d9-128">Data</span><span class="sxs-lookup"><span data-stu-id="886d9-128">Date</span></span>                                                       |<span data-ttu-id="886d9-129">O mês e o ano em que o usuário concluiu a atividade educacional referenciada.</span><span class="sxs-lookup"><span data-stu-id="886d9-129">The month and year the user completed the educational activity referenced.</span></span>  |
|<span data-ttu-id="886d9-130">instituição</span><span class="sxs-lookup"><span data-stu-id="886d9-130">institution</span></span>         |[<span data-ttu-id="886d9-131">institutionData</span><span class="sxs-lookup"><span data-stu-id="886d9-131">institutionData</span></span>](institutiondata.md)                      |<span data-ttu-id="886d9-132">Contém detalhes da instituição estudada em.</span><span class="sxs-lookup"><span data-stu-id="886d9-132">Contains details of the institution studied at.</span></span>                             |
|<span data-ttu-id="886d9-133">programa</span><span class="sxs-lookup"><span data-stu-id="886d9-133">program</span></span>             |[<span data-ttu-id="886d9-134">educationalActivityDetail</span><span class="sxs-lookup"><span data-stu-id="886d9-134">educationalActivityDetail</span></span>](educationalactivitydetail.md)  |<span data-ttu-id="886d9-135">Contém informações estendidas sobre o programa ou o curso.</span><span class="sxs-lookup"><span data-stu-id="886d9-135">Contains extended information about the program or course.</span></span>                  |
|<span data-ttu-id="886d9-136">startMonthYear</span><span class="sxs-lookup"><span data-stu-id="886d9-136">startMonthYear</span></span>      |<span data-ttu-id="886d9-137">Data</span><span class="sxs-lookup"><span data-stu-id="886d9-137">Date</span></span>                                                       |<span data-ttu-id="886d9-138">O mês e o ano em que o usuário tiver iniciado a atividade referenciada.</span><span class="sxs-lookup"><span data-stu-id="886d9-138">The month and year the user commenced the activity referenced.</span></span>              |

## <a name="relationships"></a><span data-ttu-id="886d9-139">Relações</span><span class="sxs-lookup"><span data-stu-id="886d9-139">Relationships</span></span>

<span data-ttu-id="886d9-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="886d9-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="886d9-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="886d9-141">JSON representation</span></span>

<span data-ttu-id="886d9-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="886d9-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationalActivity",
  "baseType": ""
}-->

```json
{
  "completionMonthYear": "String (timestamp)",
  "endMonthYear": "String (timestamp)",
  "institution": {"@odata.type": "microsoft.graph.institutionData"},
  "program": {"@odata.type": "microsoft.graph.educationalActivityDetail"},
  "startMonthYear": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationalActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->