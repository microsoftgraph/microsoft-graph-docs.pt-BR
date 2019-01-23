---
title: Tipo de recurso iosNetworkUsageRule
description: Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0a287fcf8be771037a39efd821f5468acf518371
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398321"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="6e9a0-103">Tipo de recurso iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="6e9a0-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="6e9a0-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="6e9a0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6e9a0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6e9a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e9a0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="6e9a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e9a0-107">Regras de Uso da Rede permitem que empresas especifiquem como aplicativos gerenciados usam redes, como redes de dados celulares.</span><span class="sxs-lookup"><span data-stu-id="6e9a0-107">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="6e9a0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e9a0-108">Properties</span></span>
|<span data-ttu-id="6e9a0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e9a0-109">Property</span></span>|<span data-ttu-id="6e9a0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e9a0-110">Type</span></span>|<span data-ttu-id="6e9a0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e9a0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e9a0-112">managedApps</span><span class="sxs-lookup"><span data-stu-id="6e9a0-112">managedApps</span></span>|<span data-ttu-id="6e9a0-113">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6e9a0-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6e9a0-114">Informações sobre os aplicativos gerenciados aos quais essa regra se aplicará.</span><span class="sxs-lookup"><span data-stu-id="6e9a0-114">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="6e9a0-115">Essa coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="6e9a0-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6e9a0-116">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="6e9a0-116">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="6e9a0-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="6e9a0-117">Boolean</span></span>|<span data-ttu-id="6e9a0-118">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em roaming.</span><span class="sxs-lookup"><span data-stu-id="6e9a0-118">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="6e9a0-119">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="6e9a0-119">cellularDataBlocked</span></span>|<span data-ttu-id="6e9a0-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="6e9a0-120">Boolean</span></span>|<span data-ttu-id="6e9a0-121">Se definido como true, os aplicativos gerenciados correspondentes não poderão usar dados celulares em nenhum momento.</span><span class="sxs-lookup"><span data-stu-id="6e9a0-121">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e9a0-122">Relações</span><span class="sxs-lookup"><span data-stu-id="6e9a0-122">Relationships</span></span>
<span data-ttu-id="6e9a0-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e9a0-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e9a0-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e9a0-124">JSON Representation</span></span>
<span data-ttu-id="6e9a0-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e9a0-125">Here is a JSON representation of the resource.</span></span>
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




