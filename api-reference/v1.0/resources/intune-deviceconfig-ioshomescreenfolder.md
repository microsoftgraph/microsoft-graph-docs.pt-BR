---
title: Tipo de recurso iosHomeScreenFolder
description: Uma pasta que contém páginas de aplicativos e clipes da Web na Tela Inicial.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4ee4d2f1119a7fb6c4318b2afd195518f4b8095b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760068"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="d3657-103">Tipo de recurso iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="d3657-103">iosHomeScreenFolder resource type</span></span>

<span data-ttu-id="d3657-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3657-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3657-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3657-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3657-106">Uma pasta que contém páginas de aplicativos e clipes da Web na Tela Inicial.</span><span class="sxs-lookup"><span data-stu-id="d3657-106">A folder containing pages of apps and web clips on the Home Screen.</span></span>


<span data-ttu-id="d3657-107">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="d3657-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d3657-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3657-108">Properties</span></span>
|<span data-ttu-id="d3657-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3657-109">Property</span></span>|<span data-ttu-id="d3657-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3657-110">Type</span></span>|<span data-ttu-id="d3657-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3657-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3657-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d3657-112">displayName</span></span>|<span data-ttu-id="d3657-113">String</span><span class="sxs-lookup"><span data-stu-id="d3657-113">String</span></span>|<span data-ttu-id="d3657-114">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="d3657-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="d3657-115">páginas</span><span class="sxs-lookup"><span data-stu-id="d3657-115">pages</span></span>|<span data-ttu-id="d3657-116">Conjunto [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="d3657-116">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="d3657-117">Páginas de Ícones de Layout da Tela Inicial que devem ser aplicativos ou clipes da Web.</span><span class="sxs-lookup"><span data-stu-id="d3657-117">Pages of Home Screen Layout Icons which must be applications or web clips.</span></span> <span data-ttu-id="d3657-118">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d3657-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3657-119">Relações</span><span class="sxs-lookup"><span data-stu-id="d3657-119">Relationships</span></span>
<span data-ttu-id="d3657-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d3657-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3657-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3657-121">JSON Representation</span></span>
<span data-ttu-id="d3657-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d3657-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
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
```




