---
title: tipo de recurso deviceManagementApplicabilityRuleOsVersion
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 99476ad2b42caf10d64f26ccd5725655ae8cac34
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49283466"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a><span data-ttu-id="f980d-103">tipo de recurso deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f980d-103">deviceManagementApplicabilityRuleOsVersion resource type</span></span>

<span data-ttu-id="f980d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f980d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f980d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f980d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f980d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f980d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f980d-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f980d-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f980d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f980d-108">Properties</span></span>
|<span data-ttu-id="f980d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f980d-109">Property</span></span>|<span data-ttu-id="f980d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f980d-110">Type</span></span>|<span data-ttu-id="f980d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f980d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f980d-112">minOSVersion</span><span class="sxs-lookup"><span data-stu-id="f980d-112">minOSVersion</span></span>|<span data-ttu-id="f980d-113">String</span><span class="sxs-lookup"><span data-stu-id="f980d-113">String</span></span>|<span data-ttu-id="f980d-114">Versão mínima do sistema operacional para regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="f980d-114">Min OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="f980d-115">maxOSVersion</span><span class="sxs-lookup"><span data-stu-id="f980d-115">maxOSVersion</span></span>|<span data-ttu-id="f980d-116">String</span><span class="sxs-lookup"><span data-stu-id="f980d-116">String</span></span>|<span data-ttu-id="f980d-117">Versão do sistema operacional máximo para a regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="f980d-117">Max OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="f980d-118">nome</span><span class="sxs-lookup"><span data-stu-id="f980d-118">name</span></span>|<span data-ttu-id="f980d-119">String</span><span class="sxs-lookup"><span data-stu-id="f980d-119">String</span></span>|<span data-ttu-id="f980d-120">Nome do objeto.</span><span class="sxs-lookup"><span data-stu-id="f980d-120">Name for object.</span></span>|
|<span data-ttu-id="f980d-121">ruleType</span><span class="sxs-lookup"><span data-stu-id="f980d-121">ruleType</span></span>|[<span data-ttu-id="f980d-122">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="f980d-122">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="f980d-123">Tipo de regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="f980d-123">Applicability Rule type.</span></span> <span data-ttu-id="f980d-124">Os valores possíveis são: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="f980d-124">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f980d-125">Relações</span><span class="sxs-lookup"><span data-stu-id="f980d-125">Relationships</span></span>
<span data-ttu-id="f980d-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f980d-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f980d-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f980d-127">JSON Representation</span></span>
<span data-ttu-id="f980d-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f980d-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
  "minOSVersion": "String",
  "maxOSVersion": "String",
  "name": "String",
  "ruleType": "String"
}
```




