---
title: tipo de recurso de macOSFirewallApplication
description: Representa um aplicativo na lista de aplicativos de firewall macOS
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8ad53f1a30c19a6ab1c3e32dc0871481fbac21f8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954124"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="9ce79-103">tipo de recurso de macOSFirewallApplication</span><span class="sxs-lookup"><span data-stu-id="9ce79-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="9ce79-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9ce79-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ce79-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9ce79-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ce79-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9ce79-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ce79-107">Representa um aplicativo na lista de aplicativos de firewall macOS</span><span class="sxs-lookup"><span data-stu-id="9ce79-107">Represents an app in the list of macOS firewall applications</span></span>
## <a name="properties"></a><span data-ttu-id="9ce79-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ce79-108">Properties</span></span>
|<span data-ttu-id="9ce79-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ce79-109">Property</span></span>|<span data-ttu-id="9ce79-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ce79-110">Type</span></span>|<span data-ttu-id="9ce79-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ce79-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ce79-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="9ce79-112">bundleId</span></span>|<span data-ttu-id="9ce79-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ce79-113">String</span></span>|<span data-ttu-id="9ce79-114">BundleId do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ce79-114">BundleId of the application.</span></span>|
|<span data-ttu-id="9ce79-115">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="9ce79-115">allowsIncomingConnections</span></span>|<span data-ttu-id="9ce79-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="9ce79-116">Boolean</span></span>|<span data-ttu-id="9ce79-117">Ou não são permitidas conexões de entrada.</span><span class="sxs-lookup"><span data-stu-id="9ce79-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ce79-118">Relações</span><span class="sxs-lookup"><span data-stu-id="9ce79-118">Relationships</span></span>
<span data-ttu-id="9ce79-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9ce79-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9ce79-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ce79-120">JSON Representation</span></span>
<span data-ttu-id="9ce79-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ce79-121">Here is a JSON representation of the resource.</span></span>
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





