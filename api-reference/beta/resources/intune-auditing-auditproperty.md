---
title: Tipo de recurso auditProperty
description: Uma classe que contém as propriedades para a Propriedade de auditoria.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3f1f5cc213f99300811c627692a516ac8c0b6e89
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797420"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="fc071-103">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="fc071-103">auditProperty resource type</span></span>

> <span data-ttu-id="fc071-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fc071-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc071-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fc071-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc071-106">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="fc071-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="fc071-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc071-107">Properties</span></span>
|<span data-ttu-id="fc071-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc071-108">Property</span></span>|<span data-ttu-id="fc071-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc071-109">Type</span></span>|<span data-ttu-id="fc071-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc071-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc071-111">displayName</span><span class="sxs-lookup"><span data-stu-id="fc071-111">displayName</span></span>|<span data-ttu-id="fc071-112">String</span><span class="sxs-lookup"><span data-stu-id="fc071-112">String</span></span>|<span data-ttu-id="fc071-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="fc071-113">Display name.</span></span>|
|<span data-ttu-id="fc071-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="fc071-114">oldValue</span></span>|<span data-ttu-id="fc071-115">String</span><span class="sxs-lookup"><span data-stu-id="fc071-115">String</span></span>|<span data-ttu-id="fc071-116">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="fc071-116">Old value.</span></span>|
|<span data-ttu-id="fc071-117">newValue</span><span class="sxs-lookup"><span data-stu-id="fc071-117">newValue</span></span>|<span data-ttu-id="fc071-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fc071-118">String</span></span>|<span data-ttu-id="fc071-119">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="fc071-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc071-120">Relações</span><span class="sxs-lookup"><span data-stu-id="fc071-120">Relationships</span></span>
<span data-ttu-id="fc071-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc071-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc071-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc071-122">JSON Representation</span></span>
<span data-ttu-id="fc071-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc071-123">Here is a JSON representation of the resource.</span></span>
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



