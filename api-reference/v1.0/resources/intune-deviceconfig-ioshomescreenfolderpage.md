---
title: Tipo de recurso iosHomeScreenFolderPage
description: Uma pasta com os aplicativos na tela inicial
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bb2ea3cb1a183af0f437a7a128331084634cca4b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43410634"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="ac379-103">Tipo de recurso iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="ac379-103">iosHomeScreenFolderPage resource type</span></span>

<span data-ttu-id="ac379-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac379-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ac379-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ac379-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac379-106">Uma pasta com os aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="ac379-106">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="ac379-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac379-107">Properties</span></span>
|<span data-ttu-id="ac379-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac379-108">Property</span></span>|<span data-ttu-id="ac379-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac379-109">Type</span></span>|<span data-ttu-id="ac379-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac379-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac379-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ac379-111">displayName</span></span>|<span data-ttu-id="ac379-112">String</span><span class="sxs-lookup"><span data-stu-id="ac379-112">String</span></span>|<span data-ttu-id="ac379-113">Nome da página da pasta</span><span class="sxs-lookup"><span data-stu-id="ac379-113">Name of the folder page</span></span>|
|<span data-ttu-id="ac379-114">aplicativos</span><span class="sxs-lookup"><span data-stu-id="ac379-114">apps</span></span>|<span data-ttu-id="ac379-115">Conjunto [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac379-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="ac379-116">Uma lista de aplicativos exibidos em uma página dentro de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="ac379-116">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="ac379-117">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="ac379-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac379-118">Relações</span><span class="sxs-lookup"><span data-stu-id="ac379-118">Relationships</span></span>
<span data-ttu-id="ac379-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ac379-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac379-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac379-120">JSON Representation</span></span>
<span data-ttu-id="ac379-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ac379-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "displayName": "String",
      "bundleID": "String"
    }
  ]
}
```







