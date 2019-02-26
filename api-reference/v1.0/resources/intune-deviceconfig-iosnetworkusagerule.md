---
title: Tipo de recurso iosNetworkUsageRule
description: Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 516e880e4b6230ca165426b849f57609dcc6e6ad
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250100"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="f60a6-103">Tipo de recurso iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="f60a6-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="f60a6-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f60a6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f60a6-105">Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.</span><span class="sxs-lookup"><span data-stu-id="f60a6-105">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="f60a6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f60a6-106">Properties</span></span>
|<span data-ttu-id="f60a6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f60a6-107">Property</span></span>|<span data-ttu-id="f60a6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f60a6-108">Type</span></span>|<span data-ttu-id="f60a6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f60a6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f60a6-110">managedApps</span><span class="sxs-lookup"><span data-stu-id="f60a6-110">managedApps</span></span>|<span data-ttu-id="f60a6-111">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="f60a6-111">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f60a6-112">Informações sobre os aplicativos gerenciados aos quais essa regra se aplicará.</span><span class="sxs-lookup"><span data-stu-id="f60a6-112">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="f60a6-113">Essa coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f60a6-113">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f60a6-114">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="f60a6-114">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="f60a6-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="f60a6-115">Boolean</span></span>|<span data-ttu-id="f60a6-116">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em roaming.</span><span class="sxs-lookup"><span data-stu-id="f60a6-116">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="f60a6-117">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="f60a6-117">cellularDataBlocked</span></span>|<span data-ttu-id="f60a6-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="f60a6-118">Boolean</span></span>|<span data-ttu-id="f60a6-119">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em nenhum momento.</span><span class="sxs-lookup"><span data-stu-id="f60a6-119">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f60a6-120">Relações</span><span class="sxs-lookup"><span data-stu-id="f60a6-120">Relationships</span></span>
<span data-ttu-id="f60a6-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f60a6-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f60a6-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f60a6-122">JSON Representation</span></span>
<span data-ttu-id="f60a6-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f60a6-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNetworkUsageRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNetworkUsageRule",
  "managedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "cellularDataBlockWhenRoaming": true,
  "cellularDataBlocked": true
}
```



