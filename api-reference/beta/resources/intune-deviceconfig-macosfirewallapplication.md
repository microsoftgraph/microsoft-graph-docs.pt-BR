---
title: tipo de recurso macOSFirewallApplication
description: Representa um aplicativo na lista de aplicativos de firewall do macOS
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 477911dba492bdda09eb815aba968bb7f63955bf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145399"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="94734-103">tipo de recurso macOSFirewallApplication</span><span class="sxs-lookup"><span data-stu-id="94734-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="94734-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="94734-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94734-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="94734-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94734-106">Representa um aplicativo na lista de aplicativos de firewall do macOS</span><span class="sxs-lookup"><span data-stu-id="94734-106">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="94734-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94734-107">Properties</span></span>
|<span data-ttu-id="94734-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94734-108">Property</span></span>|<span data-ttu-id="94734-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="94734-109">Type</span></span>|<span data-ttu-id="94734-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="94734-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94734-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="94734-111">bundleId</span></span>|<span data-ttu-id="94734-112">String</span><span class="sxs-lookup"><span data-stu-id="94734-112">String</span></span>|<span data-ttu-id="94734-113">Pacoteid do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="94734-113">BundleId of the application.</span></span>|
|<span data-ttu-id="94734-114">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="94734-114">allowsIncomingConnections</span></span>|<span data-ttu-id="94734-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="94734-115">Boolean</span></span>|<span data-ttu-id="94734-116">Se as conexões de entrada são permitidas ou não.</span><span class="sxs-lookup"><span data-stu-id="94734-116">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94734-117">Relações</span><span class="sxs-lookup"><span data-stu-id="94734-117">Relationships</span></span>
<span data-ttu-id="94734-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94734-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94734-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94734-119">JSON Representation</span></span>
<span data-ttu-id="94734-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94734-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSFirewallApplication"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSFirewallApplication",
  "bundleId": "String",
  "allowsIncomingConnections": true
}
```




