---
title: Tipo de recurso managementIntentInfo
description: Representa informações de relação para uma intenção de gerenciamento.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 9bc58ff4c850661b968e7b540de9038074406ac5
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401997"
---
# <a name="managementintentinfo-resource-type"></a><span data-ttu-id="38e3b-103">Tipo de recurso managementIntentInfo</span><span class="sxs-lookup"><span data-stu-id="38e3b-103">managementIntentInfo resource type</span></span>

<span data-ttu-id="38e3b-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="38e3b-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38e3b-105">Representa informações de relação para uma intenção de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="38e3b-105">Represents relationship information for a management intent.</span></span>

## <a name="properties"></a><span data-ttu-id="38e3b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38e3b-106">Properties</span></span>
|<span data-ttu-id="38e3b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38e3b-107">Property</span></span>|<span data-ttu-id="38e3b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="38e3b-108">Type</span></span>|<span data-ttu-id="38e3b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="38e3b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38e3b-110">managementIntentDisplayName</span><span class="sxs-lookup"><span data-stu-id="38e3b-110">managementIntentDisplayName</span></span>|<span data-ttu-id="38e3b-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38e3b-111">String</span></span>|<span data-ttu-id="38e3b-112">O nome de exibição para a intenção de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="38e3b-112">The display name for the management intent.</span></span> <span data-ttu-id="38e3b-113">Opcional.</span><span class="sxs-lookup"><span data-stu-id="38e3b-113">Optional.</span></span> <span data-ttu-id="38e3b-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38e3b-114">Read-only.</span></span>|
|<span data-ttu-id="38e3b-115">managementIntentId</span><span class="sxs-lookup"><span data-stu-id="38e3b-115">managementIntentId</span></span>|<span data-ttu-id="38e3b-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38e3b-116">String</span></span>|<span data-ttu-id="38e3b-117">O identificador da intenção de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="38e3b-117">The identifier for the management intent.</span></span> <span data-ttu-id="38e3b-118">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38e3b-118">Required.</span></span> <span data-ttu-id="38e3b-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38e3b-119">Read-only.</span></span>|
|<span data-ttu-id="38e3b-120">managementTemplates</span><span class="sxs-lookup"><span data-stu-id="38e3b-120">managementTemplates</span></span>|<span data-ttu-id="38e3b-121">[coleção microsoft.graph.managedTenants.managementTemplateDetailedInfo](../resources/managedtenants-managementtemplatedetailedinfo.md)</span><span class="sxs-lookup"><span data-stu-id="38e3b-121">[microsoft.graph.managedTenants.managementTemplateDetailedInfo](../resources/managedtenants-managementtemplatedetailedinfo.md) collection</span></span>|<span data-ttu-id="38e3b-122">A coleção de informações do modelo de gerenciamento associadas à intenção de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="38e3b-122">The collection of management template information associated with the management intent.</span></span> <span data-ttu-id="38e3b-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="38e3b-123">Optional.</span></span> <span data-ttu-id="38e3b-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38e3b-124">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38e3b-125">Relações</span><span class="sxs-lookup"><span data-stu-id="38e3b-125">Relationships</span></span>
<span data-ttu-id="38e3b-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="38e3b-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="38e3b-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38e3b-127">JSON representation</span></span>
<span data-ttu-id="38e3b-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38e3b-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementIntentInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementIntentInfo",
  "managementIntentId": "String",
  "managementIntentDisplayName": "String",
  "managementTemplates": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementTemplateDetailedInfo"
    }
  ]
}
```
