---
title: tipo de recurso de macOSFirewallApplication
description: Representa um aplicativo na lista de aplicativos de firewall macOS
author: tfitzmac
ms.openlocfilehash: 0d248194eed1b6e1841d2e4533aa1f79b772ccc0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302720"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="c656e-103">tipo de recurso de macOSFirewallApplication</span><span class="sxs-lookup"><span data-stu-id="c656e-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="c656e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c656e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c656e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c656e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c656e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c656e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c656e-107">Representa um aplicativo na lista de aplicativos de firewall macOS</span><span class="sxs-lookup"><span data-stu-id="c656e-107">Represents an app in the list of macOS firewall applications</span></span>
## <a name="properties"></a><span data-ttu-id="c656e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c656e-108">Properties</span></span>
|<span data-ttu-id="c656e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c656e-109">Property</span></span>|<span data-ttu-id="c656e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c656e-110">Type</span></span>|<span data-ttu-id="c656e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c656e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c656e-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="c656e-112">bundleId</span></span>|<span data-ttu-id="c656e-113">String</span><span class="sxs-lookup"><span data-stu-id="c656e-113">String</span></span>|<span data-ttu-id="c656e-114">BundleId do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c656e-114">BundleId of the application.</span></span>|
|<span data-ttu-id="c656e-115">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="c656e-115">allowsIncomingConnections</span></span>|<span data-ttu-id="c656e-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="c656e-116">Boolean</span></span>|<span data-ttu-id="c656e-117">Ou não são permitidas conexões de entrada.</span><span class="sxs-lookup"><span data-stu-id="c656e-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c656e-118">Relações</span><span class="sxs-lookup"><span data-stu-id="c656e-118">Relationships</span></span>
<span data-ttu-id="c656e-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c656e-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c656e-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c656e-120">JSON Representation</span></span>
<span data-ttu-id="c656e-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c656e-121">Here is a JSON representation of the resource.</span></span>
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





