---
title: tipo de recurso appleAppListItem
description: Representa um aplicativo na lista de aplicativos Apple gerenciados
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6f4804f3834a63a3c446c09d383c2244def97398
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470122"
---
# <a name="appleapplistitem-resource-type"></a><span data-ttu-id="36b2b-103">tipo de recurso appleAppListItem</span><span class="sxs-lookup"><span data-stu-id="36b2b-103">appleAppListItem resource type</span></span>

<span data-ttu-id="36b2b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36b2b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36b2b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="36b2b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36b2b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="36b2b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36b2b-107">Representa um aplicativo na lista de aplicativos Apple gerenciados</span><span class="sxs-lookup"><span data-stu-id="36b2b-107">Represents an app in the list of managed Apple applications</span></span>


<span data-ttu-id="36b2b-108">Herda de [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="36b2b-108">Inherits from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="36b2b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36b2b-109">Properties</span></span>
|<span data-ttu-id="36b2b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36b2b-110">Property</span></span>|<span data-ttu-id="36b2b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="36b2b-111">Type</span></span>|<span data-ttu-id="36b2b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="36b2b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36b2b-113">nome</span><span class="sxs-lookup"><span data-stu-id="36b2b-113">name</span></span>|<span data-ttu-id="36b2b-114">String</span><span class="sxs-lookup"><span data-stu-id="36b2b-114">String</span></span>|<span data-ttu-id="36b2b-115">O nome do aplicativo herdado de [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="36b2b-115">The application name Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="36b2b-116">publicador</span><span class="sxs-lookup"><span data-stu-id="36b2b-116">publisher</span></span>|<span data-ttu-id="36b2b-117">String</span><span class="sxs-lookup"><span data-stu-id="36b2b-117">String</span></span>|<span data-ttu-id="36b2b-118">O fornecedor do aplicativo herdado de [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="36b2b-118">The publisher of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="36b2b-119">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="36b2b-119">appStoreUrl</span></span>|<span data-ttu-id="36b2b-120">String</span><span class="sxs-lookup"><span data-stu-id="36b2b-120">String</span></span>|<span data-ttu-id="36b2b-121">A URL da loja do aplicativo herdado de [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="36b2b-121">The Store URL of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="36b2b-122">appId</span><span class="sxs-lookup"><span data-stu-id="36b2b-122">appId</span></span>|<span data-ttu-id="36b2b-123">String</span><span class="sxs-lookup"><span data-stu-id="36b2b-123">String</span></span>|<span data-ttu-id="36b2b-124">O identificador do pacote do aplicativo herdado de [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="36b2b-124">The bundle identifier of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="36b2b-125">Relações</span><span class="sxs-lookup"><span data-stu-id="36b2b-125">Relationships</span></span>
<span data-ttu-id="36b2b-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="36b2b-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="36b2b-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36b2b-127">JSON Representation</span></span>
<span data-ttu-id="36b2b-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="36b2b-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleAppListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleAppListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```



