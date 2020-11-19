---
title: tipo de recurso macOSFirewallApplication
description: Representa um aplicativo na lista de aplicativos de firewall do macOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dd6aed2dcb1f6a593109f3d7c3f6ab012caf3937
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279889"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="b893a-103">tipo de recurso macOSFirewallApplication</span><span class="sxs-lookup"><span data-stu-id="b893a-103">macOSFirewallApplication resource type</span></span>

<span data-ttu-id="b893a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b893a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b893a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b893a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b893a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b893a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b893a-107">Representa um aplicativo na lista de aplicativos de firewall do macOS</span><span class="sxs-lookup"><span data-stu-id="b893a-107">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="b893a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b893a-108">Properties</span></span>
|<span data-ttu-id="b893a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b893a-109">Property</span></span>|<span data-ttu-id="b893a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b893a-110">Type</span></span>|<span data-ttu-id="b893a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b893a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b893a-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="b893a-112">bundleId</span></span>|<span data-ttu-id="b893a-113">String</span><span class="sxs-lookup"><span data-stu-id="b893a-113">String</span></span>|<span data-ttu-id="b893a-114">Pacoteid do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b893a-114">BundleId of the application.</span></span>|
|<span data-ttu-id="b893a-115">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="b893a-115">allowsIncomingConnections</span></span>|<span data-ttu-id="b893a-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="b893a-116">Boolean</span></span>|<span data-ttu-id="b893a-117">Se as conexões de entrada são permitidas ou não.</span><span class="sxs-lookup"><span data-stu-id="b893a-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b893a-118">Relações</span><span class="sxs-lookup"><span data-stu-id="b893a-118">Relationships</span></span>
<span data-ttu-id="b893a-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b893a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b893a-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b893a-120">JSON Representation</span></span>
<span data-ttu-id="b893a-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b893a-121">Here is a JSON representation of the resource.</span></span>
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




