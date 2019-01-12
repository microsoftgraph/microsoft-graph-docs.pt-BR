---
title: Tipo de recurso iosNetworkUsageRule
description: Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 7476f49c6049eb18e56fa57310aa75707f566bd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912019"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="73cca-103">Tipo de recurso iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="73cca-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="73cca-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="73cca-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73cca-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="73cca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73cca-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="73cca-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73cca-107">Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.</span><span class="sxs-lookup"><span data-stu-id="73cca-107">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>
## <a name="properties"></a><span data-ttu-id="73cca-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73cca-108">Properties</span></span>
|<span data-ttu-id="73cca-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73cca-109">Property</span></span>|<span data-ttu-id="73cca-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="73cca-110">Type</span></span>|<span data-ttu-id="73cca-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="73cca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73cca-112">managedApps</span><span class="sxs-lookup"><span data-stu-id="73cca-112">managedApps</span></span>|<span data-ttu-id="73cca-113">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="73cca-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="73cca-114">Informações sobre os aplicativos gerenciados aos quais essa regra se aplicará.</span><span class="sxs-lookup"><span data-stu-id="73cca-114">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="73cca-115">Essa coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="73cca-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="73cca-116">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="73cca-116">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="73cca-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="73cca-117">Boolean</span></span>|<span data-ttu-id="73cca-118">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em roaming.</span><span class="sxs-lookup"><span data-stu-id="73cca-118">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="73cca-119">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="73cca-119">cellularDataBlocked</span></span>|<span data-ttu-id="73cca-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="73cca-120">Boolean</span></span>|<span data-ttu-id="73cca-121">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em nenhum momento.</span><span class="sxs-lookup"><span data-stu-id="73cca-121">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73cca-122">Relações</span><span class="sxs-lookup"><span data-stu-id="73cca-122">Relationships</span></span>
<span data-ttu-id="73cca-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="73cca-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="73cca-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73cca-124">JSON Representation</span></span>
<span data-ttu-id="73cca-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="73cca-125">Here is a JSON representation of the resource.</span></span>
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





