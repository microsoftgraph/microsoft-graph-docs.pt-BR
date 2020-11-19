---
title: Tipo de recurso iosNetworkUsageRule
description: Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67e5b5c1df4fa4f10301bbaa7177c5d3ab8ed70e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280273"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="5a5b3-103">Tipo de recurso iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="5a5b3-103">iosNetworkUsageRule resource type</span></span>

<span data-ttu-id="5a5b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a5b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5a5b3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5a5b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a5b3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5a5b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a5b3-107">Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.</span><span class="sxs-lookup"><span data-stu-id="5a5b3-107">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="5a5b3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a5b3-108">Properties</span></span>
|<span data-ttu-id="5a5b3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a5b3-109">Property</span></span>|<span data-ttu-id="5a5b3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a5b3-110">Type</span></span>|<span data-ttu-id="5a5b3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a5b3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a5b3-112">managedApps</span><span class="sxs-lookup"><span data-stu-id="5a5b3-112">managedApps</span></span>|<span data-ttu-id="5a5b3-113">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="5a5b3-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="5a5b3-114">Informações sobre os aplicativos gerenciados aos quais essa regra se aplicará.</span><span class="sxs-lookup"><span data-stu-id="5a5b3-114">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="5a5b3-115">Essa coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="5a5b3-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5a5b3-116">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="5a5b3-116">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="5a5b3-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="5a5b3-117">Boolean</span></span>|<span data-ttu-id="5a5b3-118">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em roaming.</span><span class="sxs-lookup"><span data-stu-id="5a5b3-118">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="5a5b3-119">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="5a5b3-119">cellularDataBlocked</span></span>|<span data-ttu-id="5a5b3-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="5a5b3-120">Boolean</span></span>|<span data-ttu-id="5a5b3-121">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em nenhum momento.</span><span class="sxs-lookup"><span data-stu-id="5a5b3-121">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a5b3-122">Relações</span><span class="sxs-lookup"><span data-stu-id="5a5b3-122">Relationships</span></span>
<span data-ttu-id="5a5b3-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5a5b3-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a5b3-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a5b3-124">JSON Representation</span></span>
<span data-ttu-id="5a5b3-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a5b3-125">Here is a JSON representation of the resource.</span></span>
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




