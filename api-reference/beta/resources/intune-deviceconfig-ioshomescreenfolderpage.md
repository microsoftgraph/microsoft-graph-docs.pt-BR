---
title: Tipo de recurso iosHomeScreenFolderPage
description: Uma pasta com os aplicativos na tela inicial
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7d50f83fb180df3d3c94e142854f7cce72955c38
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280428"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="5ed13-103">Tipo de recurso iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="5ed13-103">iosHomeScreenFolderPage resource type</span></span>

<span data-ttu-id="5ed13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ed13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ed13-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5ed13-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ed13-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ed13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ed13-107">Uma pasta com os aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="5ed13-107">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="5ed13-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ed13-108">Properties</span></span>
|<span data-ttu-id="5ed13-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ed13-109">Property</span></span>|<span data-ttu-id="5ed13-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ed13-110">Type</span></span>|<span data-ttu-id="5ed13-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ed13-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ed13-112">displayName</span><span class="sxs-lookup"><span data-stu-id="5ed13-112">displayName</span></span>|<span data-ttu-id="5ed13-113">String</span><span class="sxs-lookup"><span data-stu-id="5ed13-113">String</span></span>|<span data-ttu-id="5ed13-114">Nome da página da pasta</span><span class="sxs-lookup"><span data-stu-id="5ed13-114">Name of the folder page</span></span>|
|<span data-ttu-id="5ed13-115">aplicativos</span><span class="sxs-lookup"><span data-stu-id="5ed13-115">apps</span></span>|<span data-ttu-id="5ed13-116">Conjunto [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed13-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="5ed13-117">Uma lista de aplicativos exibidos em uma página dentro de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="5ed13-117">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="5ed13-118">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="5ed13-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ed13-119">Relações</span><span class="sxs-lookup"><span data-stu-id="5ed13-119">Relationships</span></span>
<span data-ttu-id="5ed13-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5ed13-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ed13-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ed13-121">JSON Representation</span></span>
<span data-ttu-id="5ed13-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ed13-122">Here is a JSON representation of the resource.</span></span>
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




