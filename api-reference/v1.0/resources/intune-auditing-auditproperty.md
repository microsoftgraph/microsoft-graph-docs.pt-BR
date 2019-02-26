---
title: Tipo de recurso auditProperty
description: Uma classe que contém as propriedades para a Propriedade de auditoria.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18e819234fd4ee7065378046f8ec977276a8c9f2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260610"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="82237-103">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="82237-103">auditProperty resource type</span></span>

> <span data-ttu-id="82237-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="82237-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82237-105">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="82237-105">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="82237-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="82237-106">Properties</span></span>
|<span data-ttu-id="82237-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82237-107">Property</span></span>|<span data-ttu-id="82237-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="82237-108">Type</span></span>|<span data-ttu-id="82237-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="82237-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82237-110">displayName</span><span class="sxs-lookup"><span data-stu-id="82237-110">displayName</span></span>|<span data-ttu-id="82237-111">String</span><span class="sxs-lookup"><span data-stu-id="82237-111">String</span></span>|<span data-ttu-id="82237-112">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="82237-112">Display name.</span></span>|
|<span data-ttu-id="82237-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="82237-113">oldValue</span></span>|<span data-ttu-id="82237-114">String</span><span class="sxs-lookup"><span data-stu-id="82237-114">String</span></span>|<span data-ttu-id="82237-115">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="82237-115">Old value.</span></span>|
|<span data-ttu-id="82237-116">newValue</span><span class="sxs-lookup"><span data-stu-id="82237-116">newValue</span></span>|<span data-ttu-id="82237-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82237-117">String</span></span>|<span data-ttu-id="82237-118">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="82237-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82237-119">Relações</span><span class="sxs-lookup"><span data-stu-id="82237-119">Relationships</span></span>
<span data-ttu-id="82237-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="82237-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82237-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="82237-121">JSON Representation</span></span>
<span data-ttu-id="82237-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="82237-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```



