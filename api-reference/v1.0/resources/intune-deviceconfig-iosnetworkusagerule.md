---
title: Tipo de recurso iosNetworkUsageRule
description: Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ab6f070457db8499caa6f9bb842078086e33c02a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43410557"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="c2915-103">Tipo de recurso iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="c2915-103">iosNetworkUsageRule resource type</span></span>

<span data-ttu-id="c2915-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2915-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2915-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c2915-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2915-106">Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.</span><span class="sxs-lookup"><span data-stu-id="c2915-106">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="c2915-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c2915-107">Properties</span></span>
|<span data-ttu-id="c2915-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2915-108">Property</span></span>|<span data-ttu-id="c2915-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2915-109">Type</span></span>|<span data-ttu-id="c2915-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2915-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2915-111">managedApps</span><span class="sxs-lookup"><span data-stu-id="c2915-111">managedApps</span></span>|<span data-ttu-id="c2915-112">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c2915-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c2915-113">Informações sobre os aplicativos gerenciados aos quais essa regra se aplicará.</span><span class="sxs-lookup"><span data-stu-id="c2915-113">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="c2915-114">Essa coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c2915-114">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c2915-115">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="c2915-115">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="c2915-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="c2915-116">Boolean</span></span>|<span data-ttu-id="c2915-117">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em roaming.</span><span class="sxs-lookup"><span data-stu-id="c2915-117">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="c2915-118">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="c2915-118">cellularDataBlocked</span></span>|<span data-ttu-id="c2915-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="c2915-119">Boolean</span></span>|<span data-ttu-id="c2915-120">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em nenhum momento.</span><span class="sxs-lookup"><span data-stu-id="c2915-120">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2915-121">Relações</span><span class="sxs-lookup"><span data-stu-id="c2915-121">Relationships</span></span>
<span data-ttu-id="c2915-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c2915-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2915-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c2915-123">JSON Representation</span></span>
<span data-ttu-id="c2915-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c2915-124">Here is a JSON representation of the resource.</span></span>
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







