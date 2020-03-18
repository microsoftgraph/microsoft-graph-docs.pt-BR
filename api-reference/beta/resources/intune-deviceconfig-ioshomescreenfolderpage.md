---
title: Tipo de recurso iosHomeScreenFolderPage
description: Uma pasta com os aplicativos na tela inicial
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 93fca952cfda7bf1e49c17a3fe71b3a62384d0e6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791573"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="e07e1-103">Tipo de recurso iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="e07e1-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="e07e1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e07e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e07e1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e07e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e07e1-106">Uma pasta com os aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="e07e1-106">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="e07e1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e07e1-107">Properties</span></span>
|<span data-ttu-id="e07e1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e07e1-108">Property</span></span>|<span data-ttu-id="e07e1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e07e1-109">Type</span></span>|<span data-ttu-id="e07e1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e07e1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e07e1-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e07e1-111">displayName</span></span>|<span data-ttu-id="e07e1-112">String</span><span class="sxs-lookup"><span data-stu-id="e07e1-112">String</span></span>|<span data-ttu-id="e07e1-113">Nome da página da pasta</span><span class="sxs-lookup"><span data-stu-id="e07e1-113">Name of the folder page</span></span>|
|<span data-ttu-id="e07e1-114">aplicativos</span><span class="sxs-lookup"><span data-stu-id="e07e1-114">apps</span></span>|<span data-ttu-id="e07e1-115">Conjunto [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="e07e1-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="e07e1-116">Uma lista de aplicativos exibidos em uma página dentro de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="e07e1-116">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="e07e1-117">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="e07e1-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e07e1-118">Relações</span><span class="sxs-lookup"><span data-stu-id="e07e1-118">Relationships</span></span>
<span data-ttu-id="e07e1-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e07e1-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e07e1-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e07e1-120">JSON Representation</span></span>
<span data-ttu-id="e07e1-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e07e1-121">Here is a JSON representation of the resource.</span></span>
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



