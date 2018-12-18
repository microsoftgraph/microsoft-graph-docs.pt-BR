---
title: Tipo de recurso iosHomeScreenFolderPage
description: Uma pasta com os aplicativos na tela inicial
author: tfitzmac
ms.openlocfilehash: 147504fc356f3a4092b2ffd1c7d03275ff7dea31
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353638"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="c27cb-103">Tipo de recurso iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="c27cb-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="c27cb-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c27cb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c27cb-105">Uma pasta com os aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="c27cb-105">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="c27cb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c27cb-106">Properties</span></span>
|<span data-ttu-id="c27cb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c27cb-107">Property</span></span>|<span data-ttu-id="c27cb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c27cb-108">Type</span></span>|<span data-ttu-id="c27cb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c27cb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c27cb-110">displayName</span><span class="sxs-lookup"><span data-stu-id="c27cb-110">displayName</span></span>|<span data-ttu-id="c27cb-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c27cb-111">String</span></span>|<span data-ttu-id="c27cb-112">Nome da página da pasta</span><span class="sxs-lookup"><span data-stu-id="c27cb-112">Name of the folder page</span></span>|
|<span data-ttu-id="c27cb-113">aplicativos</span><span class="sxs-lookup"><span data-stu-id="c27cb-113">apps</span></span>|<span data-ttu-id="c27cb-114">Conjunto [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="c27cb-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="c27cb-115">Uma lista de aplicativos exibidos em uma página dentro de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="c27cb-115">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="c27cb-116">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c27cb-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c27cb-117">Relações</span><span class="sxs-lookup"><span data-stu-id="c27cb-117">Relationships</span></span>
<span data-ttu-id="c27cb-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c27cb-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c27cb-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c27cb-119">JSON Representation</span></span>
<span data-ttu-id="c27cb-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c27cb-120">Here is a JSON representation of the resource.</span></span>
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



