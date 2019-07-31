---
title: Tipo de recurso iosHomeScreenPage
description: Uma página que contém aplicativos e pastas na tela inicial
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 79971e74fef96ee77a2ed1106de0a39bf8b64117
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001205"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="214bb-103">Tipo de recurso iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="214bb-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="214bb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="214bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="214bb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="214bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="214bb-106">Uma página que contém aplicativos e pastas na tela inicial</span><span class="sxs-lookup"><span data-stu-id="214bb-106">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="214bb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="214bb-107">Properties</span></span>
|<span data-ttu-id="214bb-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="214bb-108">Property</span></span>|<span data-ttu-id="214bb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="214bb-109">Type</span></span>|<span data-ttu-id="214bb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="214bb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="214bb-111">displayName</span><span class="sxs-lookup"><span data-stu-id="214bb-111">displayName</span></span>|<span data-ttu-id="214bb-112">String</span><span class="sxs-lookup"><span data-stu-id="214bb-112">String</span></span>|<span data-ttu-id="214bb-113">Nome da página</span><span class="sxs-lookup"><span data-stu-id="214bb-113">Name of the page</span></span>|
|<span data-ttu-id="214bb-114">ícones</span><span class="sxs-lookup"><span data-stu-id="214bb-114">icons</span></span>|<span data-ttu-id="214bb-115">Conjunto [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="214bb-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="214bb-116">Uma lista dos aplicativos e pastas exibidos em uma página.</span><span class="sxs-lookup"><span data-stu-id="214bb-116">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="214bb-117">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="214bb-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="214bb-118">Relações</span><span class="sxs-lookup"><span data-stu-id="214bb-118">Relationships</span></span>
<span data-ttu-id="214bb-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="214bb-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="214bb-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="214bb-120">JSON Representation</span></span>
<span data-ttu-id="214bb-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="214bb-121">Here is a JSON representation of the resource.</span></span>
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





