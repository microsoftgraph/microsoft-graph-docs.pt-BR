---
title: tipo de recurso deviceManagementApplicabilityRuleOsEdition
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cff458e69d0394ce3e74f2faab29bec9cfe2ea50
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49283494"
---
# <a name="devicemanagementapplicabilityruleosedition-resource-type"></a><span data-ttu-id="31501-103">tipo de recurso deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="31501-103">deviceManagementApplicabilityRuleOsEdition resource type</span></span>

<span data-ttu-id="31501-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31501-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31501-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="31501-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31501-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="31501-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31501-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="31501-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="31501-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="31501-108">Properties</span></span>
|<span data-ttu-id="31501-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31501-109">Property</span></span>|<span data-ttu-id="31501-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="31501-110">Type</span></span>|<span data-ttu-id="31501-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="31501-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31501-112">osEditionTypes</span><span class="sxs-lookup"><span data-stu-id="31501-112">osEditionTypes</span></span>|<span data-ttu-id="31501-113">coleção [windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md)</span><span class="sxs-lookup"><span data-stu-id="31501-113">[windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md) collection</span></span>|<span data-ttu-id="31501-114">Tipo de edição de so da regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="31501-114">Applicability rule OS edition type.</span></span>|
|<span data-ttu-id="31501-115">nome</span><span class="sxs-lookup"><span data-stu-id="31501-115">name</span></span>|<span data-ttu-id="31501-116">String</span><span class="sxs-lookup"><span data-stu-id="31501-116">String</span></span>|<span data-ttu-id="31501-117">Nome do objeto.</span><span class="sxs-lookup"><span data-stu-id="31501-117">Name for object.</span></span>|
|<span data-ttu-id="31501-118">ruleType</span><span class="sxs-lookup"><span data-stu-id="31501-118">ruleType</span></span>|[<span data-ttu-id="31501-119">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="31501-119">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="31501-120">Tipo de regra de aplicabilidade.</span><span class="sxs-lookup"><span data-stu-id="31501-120">Applicability Rule type.</span></span> <span data-ttu-id="31501-121">Os valores possíveis são: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="31501-121">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31501-122">Relações</span><span class="sxs-lookup"><span data-stu-id="31501-122">Relationships</span></span>
<span data-ttu-id="31501-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="31501-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="31501-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="31501-124">JSON Representation</span></span>
<span data-ttu-id="31501-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="31501-125">Here is a JSON representation of the resource.</span></span>
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




