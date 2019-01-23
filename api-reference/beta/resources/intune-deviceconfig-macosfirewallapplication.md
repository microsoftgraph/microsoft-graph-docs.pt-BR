---
title: tipo de recurso de macOSFirewallApplication
description: Representa um aplicativo na lista de aplicativos de firewall macOS
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fe3bbd83c3101420ec011fda85304fabce06daf0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404208"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="3a14f-103">tipo de recurso de macOSFirewallApplication</span><span class="sxs-lookup"><span data-stu-id="3a14f-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="3a14f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="3a14f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3a14f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3a14f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a14f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="3a14f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a14f-107">Representa um aplicativo na lista de aplicativos de firewall macOS</span><span class="sxs-lookup"><span data-stu-id="3a14f-107">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="3a14f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a14f-108">Properties</span></span>
|<span data-ttu-id="3a14f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a14f-109">Property</span></span>|<span data-ttu-id="3a14f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a14f-110">Type</span></span>|<span data-ttu-id="3a14f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a14f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a14f-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="3a14f-112">bundleId</span></span>|<span data-ttu-id="3a14f-113">String</span><span class="sxs-lookup"><span data-stu-id="3a14f-113">String</span></span>|<span data-ttu-id="3a14f-114">BundleId do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3a14f-114">BundleId of the application.</span></span>|
|<span data-ttu-id="3a14f-115">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="3a14f-115">allowsIncomingConnections</span></span>|<span data-ttu-id="3a14f-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a14f-116">Boolean</span></span>|<span data-ttu-id="3a14f-117">Ou não são permitidas conexões de entrada.</span><span class="sxs-lookup"><span data-stu-id="3a14f-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a14f-118">Relações</span><span class="sxs-lookup"><span data-stu-id="3a14f-118">Relationships</span></span>
<span data-ttu-id="3a14f-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3a14f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a14f-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a14f-120">JSON Representation</span></span>
<span data-ttu-id="3a14f-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a14f-121">Here is a JSON representation of the resource.</span></span>
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




