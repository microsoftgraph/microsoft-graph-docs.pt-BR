---
title: Tipo de recurso iosNetworkUsageRule
description: Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 52da789c1a01bc74868157b4a81e459b1059856e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004215"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="5ac76-103">Tipo de recurso iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="5ac76-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="5ac76-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5ac76-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ac76-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ac76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ac76-106">Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.</span><span class="sxs-lookup"><span data-stu-id="5ac76-106">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="5ac76-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ac76-107">Properties</span></span>
|<span data-ttu-id="5ac76-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ac76-108">Property</span></span>|<span data-ttu-id="5ac76-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ac76-109">Type</span></span>|<span data-ttu-id="5ac76-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ac76-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ac76-111">managedApps</span><span class="sxs-lookup"><span data-stu-id="5ac76-111">managedApps</span></span>|<span data-ttu-id="5ac76-112">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="5ac76-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="5ac76-113">Informações sobre os aplicativos gerenciados aos quais essa regra se aplicará.</span><span class="sxs-lookup"><span data-stu-id="5ac76-113">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="5ac76-114">Essa coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="5ac76-114">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5ac76-115">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="5ac76-115">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="5ac76-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="5ac76-116">Boolean</span></span>|<span data-ttu-id="5ac76-117">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em roaming.</span><span class="sxs-lookup"><span data-stu-id="5ac76-117">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="5ac76-118">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="5ac76-118">cellularDataBlocked</span></span>|<span data-ttu-id="5ac76-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="5ac76-119">Boolean</span></span>|<span data-ttu-id="5ac76-120">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em nenhum momento.</span><span class="sxs-lookup"><span data-stu-id="5ac76-120">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ac76-121">Relações</span><span class="sxs-lookup"><span data-stu-id="5ac76-121">Relationships</span></span>
<span data-ttu-id="5ac76-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5ac76-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ac76-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ac76-123">JSON Representation</span></span>
<span data-ttu-id="5ac76-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ac76-124">Here is a JSON representation of the resource.</span></span>
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





