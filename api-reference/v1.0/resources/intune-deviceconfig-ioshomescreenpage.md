---
title: Tipo de recurso iosHomeScreenPage
description: Uma página que contém aplicativos e pastas na tela inicial
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fea1480b8b84a68d67a1bad499fa6c5b53841d35
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43410588"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="ed565-103">Tipo de recurso iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="ed565-103">iosHomeScreenPage resource type</span></span>

<span data-ttu-id="ed565-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed565-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed565-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed565-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed565-106">Uma página que contém aplicativos e pastas na tela inicial</span><span class="sxs-lookup"><span data-stu-id="ed565-106">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="ed565-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed565-107">Properties</span></span>
|<span data-ttu-id="ed565-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed565-108">Property</span></span>|<span data-ttu-id="ed565-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed565-109">Type</span></span>|<span data-ttu-id="ed565-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed565-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed565-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ed565-111">displayName</span></span>|<span data-ttu-id="ed565-112">String</span><span class="sxs-lookup"><span data-stu-id="ed565-112">String</span></span>|<span data-ttu-id="ed565-113">Nome da página</span><span class="sxs-lookup"><span data-stu-id="ed565-113">Name of the page</span></span>|
|<span data-ttu-id="ed565-114">ícones</span><span class="sxs-lookup"><span data-stu-id="ed565-114">icons</span></span>|<span data-ttu-id="ed565-115">Conjunto [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="ed565-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="ed565-116">Uma lista dos aplicativos e pastas exibidos em uma página.</span><span class="sxs-lookup"><span data-stu-id="ed565-116">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="ed565-117">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="ed565-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed565-118">Relações</span><span class="sxs-lookup"><span data-stu-id="ed565-118">Relationships</span></span>
<span data-ttu-id="ed565-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed565-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed565-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed565-120">JSON Representation</span></span>
<span data-ttu-id="ed565-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed565-121">Here is a JSON representation of the resource.</span></span>
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







