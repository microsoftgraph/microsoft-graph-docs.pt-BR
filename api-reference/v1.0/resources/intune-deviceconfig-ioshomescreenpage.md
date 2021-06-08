---
title: Tipo de recurso iosHomeScreenPage
description: Uma página que contém aplicativos, pastas e clipes da Web na Tela Inicial.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9bc9880f63bc27ce4cdab44b128d6d373e348fb1
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760047"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="1b654-103">Tipo de recurso iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="1b654-103">iosHomeScreenPage resource type</span></span>

<span data-ttu-id="1b654-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b654-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b654-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1b654-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b654-106">Uma página que contém aplicativos, pastas e clipes da Web na Tela Inicial.</span><span class="sxs-lookup"><span data-stu-id="1b654-106">A page containing apps, folders, and web clips on the Home Screen.</span></span>

## <a name="properties"></a><span data-ttu-id="1b654-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b654-107">Properties</span></span>
|<span data-ttu-id="1b654-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b654-108">Property</span></span>|<span data-ttu-id="1b654-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b654-109">Type</span></span>|<span data-ttu-id="1b654-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b654-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b654-111">displayName</span><span class="sxs-lookup"><span data-stu-id="1b654-111">displayName</span></span>|<span data-ttu-id="1b654-112">String</span><span class="sxs-lookup"><span data-stu-id="1b654-112">String</span></span>|<span data-ttu-id="1b654-113">Nome da página</span><span class="sxs-lookup"><span data-stu-id="1b654-113">Name of the page</span></span>|
|<span data-ttu-id="1b654-114">ícones</span><span class="sxs-lookup"><span data-stu-id="1b654-114">icons</span></span>|<span data-ttu-id="1b654-115">Conjunto [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="1b654-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="1b654-116">Uma lista de aplicativos, pastas e clipes da Web a ser exibida em uma página.</span><span class="sxs-lookup"><span data-stu-id="1b654-116">A list of apps, folders, and web clips to appear on a page.</span></span> <span data-ttu-id="1b654-117">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="1b654-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b654-118">Relações</span><span class="sxs-lookup"><span data-stu-id="1b654-118">Relationships</span></span>
<span data-ttu-id="1b654-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1b654-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b654-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b654-120">JSON Representation</span></span>
<span data-ttu-id="1b654-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1b654-121">Here is a JSON representation of the resource.</span></span>
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




