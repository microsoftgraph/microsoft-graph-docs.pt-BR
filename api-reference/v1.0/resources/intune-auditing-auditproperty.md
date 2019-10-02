---
title: Tipo de recurso auditProperty
description: Uma classe que contém as propriedades para a Propriedade de auditoria.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b5330acfaa58cb5b1400851a861eb142d51b0ddb
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355978"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="73283-103">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="73283-103">auditProperty resource type</span></span>

> <span data-ttu-id="73283-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73283-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73283-105">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="73283-105">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="73283-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73283-106">Properties</span></span>
|<span data-ttu-id="73283-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73283-107">Property</span></span>|<span data-ttu-id="73283-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="73283-108">Type</span></span>|<span data-ttu-id="73283-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="73283-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73283-110">displayName</span><span class="sxs-lookup"><span data-stu-id="73283-110">displayName</span></span>|<span data-ttu-id="73283-111">String</span><span class="sxs-lookup"><span data-stu-id="73283-111">String</span></span>|<span data-ttu-id="73283-112">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="73283-112">Display name.</span></span>|
|<span data-ttu-id="73283-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="73283-113">oldValue</span></span>|<span data-ttu-id="73283-114">String</span><span class="sxs-lookup"><span data-stu-id="73283-114">String</span></span>|<span data-ttu-id="73283-115">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="73283-115">Old value.</span></span>|
|<span data-ttu-id="73283-116">newValue</span><span class="sxs-lookup"><span data-stu-id="73283-116">newValue</span></span>|<span data-ttu-id="73283-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73283-117">String</span></span>|<span data-ttu-id="73283-118">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="73283-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73283-119">Relações</span><span class="sxs-lookup"><span data-stu-id="73283-119">Relationships</span></span>
<span data-ttu-id="73283-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="73283-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="73283-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73283-121">JSON Representation</span></span>
<span data-ttu-id="73283-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="73283-122">Here is a JSON representation of the resource.</span></span>
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




