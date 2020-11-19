---
title: Tipo de recurso iosHomeScreenFolder
description: Uma pasta que contém as páginas de aplicativos na tela inicial
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4571baad6e1e0967b8b38ced9b96fd977f154fd7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280421"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="63dab-103">Tipo de recurso iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="63dab-103">iosHomeScreenFolder resource type</span></span>

<span data-ttu-id="63dab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63dab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63dab-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="63dab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63dab-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63dab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63dab-107">Uma pasta que contém as páginas de aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="63dab-107">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="63dab-108">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="63dab-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="63dab-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="63dab-109">Properties</span></span>
|<span data-ttu-id="63dab-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63dab-110">Property</span></span>|<span data-ttu-id="63dab-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="63dab-111">Type</span></span>|<span data-ttu-id="63dab-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="63dab-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63dab-113">displayName</span><span class="sxs-lookup"><span data-stu-id="63dab-113">displayName</span></span>|<span data-ttu-id="63dab-114">String</span><span class="sxs-lookup"><span data-stu-id="63dab-114">String</span></span>|<span data-ttu-id="63dab-115">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="63dab-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="63dab-116">páginas</span><span class="sxs-lookup"><span data-stu-id="63dab-116">pages</span></span>|<span data-ttu-id="63dab-117">Conjunto [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="63dab-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="63dab-118">Páginas de ícones de layout da tela inicial que devem ser do tipo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="63dab-118">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="63dab-119">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="63dab-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63dab-120">Relações</span><span class="sxs-lookup"><span data-stu-id="63dab-120">Relationships</span></span>
<span data-ttu-id="63dab-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="63dab-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63dab-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="63dab-122">JSON Representation</span></span>
<span data-ttu-id="63dab-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="63dab-123">Here is a JSON representation of the resource.</span></span>
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




