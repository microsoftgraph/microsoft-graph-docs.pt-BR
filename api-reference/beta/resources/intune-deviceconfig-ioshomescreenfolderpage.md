---
title: Tipo de recurso iosHomeScreenFolderPage
description: Uma pasta com os aplicativos na tela inicial
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f18061e8bc8c974eab443d389b94be80134924f9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993907"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="6bfd9-103">Tipo de recurso iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="6bfd9-103">iosHomeScreenFolderPage resource type</span></span>

<span data-ttu-id="6bfd9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bfd9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6bfd9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6bfd9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bfd9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6bfd9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bfd9-107">Uma pasta com os aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="6bfd9-107">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="6bfd9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6bfd9-108">Properties</span></span>
|<span data-ttu-id="6bfd9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6bfd9-109">Property</span></span>|<span data-ttu-id="6bfd9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bfd9-110">Type</span></span>|<span data-ttu-id="6bfd9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bfd9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bfd9-112">displayName</span><span class="sxs-lookup"><span data-stu-id="6bfd9-112">displayName</span></span>|<span data-ttu-id="6bfd9-113">String</span><span class="sxs-lookup"><span data-stu-id="6bfd9-113">String</span></span>|<span data-ttu-id="6bfd9-114">Nome da página da pasta</span><span class="sxs-lookup"><span data-stu-id="6bfd9-114">Name of the folder page</span></span>|
|<span data-ttu-id="6bfd9-115">aplicativos</span><span class="sxs-lookup"><span data-stu-id="6bfd9-115">apps</span></span>|<span data-ttu-id="6bfd9-116">Conjunto [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="6bfd9-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="6bfd9-117">Uma lista de aplicativos exibidos em uma página dentro de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="6bfd9-117">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="6bfd9-118">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="6bfd9-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bfd9-119">Relações</span><span class="sxs-lookup"><span data-stu-id="6bfd9-119">Relationships</span></span>
<span data-ttu-id="6bfd9-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6bfd9-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6bfd9-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6bfd9-121">JSON Representation</span></span>
<span data-ttu-id="6bfd9-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6bfd9-122">Here is a JSON representation of the resource.</span></span>
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






