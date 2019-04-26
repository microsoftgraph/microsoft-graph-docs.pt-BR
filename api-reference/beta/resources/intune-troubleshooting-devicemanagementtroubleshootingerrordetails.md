---
title: tipo de recurso deviceManagementTroubleshootingErrorDetails
description: Objeto contendo informações detalhadas sobre o erro e sua correção.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6cfcbe0688836fa394237f1a25656540e401555f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554062"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="0bd6d-103">tipo de recurso deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="0bd6d-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

> <span data-ttu-id="0bd6d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0bd6d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bd6d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0bd6d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bd6d-106">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="0bd6d-106">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="0bd6d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0bd6d-107">Properties</span></span>
|<span data-ttu-id="0bd6d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bd6d-108">Property</span></span>|<span data-ttu-id="0bd6d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bd6d-109">Type</span></span>|<span data-ttu-id="0bd6d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bd6d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bd6d-111">context</span><span class="sxs-lookup"><span data-stu-id="0bd6d-111">context</span></span>|<span data-ttu-id="0bd6d-112">String</span><span class="sxs-lookup"><span data-stu-id="0bd6d-112">String</span></span>|<span data-ttu-id="0bd6d-113">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0bd6d-113">Not yet documented</span></span>|
|<span data-ttu-id="0bd6d-114">alguma</span><span class="sxs-lookup"><span data-stu-id="0bd6d-114">failure</span></span>|<span data-ttu-id="0bd6d-115">String</span><span class="sxs-lookup"><span data-stu-id="0bd6d-115">String</span></span>|<span data-ttu-id="0bd6d-116">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0bd6d-116">Not yet documented</span></span>|
|<span data-ttu-id="0bd6d-117">failureDetails</span><span class="sxs-lookup"><span data-stu-id="0bd6d-117">failureDetails</span></span>|<span data-ttu-id="0bd6d-118">String</span><span class="sxs-lookup"><span data-stu-id="0bd6d-118">String</span></span>|<span data-ttu-id="0bd6d-119">A descrição detalhada do que deu errado.</span><span class="sxs-lookup"><span data-stu-id="0bd6d-119">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="0bd6d-120">correção</span><span class="sxs-lookup"><span data-stu-id="0bd6d-120">remediation</span></span>|<span data-ttu-id="0bd6d-121">String</span><span class="sxs-lookup"><span data-stu-id="0bd6d-121">String</span></span>|<span data-ttu-id="0bd6d-122">A descrição detalhada de como corrigir esse problema.</span><span class="sxs-lookup"><span data-stu-id="0bd6d-122">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="0bd6d-123">recursos</span><span class="sxs-lookup"><span data-stu-id="0bd6d-123">resources</span></span>|<span data-ttu-id="0bd6d-124">coleção [deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)</span><span class="sxs-lookup"><span data-stu-id="0bd6d-124">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="0bd6d-125">Links para a documentação útil sobre esta falha.</span><span class="sxs-lookup"><span data-stu-id="0bd6d-125">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0bd6d-126">Relações</span><span class="sxs-lookup"><span data-stu-id="0bd6d-126">Relationships</span></span>
<span data-ttu-id="0bd6d-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0bd6d-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0bd6d-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0bd6d-128">JSON Representation</span></span>
<span data-ttu-id="0bd6d-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0bd6d-129">Here is a JSON representation of the resource.</span></span>
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



