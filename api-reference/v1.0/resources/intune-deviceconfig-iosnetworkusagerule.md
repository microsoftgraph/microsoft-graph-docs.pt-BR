---
title: Tipo de recurso iosNetworkUsageRule
description: Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b0698ada0fbda3c30e0c2d836c0e949b742b1c99
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091688"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="ed8d2-103">Tipo de recurso iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="ed8d2-103">iosNetworkUsageRule resource type</span></span>

<span data-ttu-id="ed8d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed8d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed8d2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed8d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed8d2-106">Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.</span><span class="sxs-lookup"><span data-stu-id="ed8d2-106">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="ed8d2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed8d2-107">Properties</span></span>
|<span data-ttu-id="ed8d2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed8d2-108">Property</span></span>|<span data-ttu-id="ed8d2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed8d2-109">Type</span></span>|<span data-ttu-id="ed8d2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed8d2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed8d2-111">managedApps</span><span class="sxs-lookup"><span data-stu-id="ed8d2-111">managedApps</span></span>|<span data-ttu-id="ed8d2-112">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ed8d2-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ed8d2-113">Informações sobre os aplicativos gerenciados aos quais essa regra se aplicará.</span><span class="sxs-lookup"><span data-stu-id="ed8d2-113">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="ed8d2-114">Essa coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="ed8d2-114">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ed8d2-115">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="ed8d2-115">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="ed8d2-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="ed8d2-116">Boolean</span></span>|<span data-ttu-id="ed8d2-117">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em roaming.</span><span class="sxs-lookup"><span data-stu-id="ed8d2-117">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="ed8d2-118">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="ed8d2-118">cellularDataBlocked</span></span>|<span data-ttu-id="ed8d2-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="ed8d2-119">Boolean</span></span>|<span data-ttu-id="ed8d2-120">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em nenhum momento.</span><span class="sxs-lookup"><span data-stu-id="ed8d2-120">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed8d2-121">Relações</span><span class="sxs-lookup"><span data-stu-id="ed8d2-121">Relationships</span></span>
<span data-ttu-id="ed8d2-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed8d2-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed8d2-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed8d2-123">JSON Representation</span></span>
<span data-ttu-id="ed8d2-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed8d2-124">Here is a JSON representation of the resource.</span></span>
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









