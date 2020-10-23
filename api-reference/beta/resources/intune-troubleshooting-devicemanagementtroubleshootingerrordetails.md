---
title: tipo de recurso deviceManagementTroubleshootingErrorDetails
description: Objeto contendo informações detalhadas sobre o erro e sua correção.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 790eac6bd48590773b4b27f59aca92546802c407
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727994"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="b8799-103">tipo de recurso deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="b8799-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

<span data-ttu-id="b8799-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8799-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8799-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b8799-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8799-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8799-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8799-107">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="b8799-107">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="b8799-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8799-108">Properties</span></span>
|<span data-ttu-id="b8799-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8799-109">Property</span></span>|<span data-ttu-id="b8799-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8799-110">Type</span></span>|<span data-ttu-id="b8799-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8799-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8799-112">context</span><span class="sxs-lookup"><span data-stu-id="b8799-112">context</span></span>|<span data-ttu-id="b8799-113">String</span><span class="sxs-lookup"><span data-stu-id="b8799-113">String</span></span>|<span data-ttu-id="b8799-114">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b8799-114">Not yet documented</span></span>|
|<span data-ttu-id="b8799-115">alguma</span><span class="sxs-lookup"><span data-stu-id="b8799-115">failure</span></span>|<span data-ttu-id="b8799-116">String</span><span class="sxs-lookup"><span data-stu-id="b8799-116">String</span></span>|<span data-ttu-id="b8799-117">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b8799-117">Not yet documented</span></span>|
|<span data-ttu-id="b8799-118">failureDetails</span><span class="sxs-lookup"><span data-stu-id="b8799-118">failureDetails</span></span>|<span data-ttu-id="b8799-119">String</span><span class="sxs-lookup"><span data-stu-id="b8799-119">String</span></span>|<span data-ttu-id="b8799-120">A descrição detalhada do que deu errado.</span><span class="sxs-lookup"><span data-stu-id="b8799-120">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="b8799-121">correção</span><span class="sxs-lookup"><span data-stu-id="b8799-121">remediation</span></span>|<span data-ttu-id="b8799-122">String</span><span class="sxs-lookup"><span data-stu-id="b8799-122">String</span></span>|<span data-ttu-id="b8799-123">A descrição detalhada de como corrigir esse problema.</span><span class="sxs-lookup"><span data-stu-id="b8799-123">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="b8799-124">recursos</span><span class="sxs-lookup"><span data-stu-id="b8799-124">resources</span></span>|<span data-ttu-id="b8799-125">coleção [deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)</span><span class="sxs-lookup"><span data-stu-id="b8799-125">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="b8799-126">Links para a documentação útil sobre esta falha.</span><span class="sxs-lookup"><span data-stu-id="b8799-126">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8799-127">Relações</span><span class="sxs-lookup"><span data-stu-id="b8799-127">Relationships</span></span>
<span data-ttu-id="b8799-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8799-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8799-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8799-129">JSON Representation</span></span>
<span data-ttu-id="b8799-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8799-130">Here is a JSON representation of the resource.</span></span>
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





