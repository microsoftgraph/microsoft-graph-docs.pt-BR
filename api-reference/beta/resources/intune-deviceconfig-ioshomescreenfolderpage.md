---
title: Tipo de recurso iosHomeScreenFolderPage
description: Uma pasta com os aplicativos na tela inicial
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 70cda0dac8c367d279c419e106f71bb0fd171d37
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356974"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="d920c-103">Tipo de recurso iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="d920c-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="d920c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d920c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d920c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d920c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d920c-106">Uma pasta com os aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="d920c-106">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="d920c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d920c-107">Properties</span></span>
|<span data-ttu-id="d920c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d920c-108">Property</span></span>|<span data-ttu-id="d920c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d920c-109">Type</span></span>|<span data-ttu-id="d920c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d920c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d920c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d920c-111">displayName</span></span>|<span data-ttu-id="d920c-112">String</span><span class="sxs-lookup"><span data-stu-id="d920c-112">String</span></span>|<span data-ttu-id="d920c-113">Nome da página da pasta</span><span class="sxs-lookup"><span data-stu-id="d920c-113">Name of the folder page</span></span>|
|<span data-ttu-id="d920c-114">aplicativos</span><span class="sxs-lookup"><span data-stu-id="d920c-114">apps</span></span>|<span data-ttu-id="d920c-115">Conjunto [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="d920c-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="d920c-116">Uma lista de aplicativos exibidos em uma página dentro de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="d920c-116">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="d920c-117">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d920c-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d920c-118">Relações</span><span class="sxs-lookup"><span data-stu-id="d920c-118">Relationships</span></span>
<span data-ttu-id="d920c-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d920c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d920c-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d920c-120">JSON Representation</span></span>
<span data-ttu-id="d920c-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d920c-121">Here is a JSON representation of the resource.</span></span>
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



