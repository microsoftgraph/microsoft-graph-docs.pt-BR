---
title: tipo de recurso appleAppListItem
description: Representa um aplicativo na lista de aplicativos Apple gerenciados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 831991580d2b3d667011d84179a73957c6eeb200
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703920"
---
# <a name="appleapplistitem-resource-type"></a><span data-ttu-id="abf17-103">tipo de recurso appleAppListItem</span><span class="sxs-lookup"><span data-stu-id="abf17-103">appleAppListItem resource type</span></span>

<span data-ttu-id="abf17-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abf17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="abf17-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="abf17-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abf17-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="abf17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abf17-107">Representa um aplicativo na lista de aplicativos Apple gerenciados</span><span class="sxs-lookup"><span data-stu-id="abf17-107">Represents an app in the list of managed Apple applications</span></span>


<span data-ttu-id="abf17-108">Herda de [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="abf17-108">Inherits from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="abf17-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="abf17-109">Properties</span></span>
|<span data-ttu-id="abf17-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abf17-110">Property</span></span>|<span data-ttu-id="abf17-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="abf17-111">Type</span></span>|<span data-ttu-id="abf17-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="abf17-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abf17-113">nome</span><span class="sxs-lookup"><span data-stu-id="abf17-113">name</span></span>|<span data-ttu-id="abf17-114">String</span><span class="sxs-lookup"><span data-stu-id="abf17-114">String</span></span>|<span data-ttu-id="abf17-115">O nome do aplicativo herdado de [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="abf17-115">The application name Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="abf17-116">publicador</span><span class="sxs-lookup"><span data-stu-id="abf17-116">publisher</span></span>|<span data-ttu-id="abf17-117">String</span><span class="sxs-lookup"><span data-stu-id="abf17-117">String</span></span>|<span data-ttu-id="abf17-118">O fornecedor do aplicativo herdado de [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="abf17-118">The publisher of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="abf17-119">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="abf17-119">appStoreUrl</span></span>|<span data-ttu-id="abf17-120">String</span><span class="sxs-lookup"><span data-stu-id="abf17-120">String</span></span>|<span data-ttu-id="abf17-121">A URL da loja do aplicativo herdado de [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="abf17-121">The Store URL of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="abf17-122">appId</span><span class="sxs-lookup"><span data-stu-id="abf17-122">appId</span></span>|<span data-ttu-id="abf17-123">String</span><span class="sxs-lookup"><span data-stu-id="abf17-123">String</span></span>|<span data-ttu-id="abf17-124">O identificador de aplicativo ou pacote do aplicativo herdado de [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="abf17-124">The application or bundle identifier of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="abf17-125">Relações</span><span class="sxs-lookup"><span data-stu-id="abf17-125">Relationships</span></span>
<span data-ttu-id="abf17-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="abf17-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="abf17-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="abf17-127">JSON Representation</span></span>
<span data-ttu-id="abf17-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="abf17-128">Here is a JSON representation of the resource.</span></span>
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





