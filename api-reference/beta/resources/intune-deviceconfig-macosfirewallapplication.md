---
title: tipo de recurso macOSFirewallApplication
description: Representa um aplicativo na lista de aplicativos de firewall do macOS
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 305e313dcc4dc86f71b2c4e20f29bd54d3b82e5e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366529"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="8af16-103">tipo de recurso macOSFirewallApplication</span><span class="sxs-lookup"><span data-stu-id="8af16-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="8af16-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8af16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8af16-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8af16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8af16-106">Representa um aplicativo na lista de aplicativos de firewall do macOS</span><span class="sxs-lookup"><span data-stu-id="8af16-106">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="8af16-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8af16-107">Properties</span></span>
|<span data-ttu-id="8af16-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8af16-108">Property</span></span>|<span data-ttu-id="8af16-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8af16-109">Type</span></span>|<span data-ttu-id="8af16-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8af16-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8af16-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="8af16-111">bundleId</span></span>|<span data-ttu-id="8af16-112">String</span><span class="sxs-lookup"><span data-stu-id="8af16-112">String</span></span>|<span data-ttu-id="8af16-113">Pacoteid do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8af16-113">BundleId of the application.</span></span>|
|<span data-ttu-id="8af16-114">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="8af16-114">allowsIncomingConnections</span></span>|<span data-ttu-id="8af16-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="8af16-115">Boolean</span></span>|<span data-ttu-id="8af16-116">Se as conexões de entrada são permitidas ou não.</span><span class="sxs-lookup"><span data-stu-id="8af16-116">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8af16-117">Relações</span><span class="sxs-lookup"><span data-stu-id="8af16-117">Relationships</span></span>
<span data-ttu-id="8af16-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8af16-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8af16-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8af16-119">JSON Representation</span></span>
<span data-ttu-id="8af16-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8af16-120">Here is a JSON representation of the resource.</span></span>
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



