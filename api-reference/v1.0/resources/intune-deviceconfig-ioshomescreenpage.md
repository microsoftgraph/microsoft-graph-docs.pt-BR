---
title: Tipo de recurso iosHomeScreenPage
description: Uma página que contém aplicativos e pastas na tela inicial
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: abe09741cd3ed4f25f417cbb99cd144d6105acba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532487"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="df20b-103">Tipo de recurso iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="df20b-103">iosHomeScreenPage resource type</span></span>

<span data-ttu-id="df20b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df20b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df20b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="df20b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df20b-106">Uma página que contém aplicativos e pastas na tela inicial</span><span class="sxs-lookup"><span data-stu-id="df20b-106">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="df20b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df20b-107">Properties</span></span>
|<span data-ttu-id="df20b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df20b-108">Property</span></span>|<span data-ttu-id="df20b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="df20b-109">Type</span></span>|<span data-ttu-id="df20b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="df20b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df20b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="df20b-111">displayName</span></span>|<span data-ttu-id="df20b-112">String</span><span class="sxs-lookup"><span data-stu-id="df20b-112">String</span></span>|<span data-ttu-id="df20b-113">Nome da página</span><span class="sxs-lookup"><span data-stu-id="df20b-113">Name of the page</span></span>|
|<span data-ttu-id="df20b-114">ícones</span><span class="sxs-lookup"><span data-stu-id="df20b-114">icons</span></span>|<span data-ttu-id="df20b-115">Conjunto [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="df20b-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="df20b-116">Uma lista dos aplicativos e pastas exibidos em uma página.</span><span class="sxs-lookup"><span data-stu-id="df20b-116">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="df20b-117">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="df20b-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df20b-118">Relações</span><span class="sxs-lookup"><span data-stu-id="df20b-118">Relationships</span></span>
<span data-ttu-id="df20b-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="df20b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df20b-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df20b-120">JSON Representation</span></span>
<span data-ttu-id="df20b-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df20b-121">Here is a JSON representation of the resource.</span></span>
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




