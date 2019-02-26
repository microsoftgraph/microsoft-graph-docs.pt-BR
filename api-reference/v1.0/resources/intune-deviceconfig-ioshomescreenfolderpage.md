---
title: Tipo de recurso iosHomeScreenFolderPage
description: Uma pasta com os aplicativos na tela inicial
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f00c67b7a0679d92ef6aac78bc0317e461dcd2f9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255490"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="cfee0-103">Tipo de recurso iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="cfee0-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="cfee0-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cfee0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfee0-105">Uma pasta com os aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="cfee0-105">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="cfee0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cfee0-106">Properties</span></span>
|<span data-ttu-id="cfee0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfee0-107">Property</span></span>|<span data-ttu-id="cfee0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfee0-108">Type</span></span>|<span data-ttu-id="cfee0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfee0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfee0-110">displayName</span><span class="sxs-lookup"><span data-stu-id="cfee0-110">displayName</span></span>|<span data-ttu-id="cfee0-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfee0-111">String</span></span>|<span data-ttu-id="cfee0-112">Nome da página da pasta</span><span class="sxs-lookup"><span data-stu-id="cfee0-112">Name of the folder page</span></span>|
|<span data-ttu-id="cfee0-113">aplicativos</span><span class="sxs-lookup"><span data-stu-id="cfee0-113">apps</span></span>|<span data-ttu-id="cfee0-114">Conjunto [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="cfee0-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="cfee0-115">Uma lista de aplicativos exibidos em uma página dentro de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="cfee0-115">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="cfee0-116">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="cfee0-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfee0-117">Relações</span><span class="sxs-lookup"><span data-stu-id="cfee0-117">Relationships</span></span>
<span data-ttu-id="cfee0-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cfee0-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfee0-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cfee0-119">JSON Representation</span></span>
<span data-ttu-id="cfee0-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cfee0-120">Here is a JSON representation of the resource.</span></span>
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



