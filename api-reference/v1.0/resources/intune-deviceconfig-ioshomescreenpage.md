---
title: Tipo de recurso iosHomeScreenPage
description: Uma página que contém aplicativos e pastas na tela inicial
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d898a1611c05b156ee4b16d042175b6b5c33284d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028172"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="43682-103">Tipo de recurso iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="43682-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="43682-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="43682-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43682-105">Uma página que contém aplicativos e pastas na tela inicial</span><span class="sxs-lookup"><span data-stu-id="43682-105">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="43682-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43682-106">Properties</span></span>
|<span data-ttu-id="43682-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43682-107">Property</span></span>|<span data-ttu-id="43682-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="43682-108">Type</span></span>|<span data-ttu-id="43682-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="43682-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43682-110">displayName</span><span class="sxs-lookup"><span data-stu-id="43682-110">displayName</span></span>|<span data-ttu-id="43682-111">String</span><span class="sxs-lookup"><span data-stu-id="43682-111">String</span></span>|<span data-ttu-id="43682-112">Nome da página</span><span class="sxs-lookup"><span data-stu-id="43682-112">Name of the page</span></span>|
|<span data-ttu-id="43682-113">ícones</span><span class="sxs-lookup"><span data-stu-id="43682-113">icons</span></span>|<span data-ttu-id="43682-114">Conjunto [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="43682-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="43682-115">Uma lista dos aplicativos e pastas exibidos em uma página.</span><span class="sxs-lookup"><span data-stu-id="43682-115">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="43682-116">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="43682-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43682-117">Relações</span><span class="sxs-lookup"><span data-stu-id="43682-117">Relationships</span></span>
<span data-ttu-id="43682-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="43682-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43682-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43682-119">JSON Representation</span></span>
<span data-ttu-id="43682-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="43682-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenPage",
  "displayName": "String",
  "icons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenItem",
      "displayName": "String",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "String",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "String",
              "bundleID": "String"
            }
          ]
        }
      ]
    }
  ]
}
```



