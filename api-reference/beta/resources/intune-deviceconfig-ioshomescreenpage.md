---
title: Tipo de recurso iosHomeScreenPage
description: Uma página que contém aplicativos e pastas na tela inicial
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7b0190b31f58ee5532fd1d0f3e3459e552bb00b5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455138"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="18486-103">Tipo de recurso iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="18486-103">iosHomeScreenPage resource type</span></span>

<span data-ttu-id="18486-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18486-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18486-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="18486-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18486-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="18486-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18486-107">Uma página que contém aplicativos e pastas na tela inicial</span><span class="sxs-lookup"><span data-stu-id="18486-107">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="18486-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18486-108">Properties</span></span>
|<span data-ttu-id="18486-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18486-109">Property</span></span>|<span data-ttu-id="18486-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="18486-110">Type</span></span>|<span data-ttu-id="18486-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="18486-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18486-112">displayName</span><span class="sxs-lookup"><span data-stu-id="18486-112">displayName</span></span>|<span data-ttu-id="18486-113">String</span><span class="sxs-lookup"><span data-stu-id="18486-113">String</span></span>|<span data-ttu-id="18486-114">Nome da página</span><span class="sxs-lookup"><span data-stu-id="18486-114">Name of the page</span></span>|
|<span data-ttu-id="18486-115">ícones</span><span class="sxs-lookup"><span data-stu-id="18486-115">icons</span></span>|<span data-ttu-id="18486-116">Conjunto [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="18486-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="18486-117">Uma lista dos aplicativos e pastas exibidos em uma página.</span><span class="sxs-lookup"><span data-stu-id="18486-117">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="18486-118">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="18486-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18486-119">Relações</span><span class="sxs-lookup"><span data-stu-id="18486-119">Relationships</span></span>
<span data-ttu-id="18486-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18486-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18486-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18486-121">JSON Representation</span></span>
<span data-ttu-id="18486-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18486-122">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
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



