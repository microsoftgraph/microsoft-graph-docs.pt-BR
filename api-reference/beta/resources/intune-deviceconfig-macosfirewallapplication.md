---
title: tipo de recurso macOSFirewallApplication
description: Representa um aplicativo na lista de aplicativos de firewall do macOS
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bac45dfa350dc293fcb7957e45a2698e7f179bfb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464147"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="b0323-103">tipo de recurso macOSFirewallApplication</span><span class="sxs-lookup"><span data-stu-id="b0323-103">macOSFirewallApplication resource type</span></span>

<span data-ttu-id="b0323-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0323-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0323-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0323-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0323-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0323-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0323-107">Representa um aplicativo na lista de aplicativos de firewall do macOS</span><span class="sxs-lookup"><span data-stu-id="b0323-107">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="b0323-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0323-108">Properties</span></span>
|<span data-ttu-id="b0323-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0323-109">Property</span></span>|<span data-ttu-id="b0323-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0323-110">Type</span></span>|<span data-ttu-id="b0323-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0323-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0323-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="b0323-112">bundleId</span></span>|<span data-ttu-id="b0323-113">String</span><span class="sxs-lookup"><span data-stu-id="b0323-113">String</span></span>|<span data-ttu-id="b0323-114">Pacoteid do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0323-114">BundleId of the application.</span></span>|
|<span data-ttu-id="b0323-115">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="b0323-115">allowsIncomingConnections</span></span>|<span data-ttu-id="b0323-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0323-116">Boolean</span></span>|<span data-ttu-id="b0323-117">Se as conexões de entrada são permitidas ou não.</span><span class="sxs-lookup"><span data-stu-id="b0323-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0323-118">Relações</span><span class="sxs-lookup"><span data-stu-id="b0323-118">Relationships</span></span>
<span data-ttu-id="b0323-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0323-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0323-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0323-120">JSON Representation</span></span>
<span data-ttu-id="b0323-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0323-121">Here is a JSON representation of the resource.</span></span>
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



