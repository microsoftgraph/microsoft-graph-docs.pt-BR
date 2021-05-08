---
title: tipo de recurso educationOrganization
description: Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização no setor educacional.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b24313b6b6061449faea0ecb4880a421a2333099
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231861"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="f1bb2-103">tipo de recurso educationOrganization</span><span class="sxs-lookup"><span data-stu-id="f1bb2-103">educationOrganization resource type</span></span>

<span data-ttu-id="f1bb2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1bb2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f1bb2-105">Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização no setor educacional.</span><span class="sxs-lookup"><span data-stu-id="f1bb2-105">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

<span data-ttu-id="f1bb2-106">Herda da [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="f1bb2-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f1bb2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1bb2-107">Properties</span></span>

| <span data-ttu-id="f1bb2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1bb2-108">Property</span></span>             | <span data-ttu-id="f1bb2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1bb2-109">Type</span></span>                    | <span data-ttu-id="f1bb2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1bb2-110">Description</span></span>                                                                            |
| :------------------- | :---------------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="f1bb2-111">description</span><span class="sxs-lookup"><span data-stu-id="f1bb2-111">description</span></span>          | <span data-ttu-id="f1bb2-112">String</span><span class="sxs-lookup"><span data-stu-id="f1bb2-112">String</span></span>                  | <span data-ttu-id="f1bb2-113">Descrição da organização.</span><span class="sxs-lookup"><span data-stu-id="f1bb2-113">Organization description.</span></span>                                                              |
| <span data-ttu-id="f1bb2-114">displayName</span><span class="sxs-lookup"><span data-stu-id="f1bb2-114">displayName</span></span>          | <span data-ttu-id="f1bb2-115">String</span><span class="sxs-lookup"><span data-stu-id="f1bb2-115">String</span></span>                  | <span data-ttu-id="f1bb2-116">Nome de exibição da organização.</span><span class="sxs-lookup"><span data-stu-id="f1bb2-116">Organization display name.</span></span>                                                             |
| <span data-ttu-id="f1bb2-117">externalSource</span><span class="sxs-lookup"><span data-stu-id="f1bb2-117">externalSource</span></span>       | <span data-ttu-id="f1bb2-118">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="f1bb2-118">educationExternalSource</span></span> | <span data-ttu-id="f1bb2-119">Fonte de onde essa organização foi criada.</span><span class="sxs-lookup"><span data-stu-id="f1bb2-119">Source where this organization was created from.</span></span> <span data-ttu-id="f1bb2-120">Os valores possíveis são: `sis` e `manual`.</span><span class="sxs-lookup"><span data-stu-id="f1bb2-120">Possible values are: `sis`, `manual`.</span></span> |
| <span data-ttu-id="f1bb2-121">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="f1bb2-121">externalSourceDetail</span></span> | <span data-ttu-id="f1bb2-122">String</span><span class="sxs-lookup"><span data-stu-id="f1bb2-122">String</span></span>                  | <span data-ttu-id="f1bb2-123">O nome da fonte externa de onde esses recursos foram gerados.</span><span class="sxs-lookup"><span data-stu-id="f1bb2-123">The name of the external source this resources was generated from.</span></span>                     |
| <span data-ttu-id="f1bb2-124">id</span><span class="sxs-lookup"><span data-stu-id="f1bb2-124">id</span></span>                   | <span data-ttu-id="f1bb2-125">String</span><span class="sxs-lookup"><span data-stu-id="f1bb2-125">String</span></span>                  | <span data-ttu-id="f1bb2-126">Identificador de objeto.</span><span class="sxs-lookup"><span data-stu-id="f1bb2-126">Object identifier.</span></span> <span data-ttu-id="f1bb2-127">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="f1bb2-127">Inherited from [entity](../resources/entity.md)</span></span>                     |

## <a name="relationships"></a><span data-ttu-id="f1bb2-128">Relações</span><span class="sxs-lookup"><span data-stu-id="f1bb2-128">Relationships</span></span>

<span data-ttu-id="f1bb2-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f1bb2-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1bb2-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1bb2-130">JSON representation</span></span>

<span data-ttu-id="f1bb2-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1bb2-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationOrganization",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationOrganization",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "externalSource": "String",
  "externalSourceDetail": "String"
}
```
