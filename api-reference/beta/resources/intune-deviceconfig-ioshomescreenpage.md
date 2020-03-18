---
title: Tipo de recurso iosHomeScreenPage
description: Uma página que contém aplicativos e pastas na tela inicial
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1d2316f42356bb5b7cfe642bdcdf1712e4bcff61
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790619"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="58243-103">Tipo de recurso iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="58243-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="58243-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="58243-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58243-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58243-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58243-106">Uma página que contém aplicativos e pastas na tela inicial</span><span class="sxs-lookup"><span data-stu-id="58243-106">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="58243-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="58243-107">Properties</span></span>
|<span data-ttu-id="58243-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58243-108">Property</span></span>|<span data-ttu-id="58243-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="58243-109">Type</span></span>|<span data-ttu-id="58243-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="58243-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58243-111">displayName</span><span class="sxs-lookup"><span data-stu-id="58243-111">displayName</span></span>|<span data-ttu-id="58243-112">String</span><span class="sxs-lookup"><span data-stu-id="58243-112">String</span></span>|<span data-ttu-id="58243-113">Nome da página</span><span class="sxs-lookup"><span data-stu-id="58243-113">Name of the page</span></span>|
|<span data-ttu-id="58243-114">ícones</span><span class="sxs-lookup"><span data-stu-id="58243-114">icons</span></span>|<span data-ttu-id="58243-115">Conjunto [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="58243-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="58243-116">Uma lista dos aplicativos e pastas exibidos em uma página.</span><span class="sxs-lookup"><span data-stu-id="58243-116">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="58243-117">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="58243-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58243-118">Relações</span><span class="sxs-lookup"><span data-stu-id="58243-118">Relationships</span></span>
<span data-ttu-id="58243-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58243-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58243-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="58243-120">JSON Representation</span></span>
<span data-ttu-id="58243-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="58243-121">Here is a JSON representation of the resource.</span></span>
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



