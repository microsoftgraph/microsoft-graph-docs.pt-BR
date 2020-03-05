---
title: tipo de recurso deviceManagementApplicabilityRuleOsVersion
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ef729e66f5198acae1f7a123bfc4911de76c784d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526604"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a><span data-ttu-id="ef02c-103">tipo de recurso deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ef02c-103">deviceManagementApplicabilityRuleOsVersion resource type</span></span>

<span data-ttu-id="ef02c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ef02c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef02c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ef02c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef02c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ef02c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef02c-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ef02c-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ef02c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ef02c-108">Properties</span></span>
|<span data-ttu-id="ef02c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef02c-109">Property</span></span>|<span data-ttu-id="ef02c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef02c-110">Type</span></span>|<span data-ttu-id="ef02c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef02c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef02c-112">minOSVersion</span><span class="sxs-lookup"><span data-stu-id="ef02c-112">minOSVersion</span></span>|<span data-ttu-id="ef02c-113">String</span><span class="sxs-lookup"><span data-stu-id="ef02c-113">String</span></span>|<span data-ttu-id="ef02c-114">Versão mínima do sistema operacional para regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="ef02c-114">Min OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="ef02c-115">maxOSVersion</span><span class="sxs-lookup"><span data-stu-id="ef02c-115">maxOSVersion</span></span>|<span data-ttu-id="ef02c-116">String</span><span class="sxs-lookup"><span data-stu-id="ef02c-116">String</span></span>|<span data-ttu-id="ef02c-117">Versão do sistema operacional máximo para a regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="ef02c-117">Max OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="ef02c-118">nome</span><span class="sxs-lookup"><span data-stu-id="ef02c-118">name</span></span>|<span data-ttu-id="ef02c-119">String</span><span class="sxs-lookup"><span data-stu-id="ef02c-119">String</span></span>|<span data-ttu-id="ef02c-120">Nome do objeto.</span><span class="sxs-lookup"><span data-stu-id="ef02c-120">Name for object.</span></span>|
|<span data-ttu-id="ef02c-121">ruleType</span><span class="sxs-lookup"><span data-stu-id="ef02c-121">ruleType</span></span>|[<span data-ttu-id="ef02c-122">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="ef02c-122">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="ef02c-123">Tipo de regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="ef02c-123">Applicability Rule type.</span></span> <span data-ttu-id="ef02c-124">Os valores possíveis são: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="ef02c-124">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef02c-125">Relações</span><span class="sxs-lookup"><span data-stu-id="ef02c-125">Relationships</span></span>
<span data-ttu-id="ef02c-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ef02c-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef02c-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ef02c-127">JSON Representation</span></span>
<span data-ttu-id="ef02c-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ef02c-128">Here is a JSON representation of the resource.</span></span>
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



