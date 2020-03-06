---
title: tipo de recurso deviceManagementTroubleshootingErrorDetails
description: Objeto contendo informações detalhadas sobre o erro e sua correção.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6fea29d21c34ab123ba5c573b2a19858cd3bf756
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523384"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="8ab76-103">tipo de recurso deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="8ab76-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

<span data-ttu-id="8ab76-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ab76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ab76-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8ab76-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ab76-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8ab76-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ab76-107">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="8ab76-107">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="8ab76-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ab76-108">Properties</span></span>
|<span data-ttu-id="8ab76-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ab76-109">Property</span></span>|<span data-ttu-id="8ab76-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ab76-110">Type</span></span>|<span data-ttu-id="8ab76-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ab76-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ab76-112">context</span><span class="sxs-lookup"><span data-stu-id="8ab76-112">context</span></span>|<span data-ttu-id="8ab76-113">String</span><span class="sxs-lookup"><span data-stu-id="8ab76-113">String</span></span>|<span data-ttu-id="8ab76-114">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8ab76-114">Not yet documented</span></span>|
|<span data-ttu-id="8ab76-115">alguma</span><span class="sxs-lookup"><span data-stu-id="8ab76-115">failure</span></span>|<span data-ttu-id="8ab76-116">String</span><span class="sxs-lookup"><span data-stu-id="8ab76-116">String</span></span>|<span data-ttu-id="8ab76-117">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8ab76-117">Not yet documented</span></span>|
|<span data-ttu-id="8ab76-118">failureDetails</span><span class="sxs-lookup"><span data-stu-id="8ab76-118">failureDetails</span></span>|<span data-ttu-id="8ab76-119">String</span><span class="sxs-lookup"><span data-stu-id="8ab76-119">String</span></span>|<span data-ttu-id="8ab76-120">A descrição detalhada do que deu errado.</span><span class="sxs-lookup"><span data-stu-id="8ab76-120">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="8ab76-121">correção</span><span class="sxs-lookup"><span data-stu-id="8ab76-121">remediation</span></span>|<span data-ttu-id="8ab76-122">String</span><span class="sxs-lookup"><span data-stu-id="8ab76-122">String</span></span>|<span data-ttu-id="8ab76-123">A descrição detalhada de como corrigir esse problema.</span><span class="sxs-lookup"><span data-stu-id="8ab76-123">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="8ab76-124">recursos</span><span class="sxs-lookup"><span data-stu-id="8ab76-124">resources</span></span>|<span data-ttu-id="8ab76-125">coleção [deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)</span><span class="sxs-lookup"><span data-stu-id="8ab76-125">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="8ab76-126">Links para a documentação útil sobre esta falha.</span><span class="sxs-lookup"><span data-stu-id="8ab76-126">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ab76-127">Relações</span><span class="sxs-lookup"><span data-stu-id="8ab76-127">Relationships</span></span>
<span data-ttu-id="8ab76-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8ab76-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ab76-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ab76-129">JSON Representation</span></span>
<span data-ttu-id="8ab76-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ab76-130">Here is a JSON representation of the resource.</span></span>
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



