---
title: tipo de recurso macOSFirewallApplication
description: Representa um aplicativo na lista de aplicativos de firewall do macOS
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 45d8742a888eb492b71bf9829b9621bde9608ef5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460475"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="d9c1c-103">tipo de recurso macOSFirewallApplication</span><span class="sxs-lookup"><span data-stu-id="d9c1c-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="d9c1c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9c1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9c1c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9c1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9c1c-106">Representa um aplicativo na lista de aplicativos de firewall do macOS</span><span class="sxs-lookup"><span data-stu-id="d9c1c-106">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="d9c1c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9c1c-107">Properties</span></span>
|<span data-ttu-id="d9c1c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9c1c-108">Property</span></span>|<span data-ttu-id="d9c1c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9c1c-109">Type</span></span>|<span data-ttu-id="d9c1c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9c1c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9c1c-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="d9c1c-111">bundleId</span></span>|<span data-ttu-id="d9c1c-112">String</span><span class="sxs-lookup"><span data-stu-id="d9c1c-112">String</span></span>|<span data-ttu-id="d9c1c-113">Pacoteid do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d9c1c-113">BundleId of the application.</span></span>|
|<span data-ttu-id="d9c1c-114">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="d9c1c-114">allowsIncomingConnections</span></span>|<span data-ttu-id="d9c1c-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9c1c-115">Boolean</span></span>|<span data-ttu-id="d9c1c-116">Se as conexões de entrada são permitidas ou não.</span><span class="sxs-lookup"><span data-stu-id="d9c1c-116">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9c1c-117">Relações</span><span class="sxs-lookup"><span data-stu-id="d9c1c-117">Relationships</span></span>
<span data-ttu-id="d9c1c-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d9c1c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9c1c-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9c1c-119">JSON Representation</span></span>
<span data-ttu-id="d9c1c-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d9c1c-120">Here is a JSON representation of the resource.</span></span>
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





