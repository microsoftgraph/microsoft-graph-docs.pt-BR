---
title: tipo de recurso appleAppListItem
description: Representa um aplicativo na lista de aplicativos Apple gerenciados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2583c617ae34d60e83194f5136efcc6c51f06826
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021487"
---
# <a name="appleapplistitem-resource-type"></a><span data-ttu-id="70ef9-103">tipo de recurso appleAppListItem</span><span class="sxs-lookup"><span data-stu-id="70ef9-103">appleAppListItem resource type</span></span>

<span data-ttu-id="70ef9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70ef9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="70ef9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="70ef9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70ef9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="70ef9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70ef9-107">Representa um aplicativo na lista de aplicativos Apple gerenciados</span><span class="sxs-lookup"><span data-stu-id="70ef9-107">Represents an app in the list of managed Apple applications</span></span>


<span data-ttu-id="70ef9-108">Herda de [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="70ef9-108">Inherits from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="70ef9-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70ef9-109">Properties</span></span>
|<span data-ttu-id="70ef9-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70ef9-110">Property</span></span>|<span data-ttu-id="70ef9-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="70ef9-111">Type</span></span>|<span data-ttu-id="70ef9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="70ef9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70ef9-113">nome</span><span class="sxs-lookup"><span data-stu-id="70ef9-113">name</span></span>|<span data-ttu-id="70ef9-114">String</span><span class="sxs-lookup"><span data-stu-id="70ef9-114">String</span></span>|<span data-ttu-id="70ef9-115">O nome do aplicativo herdado de [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="70ef9-115">The application name Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="70ef9-116">publicador</span><span class="sxs-lookup"><span data-stu-id="70ef9-116">publisher</span></span>|<span data-ttu-id="70ef9-117">String</span><span class="sxs-lookup"><span data-stu-id="70ef9-117">String</span></span>|<span data-ttu-id="70ef9-118">O fornecedor do aplicativo herdado de [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="70ef9-118">The publisher of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="70ef9-119">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="70ef9-119">appStoreUrl</span></span>|<span data-ttu-id="70ef9-120">String</span><span class="sxs-lookup"><span data-stu-id="70ef9-120">String</span></span>|<span data-ttu-id="70ef9-121">A URL da loja do aplicativo herdado de [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="70ef9-121">The Store URL of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="70ef9-122">appId</span><span class="sxs-lookup"><span data-stu-id="70ef9-122">appId</span></span>|<span data-ttu-id="70ef9-123">String</span><span class="sxs-lookup"><span data-stu-id="70ef9-123">String</span></span>|<span data-ttu-id="70ef9-124">O identificador de aplicativo ou pacote do aplicativo herdado de [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="70ef9-124">The application or bundle identifier of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="70ef9-125">Relações</span><span class="sxs-lookup"><span data-stu-id="70ef9-125">Relationships</span></span>
<span data-ttu-id="70ef9-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="70ef9-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="70ef9-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70ef9-127">JSON Representation</span></span>
<span data-ttu-id="70ef9-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="70ef9-128">Here is a JSON representation of the resource.</span></span>
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






