---
title: Tipo de recurso iosHomeScreenApp
description: Representa um ícone de um aplicativo na tela inicial
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0c3cf96205d6484c61a6f4ec263566ccb9c2efaa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532508"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="1f188-103">Tipo de recurso iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="1f188-103">iosHomeScreenApp resource type</span></span>

<span data-ttu-id="1f188-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f188-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f188-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1f188-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f188-106">Representa um ícone de um aplicativo na tela inicial</span><span class="sxs-lookup"><span data-stu-id="1f188-106">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="1f188-107">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="1f188-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1f188-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1f188-108">Properties</span></span>
|<span data-ttu-id="1f188-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f188-109">Property</span></span>|<span data-ttu-id="1f188-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f188-110">Type</span></span>|<span data-ttu-id="1f188-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f188-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f188-112">displayName</span><span class="sxs-lookup"><span data-stu-id="1f188-112">displayName</span></span>|<span data-ttu-id="1f188-113">String</span><span class="sxs-lookup"><span data-stu-id="1f188-113">String</span></span>|<span data-ttu-id="1f188-114">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="1f188-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="1f188-115">bundleID</span><span class="sxs-lookup"><span data-stu-id="1f188-115">bundleID</span></span>|<span data-ttu-id="1f188-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f188-116">String</span></span>|<span data-ttu-id="1f188-117">BundleID do aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f188-117">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f188-118">Relações</span><span class="sxs-lookup"><span data-stu-id="1f188-118">Relationships</span></span>
<span data-ttu-id="1f188-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f188-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f188-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1f188-120">JSON Representation</span></span>
<span data-ttu-id="1f188-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1f188-121">Here is a JSON representation of the resource.</span></span>
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




