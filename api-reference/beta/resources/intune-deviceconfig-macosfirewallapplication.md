---
title: tipo de recurso de macOSFirewallApplication
description: Representa um aplicativo na lista de aplicativos de firewall macOS
ms.openlocfilehash: 6e016f2191fd9b366bbdf5dbaef5562284a6b5ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034824"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="003c6-103">tipo de recurso de macOSFirewallApplication</span><span class="sxs-lookup"><span data-stu-id="003c6-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="003c6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="003c6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="003c6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="003c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="003c6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="003c6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="003c6-107">Representa um aplicativo na lista de aplicativos de firewall macOS</span><span class="sxs-lookup"><span data-stu-id="003c6-107">Represents an app in the list of macOS firewall applications</span></span>
## <a name="properties"></a><span data-ttu-id="003c6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="003c6-108">Properties</span></span>
|<span data-ttu-id="003c6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="003c6-109">Property</span></span>|<span data-ttu-id="003c6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="003c6-110">Type</span></span>|<span data-ttu-id="003c6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="003c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="003c6-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="003c6-112">bundleId</span></span>|<span data-ttu-id="003c6-113">String</span><span class="sxs-lookup"><span data-stu-id="003c6-113">String</span></span>|<span data-ttu-id="003c6-114">BundleId do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="003c6-114">BundleId of the application.</span></span>|
|<span data-ttu-id="003c6-115">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="003c6-115">allowsIncomingConnections</span></span>|<span data-ttu-id="003c6-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="003c6-116">Boolean</span></span>|<span data-ttu-id="003c6-117">Ou não são permitidas conexões de entrada.</span><span class="sxs-lookup"><span data-stu-id="003c6-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="003c6-118">Relações</span><span class="sxs-lookup"><span data-stu-id="003c6-118">Relationships</span></span>
<span data-ttu-id="003c6-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="003c6-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="003c6-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="003c6-120">JSON Representation</span></span>
<span data-ttu-id="003c6-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="003c6-121">Here is a JSON representation of the resource.</span></span>
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





