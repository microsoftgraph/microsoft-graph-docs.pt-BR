---
title: tipo de recurso deviceManagementTroubleshootingErrorDetails
description: Objeto contendo informações detalhadas sobre o erro e sua correção.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5fd96bafac19a3501160a3aadcd830be7643f576
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462262"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="25c5c-103">tipo de recurso deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="25c5c-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

<span data-ttu-id="25c5c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25c5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25c5c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="25c5c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25c5c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="25c5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25c5c-107">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="25c5c-107">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="25c5c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="25c5c-108">Properties</span></span>
|<span data-ttu-id="25c5c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25c5c-109">Property</span></span>|<span data-ttu-id="25c5c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="25c5c-110">Type</span></span>|<span data-ttu-id="25c5c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="25c5c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25c5c-112">context</span><span class="sxs-lookup"><span data-stu-id="25c5c-112">context</span></span>|<span data-ttu-id="25c5c-113">String</span><span class="sxs-lookup"><span data-stu-id="25c5c-113">String</span></span>|<span data-ttu-id="25c5c-114">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="25c5c-114">Not yet documented</span></span>|
|<span data-ttu-id="25c5c-115">alguma</span><span class="sxs-lookup"><span data-stu-id="25c5c-115">failure</span></span>|<span data-ttu-id="25c5c-116">String</span><span class="sxs-lookup"><span data-stu-id="25c5c-116">String</span></span>|<span data-ttu-id="25c5c-117">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="25c5c-117">Not yet documented</span></span>|
|<span data-ttu-id="25c5c-118">failureDetails</span><span class="sxs-lookup"><span data-stu-id="25c5c-118">failureDetails</span></span>|<span data-ttu-id="25c5c-119">String</span><span class="sxs-lookup"><span data-stu-id="25c5c-119">String</span></span>|<span data-ttu-id="25c5c-120">A descrição detalhada do que deu errado.</span><span class="sxs-lookup"><span data-stu-id="25c5c-120">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="25c5c-121">correção</span><span class="sxs-lookup"><span data-stu-id="25c5c-121">remediation</span></span>|<span data-ttu-id="25c5c-122">String</span><span class="sxs-lookup"><span data-stu-id="25c5c-122">String</span></span>|<span data-ttu-id="25c5c-123">A descrição detalhada de como corrigir esse problema.</span><span class="sxs-lookup"><span data-stu-id="25c5c-123">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="25c5c-124">recursos</span><span class="sxs-lookup"><span data-stu-id="25c5c-124">resources</span></span>|<span data-ttu-id="25c5c-125">coleção [deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)</span><span class="sxs-lookup"><span data-stu-id="25c5c-125">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="25c5c-126">Links para a documentação útil sobre esta falha.</span><span class="sxs-lookup"><span data-stu-id="25c5c-126">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25c5c-127">Relações</span><span class="sxs-lookup"><span data-stu-id="25c5c-127">Relationships</span></span>
<span data-ttu-id="25c5c-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="25c5c-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="25c5c-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="25c5c-129">JSON Representation</span></span>
<span data-ttu-id="25c5c-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="25c5c-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorDetails",
  "context": "String",
  "failure": "String",
  "failureDetails": "String",
  "remediation": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
      "text": "String",
      "link": "String"
    }
  ]
}
```



