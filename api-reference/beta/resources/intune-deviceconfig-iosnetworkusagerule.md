---
title: Tipo de recurso iosNetworkUsageRule
description: Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.
localization_priority: Normal
ms.openlocfilehash: 6cf2f0cd88c25a625b12b3adcaac6ccc366ea0e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860995"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="5154b-103">Tipo de recurso iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="5154b-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="5154b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5154b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5154b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5154b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5154b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5154b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5154b-107">Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.</span><span class="sxs-lookup"><span data-stu-id="5154b-107">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>
## <a name="properties"></a><span data-ttu-id="5154b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5154b-108">Properties</span></span>
|<span data-ttu-id="5154b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5154b-109">Property</span></span>|<span data-ttu-id="5154b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5154b-110">Type</span></span>|<span data-ttu-id="5154b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5154b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5154b-112">managedApps</span><span class="sxs-lookup"><span data-stu-id="5154b-112">managedApps</span></span>|<span data-ttu-id="5154b-113">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="5154b-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="5154b-114">Informações sobre os aplicativos gerenciados aos quais essa regra se aplicará.</span><span class="sxs-lookup"><span data-stu-id="5154b-114">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="5154b-115">Essa coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="5154b-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5154b-116">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="5154b-116">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="5154b-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="5154b-117">Boolean</span></span>|<span data-ttu-id="5154b-118">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em roaming.</span><span class="sxs-lookup"><span data-stu-id="5154b-118">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="5154b-119">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="5154b-119">cellularDataBlocked</span></span>|<span data-ttu-id="5154b-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="5154b-120">Boolean</span></span>|<span data-ttu-id="5154b-121">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em nenhum momento.</span><span class="sxs-lookup"><span data-stu-id="5154b-121">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5154b-122">Relações</span><span class="sxs-lookup"><span data-stu-id="5154b-122">Relationships</span></span>
<span data-ttu-id="5154b-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5154b-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5154b-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5154b-124">JSON Representation</span></span>
<span data-ttu-id="5154b-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5154b-125">Here is a JSON representation of the resource.</span></span>
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





