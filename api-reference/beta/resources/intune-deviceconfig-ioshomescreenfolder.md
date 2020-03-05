---
title: Tipo de recurso iosHomeScreenFolder
description: Uma pasta que contém as páginas de aplicativos na tela inicial
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ad2f9cb0f5530aeffbc840f2e7f38b5e0fde59a7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526357"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="1c490-103">Tipo de recurso iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="1c490-103">iosHomeScreenFolder resource type</span></span>

<span data-ttu-id="1c490-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1c490-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c490-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1c490-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c490-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1c490-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c490-107">Uma pasta que contém as páginas de aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="1c490-107">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="1c490-108">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c490-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1c490-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1c490-109">Properties</span></span>
|<span data-ttu-id="1c490-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c490-110">Property</span></span>|<span data-ttu-id="1c490-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c490-111">Type</span></span>|<span data-ttu-id="1c490-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c490-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c490-113">displayName</span><span class="sxs-lookup"><span data-stu-id="1c490-113">displayName</span></span>|<span data-ttu-id="1c490-114">String</span><span class="sxs-lookup"><span data-stu-id="1c490-114">String</span></span>|<span data-ttu-id="1c490-115">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c490-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="1c490-116">páginas</span><span class="sxs-lookup"><span data-stu-id="1c490-116">pages</span></span>|<span data-ttu-id="1c490-117">Conjunto [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="1c490-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="1c490-118">Páginas de ícones de layout da tela inicial que devem ser do tipo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1c490-118">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="1c490-119">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="1c490-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c490-120">Relações</span><span class="sxs-lookup"><span data-stu-id="1c490-120">Relationships</span></span>
<span data-ttu-id="1c490-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1c490-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c490-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1c490-122">JSON Representation</span></span>
<span data-ttu-id="1c490-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1c490-123">Here is a JSON representation of the resource.</span></span>
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



