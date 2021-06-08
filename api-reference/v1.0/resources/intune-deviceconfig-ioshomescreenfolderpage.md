---
title: Tipo de recurso iosHomeScreenFolderPage
description: Uma página para uma pasta que contém aplicativos e clipes da Web na Tela Inicial.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9a8fc93d365dc842886f3346b86ff632f3ced7cb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760061"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="03817-103">Tipo de recurso iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="03817-103">iosHomeScreenFolderPage resource type</span></span>

<span data-ttu-id="03817-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03817-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03817-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="03817-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03817-106">Uma página para uma pasta que contém aplicativos e clipes da Web na Tela Inicial.</span><span class="sxs-lookup"><span data-stu-id="03817-106">A page for a folder containing apps and web clips on the Home Screen.</span></span>

## <a name="properties"></a><span data-ttu-id="03817-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03817-107">Properties</span></span>
|<span data-ttu-id="03817-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03817-108">Property</span></span>|<span data-ttu-id="03817-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="03817-109">Type</span></span>|<span data-ttu-id="03817-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="03817-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03817-111">displayName</span><span class="sxs-lookup"><span data-stu-id="03817-111">displayName</span></span>|<span data-ttu-id="03817-112">String</span><span class="sxs-lookup"><span data-stu-id="03817-112">String</span></span>|<span data-ttu-id="03817-113">Nome da página da pasta</span><span class="sxs-lookup"><span data-stu-id="03817-113">Name of the folder page</span></span>|
|<span data-ttu-id="03817-114">aplicativos</span><span class="sxs-lookup"><span data-stu-id="03817-114">apps</span></span>|<span data-ttu-id="03817-115">Conjunto [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="03817-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="03817-116">Uma lista de aplicativos e clipes da Web a ser exibida em uma página dentro de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="03817-116">A list of apps and web clips to appear on a page within a folder.</span></span> <span data-ttu-id="03817-117">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="03817-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03817-118">Relações</span><span class="sxs-lookup"><span data-stu-id="03817-118">Relationships</span></span>
<span data-ttu-id="03817-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="03817-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="03817-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03817-120">JSON Representation</span></span>
<span data-ttu-id="03817-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03817-121">Here is a JSON representation of the resource.</span></span>
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




