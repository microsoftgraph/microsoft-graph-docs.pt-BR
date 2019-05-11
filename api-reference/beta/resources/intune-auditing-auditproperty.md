---
title: Tipo de recurso auditProperty
description: Uma classe que contém as propriedades para a Propriedade de auditoria.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c252e7912f3f34e300e1f412db63133ea3acbd8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949357"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="a88ad-103">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="a88ad-103">auditProperty resource type</span></span>

> <span data-ttu-id="a88ad-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a88ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a88ad-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a88ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a88ad-106">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="a88ad-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="a88ad-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a88ad-107">Properties</span></span>
|<span data-ttu-id="a88ad-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a88ad-108">Property</span></span>|<span data-ttu-id="a88ad-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a88ad-109">Type</span></span>|<span data-ttu-id="a88ad-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a88ad-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a88ad-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a88ad-111">displayName</span></span>|<span data-ttu-id="a88ad-112">String</span><span class="sxs-lookup"><span data-stu-id="a88ad-112">String</span></span>|<span data-ttu-id="a88ad-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="a88ad-113">Display name.</span></span>|
|<span data-ttu-id="a88ad-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="a88ad-114">oldValue</span></span>|<span data-ttu-id="a88ad-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a88ad-115">String</span></span>|<span data-ttu-id="a88ad-116">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="a88ad-116">Old value.</span></span>|
|<span data-ttu-id="a88ad-117">newValue</span><span class="sxs-lookup"><span data-stu-id="a88ad-117">newValue</span></span>|<span data-ttu-id="a88ad-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a88ad-118">String</span></span>|<span data-ttu-id="a88ad-119">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="a88ad-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a88ad-120">Relações</span><span class="sxs-lookup"><span data-stu-id="a88ad-120">Relationships</span></span>
<span data-ttu-id="a88ad-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a88ad-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a88ad-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a88ad-122">JSON Representation</span></span>
<span data-ttu-id="a88ad-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a88ad-123">Here is a JSON representation of the resource.</span></span>
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




