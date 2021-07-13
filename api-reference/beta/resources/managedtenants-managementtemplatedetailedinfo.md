---
title: Tipo de recurso managementTemplateDetailedInfo
description: Representa informações detalhadas para o modelo de gerenciamento.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: e98d2ca41bc972a5dca33c575363b1bac27d87a5
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402107"
---
# <a name="managementtemplatedetailedinfo-resource-type"></a><span data-ttu-id="2ef9f-103">Tipo de recurso managementTemplateDetailedInfo</span><span class="sxs-lookup"><span data-stu-id="2ef9f-103">managementTemplateDetailedInfo resource type</span></span>

<span data-ttu-id="2ef9f-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="2ef9f-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ef9f-105">Representa informações detalhadas para o modelo de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="2ef9f-105">Represents detailed information for the management template.</span></span>

## <a name="properties"></a><span data-ttu-id="2ef9f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ef9f-106">Properties</span></span>
|<span data-ttu-id="2ef9f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ef9f-107">Property</span></span>|<span data-ttu-id="2ef9f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ef9f-108">Type</span></span>|<span data-ttu-id="2ef9f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ef9f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ef9f-110">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="2ef9f-110">category</span></span>|<span data-ttu-id="2ef9f-111">managementCategory</span><span class="sxs-lookup"><span data-stu-id="2ef9f-111">managementCategory</span></span>|<span data-ttu-id="2ef9f-112">A categoria de gerenciamento do modelo de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="2ef9f-112">The management category for the management template.</span></span> <span data-ttu-id="2ef9f-113">Os valores possíveis são: `custom`, `devices`, `identity`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="2ef9f-113">Possible values are: `custom`, `devices`, `identity`, `unknownFutureValue`.</span></span> <span data-ttu-id="2ef9f-114">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ef9f-114">Required.</span></span> <span data-ttu-id="2ef9f-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ef9f-115">Read-only.</span></span>|
|<span data-ttu-id="2ef9f-116">displayName</span><span class="sxs-lookup"><span data-stu-id="2ef9f-116">displayName</span></span>|<span data-ttu-id="2ef9f-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ef9f-117">String</span></span>|<span data-ttu-id="2ef9f-118">O nome de exibição do modelo de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="2ef9f-118">The display name for the management template.</span></span> <span data-ttu-id="2ef9f-119">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ef9f-119">Required.</span></span> <span data-ttu-id="2ef9f-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ef9f-120">Read-only.</span></span>|
|<span data-ttu-id="2ef9f-121">managementTemplateId</span><span class="sxs-lookup"><span data-stu-id="2ef9f-121">managementTemplateId</span></span>|<span data-ttu-id="2ef9f-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ef9f-122">String</span></span>|<span data-ttu-id="2ef9f-123">O identificador exclusivo do modelo de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="2ef9f-123">The unique identifier for the management template.</span></span> <span data-ttu-id="2ef9f-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ef9f-124">Required.</span></span> <span data-ttu-id="2ef9f-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ef9f-125">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ef9f-126">Relações</span><span class="sxs-lookup"><span data-stu-id="2ef9f-126">Relationships</span></span>
<span data-ttu-id="2ef9f-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ef9f-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ef9f-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ef9f-128">JSON representation</span></span>
<span data-ttu-id="2ef9f-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ef9f-129">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplateDetailedInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplateDetailedInfo",
  "managementTemplateId": "String",
  "displayName": "String",
  "category": "String"
}
```
