---
title: tipo de recurso deviceManagementTroubleshootingErrorDetails
description: Objeto contendo informações detalhadas sobre o erro e sua correção.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a50c749e6c6c6ddd59705bbea34f0bbd2488f9a4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939781"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="83837-103">tipo de recurso deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="83837-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

> <span data-ttu-id="83837-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="83837-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83837-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83837-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83837-106">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="83837-106">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="83837-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83837-107">Properties</span></span>
|<span data-ttu-id="83837-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83837-108">Property</span></span>|<span data-ttu-id="83837-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="83837-109">Type</span></span>|<span data-ttu-id="83837-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="83837-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83837-111">context</span><span class="sxs-lookup"><span data-stu-id="83837-111">context</span></span>|<span data-ttu-id="83837-112">String</span><span class="sxs-lookup"><span data-stu-id="83837-112">String</span></span>|<span data-ttu-id="83837-113">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83837-113">Not yet documented</span></span>|
|<span data-ttu-id="83837-114">alguma</span><span class="sxs-lookup"><span data-stu-id="83837-114">failure</span></span>|<span data-ttu-id="83837-115">String</span><span class="sxs-lookup"><span data-stu-id="83837-115">String</span></span>|<span data-ttu-id="83837-116">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83837-116">Not yet documented</span></span>|
|<span data-ttu-id="83837-117">failureDetails</span><span class="sxs-lookup"><span data-stu-id="83837-117">failureDetails</span></span>|<span data-ttu-id="83837-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83837-118">String</span></span>|<span data-ttu-id="83837-119">A descrição detalhada do que deu errado.</span><span class="sxs-lookup"><span data-stu-id="83837-119">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="83837-120">correção</span><span class="sxs-lookup"><span data-stu-id="83837-120">remediation</span></span>|<span data-ttu-id="83837-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83837-121">String</span></span>|<span data-ttu-id="83837-122">A descrição detalhada de como corrigir esse problema.</span><span class="sxs-lookup"><span data-stu-id="83837-122">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="83837-123">recursos</span><span class="sxs-lookup"><span data-stu-id="83837-123">resources</span></span>|<span data-ttu-id="83837-124">coleção [deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)</span><span class="sxs-lookup"><span data-stu-id="83837-124">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="83837-125">Links para a documentação útil sobre esta falha.</span><span class="sxs-lookup"><span data-stu-id="83837-125">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83837-126">Relações</span><span class="sxs-lookup"><span data-stu-id="83837-126">Relationships</span></span>
<span data-ttu-id="83837-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="83837-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83837-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83837-128">JSON Representation</span></span>
<span data-ttu-id="83837-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83837-129">Here is a JSON representation of the resource.</span></span>
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




