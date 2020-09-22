---
title: Tipo de recurso auditProperty
description: Uma classe que contém as propriedades para a Propriedade de auditoria.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2d30f44bdf5ca002f71ac5e1f935081b032379ec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076299"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="740c8-103">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="740c8-103">auditProperty resource type</span></span>

<span data-ttu-id="740c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="740c8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="740c8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="740c8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="740c8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="740c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="740c8-107">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="740c8-107">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="740c8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="740c8-108">Properties</span></span>
|<span data-ttu-id="740c8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="740c8-109">Property</span></span>|<span data-ttu-id="740c8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="740c8-110">Type</span></span>|<span data-ttu-id="740c8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="740c8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="740c8-112">displayName</span><span class="sxs-lookup"><span data-stu-id="740c8-112">displayName</span></span>|<span data-ttu-id="740c8-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="740c8-113">String</span></span>|<span data-ttu-id="740c8-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="740c8-114">Display name.</span></span>|
|<span data-ttu-id="740c8-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="740c8-115">oldValue</span></span>|<span data-ttu-id="740c8-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="740c8-116">String</span></span>|<span data-ttu-id="740c8-117">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="740c8-117">Old value.</span></span>|
|<span data-ttu-id="740c8-118">newValue</span><span class="sxs-lookup"><span data-stu-id="740c8-118">newValue</span></span>|<span data-ttu-id="740c8-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="740c8-119">String</span></span>|<span data-ttu-id="740c8-120">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="740c8-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="740c8-121">Relações</span><span class="sxs-lookup"><span data-stu-id="740c8-121">Relationships</span></span>
<span data-ttu-id="740c8-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="740c8-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="740c8-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="740c8-123">JSON Representation</span></span>
<span data-ttu-id="740c8-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="740c8-124">Here is a JSON representation of the resource.</span></span>
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






