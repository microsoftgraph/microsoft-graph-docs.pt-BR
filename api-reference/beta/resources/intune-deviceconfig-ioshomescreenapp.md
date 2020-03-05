---
title: Tipo de recurso iosHomeScreenApp
description: Representa um ícone de um aplicativo na tela inicial
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dad65beb6339c96688d61b365ecd1a63f902b1d6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529914"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="2ef68-103">Tipo de recurso iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="2ef68-103">iosHomeScreenApp resource type</span></span>

<span data-ttu-id="2ef68-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2ef68-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ef68-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2ef68-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ef68-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ef68-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ef68-107">Representa um ícone de um aplicativo na tela inicial</span><span class="sxs-lookup"><span data-stu-id="2ef68-107">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="2ef68-108">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="2ef68-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2ef68-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ef68-109">Properties</span></span>
|<span data-ttu-id="2ef68-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ef68-110">Property</span></span>|<span data-ttu-id="2ef68-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ef68-111">Type</span></span>|<span data-ttu-id="2ef68-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ef68-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ef68-113">displayName</span><span class="sxs-lookup"><span data-stu-id="2ef68-113">displayName</span></span>|<span data-ttu-id="2ef68-114">String</span><span class="sxs-lookup"><span data-stu-id="2ef68-114">String</span></span>|<span data-ttu-id="2ef68-115">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="2ef68-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="2ef68-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="2ef68-116">bundleID</span></span>|<span data-ttu-id="2ef68-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ef68-117">String</span></span>|<span data-ttu-id="2ef68-118">BundleID do aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ef68-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ef68-119">Relações</span><span class="sxs-lookup"><span data-stu-id="2ef68-119">Relationships</span></span>
<span data-ttu-id="2ef68-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ef68-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ef68-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ef68-121">JSON Representation</span></span>
<span data-ttu-id="2ef68-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ef68-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```



