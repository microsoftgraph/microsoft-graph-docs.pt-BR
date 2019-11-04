---
title: tipo de recurso educationalActivity
description: tipo de recurso educationalActivity
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 8d060de55d765adb7e01e6b03842c569f03c8d4f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939618"
---
# <a name="educationalactivity-resource-type"></a><span data-ttu-id="4487c-103">tipo de recurso educationalActivity</span><span class="sxs-lookup"><span data-stu-id="4487c-103">educationalActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4487c-104">Representa os dados que um usuário forneceu relacionados ao Undergraduate, graduado, dograduação ou outras atividades educacionais.</span><span class="sxs-lookup"><span data-stu-id="4487c-104">Represents data that a user has supplied related to undergraduate, graduate, postgraduate or other educational activities.</span></span>

<span data-ttu-id="4487c-105">Herda as propriedades de metadados de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="4487c-105">Inherits metadata properties from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4487c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="4487c-106">Methods</span></span>

| <span data-ttu-id="4487c-107">Método</span><span class="sxs-lookup"><span data-stu-id="4487c-107">Method</span></span>                                                       | <span data-ttu-id="4487c-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4487c-108">Return Type</span></span>                                   | <span data-ttu-id="4487c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4487c-109">Description</span></span>                                                      |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="4487c-110">Obter educationalActivity</span><span class="sxs-lookup"><span data-stu-id="4487c-110">Get educationalActivity</span></span>](../api/educationalactivity-get.md) | [<span data-ttu-id="4487c-111">educationalActivity</span><span class="sxs-lookup"><span data-stu-id="4487c-111">educationalActivity</span></span>](educationalactivity.md) | <span data-ttu-id="4487c-112">Leia as propriedades e os relacionamentos do objeto educationalActivity.</span><span class="sxs-lookup"><span data-stu-id="4487c-112">Read properties and relationships of educationalActivity object.</span></span> |
| [<span data-ttu-id="4487c-113">Update</span><span class="sxs-lookup"><span data-stu-id="4487c-113">Update</span></span>](../api/educationalactivity-update.md)               | [<span data-ttu-id="4487c-114">educationalActivity</span><span class="sxs-lookup"><span data-stu-id="4487c-114">educationalActivity</span></span>](educationalactivity.md) | <span data-ttu-id="4487c-115">Atualize o objeto educationalActivity.</span><span class="sxs-lookup"><span data-stu-id="4487c-115">Update educationalActivity object.</span></span>                               |
| [<span data-ttu-id="4487c-116">Delete</span><span class="sxs-lookup"><span data-stu-id="4487c-116">Delete</span></span>](../api/educationalactivity-delete.md)               | <span data-ttu-id="4487c-117">None</span><span class="sxs-lookup"><span data-stu-id="4487c-117">None</span></span>                                          | <span data-ttu-id="4487c-118">Exclua o objeto educationalActivity.</span><span class="sxs-lookup"><span data-stu-id="4487c-118">Delete educationalActivity object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="4487c-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4487c-119">Properties</span></span>

| <span data-ttu-id="4487c-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4487c-120">Property</span></span>           | <span data-ttu-id="4487c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="4487c-121">Type</span></span>                                                      | <span data-ttu-id="4487c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4487c-122">Description</span></span>                                                                |
|:-------------------|:----------------------------------------------------------|:---------------------------------------------------------------------------|
|<span data-ttu-id="4487c-123">completionMonthYear</span><span class="sxs-lookup"><span data-stu-id="4487c-123">completionMonthYear</span></span> |<span data-ttu-id="4487c-124">Data</span><span class="sxs-lookup"><span data-stu-id="4487c-124">Date</span></span>                                                       |<span data-ttu-id="4487c-125">O mês e o ano em que o usuário formou ou concluiu a atividade.</span><span class="sxs-lookup"><span data-stu-id="4487c-125">The month and year the user graduated or completed the activity.</span></span>            |
|<span data-ttu-id="4487c-126">endMonthYear</span><span class="sxs-lookup"><span data-stu-id="4487c-126">endMonthYear</span></span>        |<span data-ttu-id="4487c-127">Data</span><span class="sxs-lookup"><span data-stu-id="4487c-127">Date</span></span>                                                       |<span data-ttu-id="4487c-128">O mês e o ano em que o usuário concluiu a atividade educacional referenciada.</span><span class="sxs-lookup"><span data-stu-id="4487c-128">The month and year the user completed the educational activity referenced.</span></span>  |
|<span data-ttu-id="4487c-129">instituição</span><span class="sxs-lookup"><span data-stu-id="4487c-129">institution</span></span>         |[<span data-ttu-id="4487c-130">institutionData</span><span class="sxs-lookup"><span data-stu-id="4487c-130">institutionData</span></span>](institutiondata.md)                      |<span data-ttu-id="4487c-131">Contém detalhes da instituição estudada em.</span><span class="sxs-lookup"><span data-stu-id="4487c-131">Contains details of the institution studied at.</span></span>                             |
|<span data-ttu-id="4487c-132">programa</span><span class="sxs-lookup"><span data-stu-id="4487c-132">program</span></span>             |[<span data-ttu-id="4487c-133">educationalActivityDetail</span><span class="sxs-lookup"><span data-stu-id="4487c-133">educationalActivityDetail</span></span>](educationalactivitydetail.md)  |<span data-ttu-id="4487c-134">Contém informações estendidas sobre o programa ou o curso.</span><span class="sxs-lookup"><span data-stu-id="4487c-134">Contains extended information about the program or course.</span></span>                  |
|<span data-ttu-id="4487c-135">startMonthYear</span><span class="sxs-lookup"><span data-stu-id="4487c-135">startMonthYear</span></span>      |<span data-ttu-id="4487c-136">Data</span><span class="sxs-lookup"><span data-stu-id="4487c-136">Date</span></span>                                                       |<span data-ttu-id="4487c-137">O mês e o ano em que o usuário tiver iniciado a atividade referenciada.</span><span class="sxs-lookup"><span data-stu-id="4487c-137">The month and year the user commenced the activity referenced.</span></span>              |

## <a name="relationships"></a><span data-ttu-id="4487c-138">Relações</span><span class="sxs-lookup"><span data-stu-id="4487c-138">Relationships</span></span>

<span data-ttu-id="4487c-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4487c-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4487c-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4487c-140">JSON representation</span></span>

<span data-ttu-id="4487c-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4487c-141">The following is a JSON representation of the resource.</span></span>

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