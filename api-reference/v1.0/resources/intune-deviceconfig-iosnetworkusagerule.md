---
title: Tipo de recurso iosNetworkUsageRule
description: Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: abe641a0a714c8e2d9e171ccb874905b3a6321b6
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359058"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="d9636-103">Tipo de recurso iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="d9636-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="d9636-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9636-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9636-105">Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.</span><span class="sxs-lookup"><span data-stu-id="d9636-105">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="d9636-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9636-106">Properties</span></span>
|<span data-ttu-id="d9636-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9636-107">Property</span></span>|<span data-ttu-id="d9636-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9636-108">Type</span></span>|<span data-ttu-id="d9636-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9636-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9636-110">managedApps</span><span class="sxs-lookup"><span data-stu-id="d9636-110">managedApps</span></span>|<span data-ttu-id="d9636-111">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d9636-111">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d9636-112">Informações sobre os aplicativos gerenciados aos quais essa regra se aplicará.</span><span class="sxs-lookup"><span data-stu-id="d9636-112">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="d9636-113">Essa coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d9636-113">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="d9636-114">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="d9636-114">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="d9636-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9636-115">Boolean</span></span>|<span data-ttu-id="d9636-116">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em roaming.</span><span class="sxs-lookup"><span data-stu-id="d9636-116">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="d9636-117">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="d9636-117">cellularDataBlocked</span></span>|<span data-ttu-id="d9636-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9636-118">Boolean</span></span>|<span data-ttu-id="d9636-119">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em nenhum momento.</span><span class="sxs-lookup"><span data-stu-id="d9636-119">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9636-120">Relações</span><span class="sxs-lookup"><span data-stu-id="d9636-120">Relationships</span></span>
<span data-ttu-id="d9636-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d9636-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9636-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9636-122">JSON Representation</span></span>
<span data-ttu-id="d9636-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d9636-123">Here is a JSON representation of the resource.</span></span>
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




