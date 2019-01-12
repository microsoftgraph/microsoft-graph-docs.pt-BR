---
title: Tipo de recurso iosNetworkUsageRule
description: Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 057ddb8027835702cdb487387efafb73cb986c2e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964841"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="2acc5-103">Tipo de recurso iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="2acc5-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="2acc5-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2acc5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2acc5-105">Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.</span><span class="sxs-lookup"><span data-stu-id="2acc5-105">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>
## <a name="properties"></a><span data-ttu-id="2acc5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2acc5-106">Properties</span></span>
|<span data-ttu-id="2acc5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2acc5-107">Property</span></span>|<span data-ttu-id="2acc5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2acc5-108">Type</span></span>|<span data-ttu-id="2acc5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2acc5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2acc5-110">managedApps</span><span class="sxs-lookup"><span data-stu-id="2acc5-110">managedApps</span></span>|<span data-ttu-id="2acc5-111">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="2acc5-111">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="2acc5-112">Informações sobre os aplicativos gerenciados aos quais essa regra se aplicará.</span><span class="sxs-lookup"><span data-stu-id="2acc5-112">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="2acc5-113">Essa coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="2acc5-113">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2acc5-114">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="2acc5-114">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="2acc5-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="2acc5-115">Boolean</span></span>|<span data-ttu-id="2acc5-116">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em roaming.</span><span class="sxs-lookup"><span data-stu-id="2acc5-116">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="2acc5-117">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="2acc5-117">cellularDataBlocked</span></span>|<span data-ttu-id="2acc5-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="2acc5-118">Boolean</span></span>|<span data-ttu-id="2acc5-119">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em nenhum momento.</span><span class="sxs-lookup"><span data-stu-id="2acc5-119">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2acc5-120">Relações</span><span class="sxs-lookup"><span data-stu-id="2acc5-120">Relationships</span></span>
<span data-ttu-id="2acc5-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2acc5-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2acc5-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2acc5-122">JSON Representation</span></span>
<span data-ttu-id="2acc5-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2acc5-123">Here is a JSON representation of the resource.</span></span>
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



