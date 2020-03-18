---
title: tipo de recurso deviceManagementApplicabilityRuleOsEdition
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c6222c6f672ce8401790acdeebff1db45ae17c63
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42792028"
---
# <a name="devicemanagementapplicabilityruleosedition-resource-type"></a><span data-ttu-id="be39d-103">tipo de recurso deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="be39d-103">deviceManagementApplicabilityRuleOsEdition resource type</span></span>

> <span data-ttu-id="be39d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="be39d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be39d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="be39d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be39d-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="be39d-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="be39d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="be39d-107">Properties</span></span>
|<span data-ttu-id="be39d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be39d-108">Property</span></span>|<span data-ttu-id="be39d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="be39d-109">Type</span></span>|<span data-ttu-id="be39d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="be39d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be39d-111">osEditionTypes</span><span class="sxs-lookup"><span data-stu-id="be39d-111">osEditionTypes</span></span>|<span data-ttu-id="be39d-112">coleção [windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md)</span><span class="sxs-lookup"><span data-stu-id="be39d-112">[windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md) collection</span></span>|<span data-ttu-id="be39d-113">Tipo de edição de so da regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="be39d-113">Applicability rule OS edition type.</span></span>|
|<span data-ttu-id="be39d-114">nome</span><span class="sxs-lookup"><span data-stu-id="be39d-114">name</span></span>|<span data-ttu-id="be39d-115">String</span><span class="sxs-lookup"><span data-stu-id="be39d-115">String</span></span>|<span data-ttu-id="be39d-116">Nome do objeto.</span><span class="sxs-lookup"><span data-stu-id="be39d-116">Name for object.</span></span>|
|<span data-ttu-id="be39d-117">ruleType</span><span class="sxs-lookup"><span data-stu-id="be39d-117">ruleType</span></span>|[<span data-ttu-id="be39d-118">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="be39d-118">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="be39d-119">Tipo de regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="be39d-119">Applicability Rule type.</span></span> <span data-ttu-id="be39d-120">Os valores possíveis são: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="be39d-120">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be39d-121">Relações</span><span class="sxs-lookup"><span data-stu-id="be39d-121">Relationships</span></span>
<span data-ttu-id="be39d-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="be39d-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be39d-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="be39d-123">JSON Representation</span></span>
<span data-ttu-id="be39d-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="be39d-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
  "osEditionTypes": [
    "String"
  ],
  "name": "String",
  "ruleType": "String"
}
```



