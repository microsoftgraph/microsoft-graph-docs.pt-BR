---
title: tipo de recurso deviceManagementApplicabilityRuleOsVersion
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cdd0e5c7a700932af5c5ffa4dd568c252dcf9848
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724576"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a><span data-ttu-id="124a0-103">tipo de recurso deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="124a0-103">deviceManagementApplicabilityRuleOsVersion resource type</span></span>

<span data-ttu-id="124a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="124a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="124a0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="124a0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="124a0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="124a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="124a0-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="124a0-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="124a0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="124a0-108">Properties</span></span>
|<span data-ttu-id="124a0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="124a0-109">Property</span></span>|<span data-ttu-id="124a0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="124a0-110">Type</span></span>|<span data-ttu-id="124a0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="124a0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="124a0-112">minOSVersion</span><span class="sxs-lookup"><span data-stu-id="124a0-112">minOSVersion</span></span>|<span data-ttu-id="124a0-113">String</span><span class="sxs-lookup"><span data-stu-id="124a0-113">String</span></span>|<span data-ttu-id="124a0-114">Versão mínima do sistema operacional para regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="124a0-114">Min OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="124a0-115">maxOSVersion</span><span class="sxs-lookup"><span data-stu-id="124a0-115">maxOSVersion</span></span>|<span data-ttu-id="124a0-116">String</span><span class="sxs-lookup"><span data-stu-id="124a0-116">String</span></span>|<span data-ttu-id="124a0-117">Versão do sistema operacional máximo para a regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="124a0-117">Max OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="124a0-118">nome</span><span class="sxs-lookup"><span data-stu-id="124a0-118">name</span></span>|<span data-ttu-id="124a0-119">String</span><span class="sxs-lookup"><span data-stu-id="124a0-119">String</span></span>|<span data-ttu-id="124a0-120">Nome do objeto.</span><span class="sxs-lookup"><span data-stu-id="124a0-120">Name for object.</span></span>|
|<span data-ttu-id="124a0-121">ruleType</span><span class="sxs-lookup"><span data-stu-id="124a0-121">ruleType</span></span>|[<span data-ttu-id="124a0-122">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="124a0-122">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="124a0-123">Tipo de regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="124a0-123">Applicability Rule type.</span></span> <span data-ttu-id="124a0-124">Os valores possíveis são: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="124a0-124">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="124a0-125">Relações</span><span class="sxs-lookup"><span data-stu-id="124a0-125">Relationships</span></span>
<span data-ttu-id="124a0-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="124a0-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="124a0-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="124a0-127">JSON Representation</span></span>
<span data-ttu-id="124a0-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="124a0-128">Here is a JSON representation of the resource.</span></span>
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





