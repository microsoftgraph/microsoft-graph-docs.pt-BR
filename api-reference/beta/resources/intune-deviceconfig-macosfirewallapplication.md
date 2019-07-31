---
title: tipo de recurso macOSFirewallApplication
description: Representa um aplicativo na lista de aplicativos de firewall do macOS
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ecd256445a54049149943d14f081f55877be240d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000981"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="45d7f-103">tipo de recurso macOSFirewallApplication</span><span class="sxs-lookup"><span data-stu-id="45d7f-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="45d7f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45d7f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45d7f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45d7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45d7f-106">Representa um aplicativo na lista de aplicativos de firewall do macOS</span><span class="sxs-lookup"><span data-stu-id="45d7f-106">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="45d7f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="45d7f-107">Properties</span></span>
|<span data-ttu-id="45d7f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45d7f-108">Property</span></span>|<span data-ttu-id="45d7f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="45d7f-109">Type</span></span>|<span data-ttu-id="45d7f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="45d7f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45d7f-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="45d7f-111">bundleId</span></span>|<span data-ttu-id="45d7f-112">String</span><span class="sxs-lookup"><span data-stu-id="45d7f-112">String</span></span>|<span data-ttu-id="45d7f-113">Pacoteid do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="45d7f-113">BundleId of the application.</span></span>|
|<span data-ttu-id="45d7f-114">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="45d7f-114">allowsIncomingConnections</span></span>|<span data-ttu-id="45d7f-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="45d7f-115">Boolean</span></span>|<span data-ttu-id="45d7f-116">Se as conexões de entrada são permitidas ou não.</span><span class="sxs-lookup"><span data-stu-id="45d7f-116">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45d7f-117">Relações</span><span class="sxs-lookup"><span data-stu-id="45d7f-117">Relationships</span></span>
<span data-ttu-id="45d7f-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="45d7f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45d7f-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="45d7f-119">JSON Representation</span></span>
<span data-ttu-id="45d7f-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="45d7f-120">Here is a JSON representation of the resource.</span></span>
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





