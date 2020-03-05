---
title: Tipo de recurso iosHomeScreenPage
description: Uma página que contém aplicativos e pastas na tela inicial
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 00d28920633f4f8aa205c77a99d70fb26639148d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529897"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="4bd99-103">Tipo de recurso iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="4bd99-103">iosHomeScreenPage resource type</span></span>

<span data-ttu-id="4bd99-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4bd99-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4bd99-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4bd99-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4bd99-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4bd99-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bd99-107">Uma página que contém aplicativos e pastas na tela inicial</span><span class="sxs-lookup"><span data-stu-id="4bd99-107">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="4bd99-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4bd99-108">Properties</span></span>
|<span data-ttu-id="4bd99-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4bd99-109">Property</span></span>|<span data-ttu-id="4bd99-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bd99-110">Type</span></span>|<span data-ttu-id="4bd99-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bd99-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bd99-112">displayName</span><span class="sxs-lookup"><span data-stu-id="4bd99-112">displayName</span></span>|<span data-ttu-id="4bd99-113">String</span><span class="sxs-lookup"><span data-stu-id="4bd99-113">String</span></span>|<span data-ttu-id="4bd99-114">Nome da página</span><span class="sxs-lookup"><span data-stu-id="4bd99-114">Name of the page</span></span>|
|<span data-ttu-id="4bd99-115">ícones</span><span class="sxs-lookup"><span data-stu-id="4bd99-115">icons</span></span>|<span data-ttu-id="4bd99-116">Conjunto [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="4bd99-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="4bd99-117">Uma lista dos aplicativos e pastas exibidos em uma página.</span><span class="sxs-lookup"><span data-stu-id="4bd99-117">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="4bd99-118">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="4bd99-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4bd99-119">Relações</span><span class="sxs-lookup"><span data-stu-id="4bd99-119">Relationships</span></span>
<span data-ttu-id="4bd99-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4bd99-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4bd99-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4bd99-121">JSON Representation</span></span>
<span data-ttu-id="4bd99-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4bd99-122">Here is a JSON representation of the resource.</span></span>
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



