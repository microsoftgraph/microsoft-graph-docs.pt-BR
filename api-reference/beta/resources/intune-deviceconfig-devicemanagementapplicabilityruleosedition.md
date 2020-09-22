---
title: tipo de recurso deviceManagementApplicabilityRuleOsEdition
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a2e145f54116272687683789e67cbab3e6429bf4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985941"
---
# <a name="devicemanagementapplicabilityruleosedition-resource-type"></a><span data-ttu-id="addfc-103">tipo de recurso deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="addfc-103">deviceManagementApplicabilityRuleOsEdition resource type</span></span>

<span data-ttu-id="addfc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="addfc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="addfc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="addfc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="addfc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="addfc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="addfc-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="addfc-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="addfc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="addfc-108">Properties</span></span>
|<span data-ttu-id="addfc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="addfc-109">Property</span></span>|<span data-ttu-id="addfc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="addfc-110">Type</span></span>|<span data-ttu-id="addfc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="addfc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="addfc-112">osEditionTypes</span><span class="sxs-lookup"><span data-stu-id="addfc-112">osEditionTypes</span></span>|<span data-ttu-id="addfc-113">coleção [windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md)</span><span class="sxs-lookup"><span data-stu-id="addfc-113">[windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md) collection</span></span>|<span data-ttu-id="addfc-114">Tipo de edição de so da regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="addfc-114">Applicability rule OS edition type.</span></span>|
|<span data-ttu-id="addfc-115">nome</span><span class="sxs-lookup"><span data-stu-id="addfc-115">name</span></span>|<span data-ttu-id="addfc-116">String</span><span class="sxs-lookup"><span data-stu-id="addfc-116">String</span></span>|<span data-ttu-id="addfc-117">Nome do objeto.</span><span class="sxs-lookup"><span data-stu-id="addfc-117">Name for object.</span></span>|
|<span data-ttu-id="addfc-118">ruleType</span><span class="sxs-lookup"><span data-stu-id="addfc-118">ruleType</span></span>|[<span data-ttu-id="addfc-119">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="addfc-119">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="addfc-120">Tipo de regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="addfc-120">Applicability Rule type.</span></span> <span data-ttu-id="addfc-121">Os valores possíveis são: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="addfc-121">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="addfc-122">Relações</span><span class="sxs-lookup"><span data-stu-id="addfc-122">Relationships</span></span>
<span data-ttu-id="addfc-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="addfc-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="addfc-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="addfc-124">JSON Representation</span></span>
<span data-ttu-id="addfc-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="addfc-125">Here is a JSON representation of the resource.</span></span>
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






