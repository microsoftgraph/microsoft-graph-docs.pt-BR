---
title: tipo de recurso deviceManagementApplicabilityRuleOsVersion
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ef95a393f04bb233d46d52470b6714f7a5ec88b0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42792014"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a><span data-ttu-id="1014b-103">tipo de recurso deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1014b-103">deviceManagementApplicabilityRuleOsVersion resource type</span></span>

> <span data-ttu-id="1014b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1014b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1014b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1014b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1014b-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1014b-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1014b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1014b-107">Properties</span></span>
|<span data-ttu-id="1014b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1014b-108">Property</span></span>|<span data-ttu-id="1014b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1014b-109">Type</span></span>|<span data-ttu-id="1014b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1014b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1014b-111">minOSVersion</span><span class="sxs-lookup"><span data-stu-id="1014b-111">minOSVersion</span></span>|<span data-ttu-id="1014b-112">String</span><span class="sxs-lookup"><span data-stu-id="1014b-112">String</span></span>|<span data-ttu-id="1014b-113">Versão mínima do sistema operacional para regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="1014b-113">Min OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="1014b-114">maxOSVersion</span><span class="sxs-lookup"><span data-stu-id="1014b-114">maxOSVersion</span></span>|<span data-ttu-id="1014b-115">String</span><span class="sxs-lookup"><span data-stu-id="1014b-115">String</span></span>|<span data-ttu-id="1014b-116">Versão do sistema operacional máximo para a regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="1014b-116">Max OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="1014b-117">nome</span><span class="sxs-lookup"><span data-stu-id="1014b-117">name</span></span>|<span data-ttu-id="1014b-118">String</span><span class="sxs-lookup"><span data-stu-id="1014b-118">String</span></span>|<span data-ttu-id="1014b-119">Nome do objeto.</span><span class="sxs-lookup"><span data-stu-id="1014b-119">Name for object.</span></span>|
|<span data-ttu-id="1014b-120">ruleType</span><span class="sxs-lookup"><span data-stu-id="1014b-120">ruleType</span></span>|[<span data-ttu-id="1014b-121">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="1014b-121">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="1014b-122">Tipo de regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="1014b-122">Applicability Rule type.</span></span> <span data-ttu-id="1014b-123">Os valores possíveis são: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="1014b-123">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1014b-124">Relações</span><span class="sxs-lookup"><span data-stu-id="1014b-124">Relationships</span></span>
<span data-ttu-id="1014b-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1014b-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1014b-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1014b-126">JSON Representation</span></span>
<span data-ttu-id="1014b-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1014b-127">Here is a JSON representation of the resource.</span></span>
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



