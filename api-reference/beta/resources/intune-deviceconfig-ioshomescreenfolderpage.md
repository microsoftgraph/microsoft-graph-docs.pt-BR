---
title: Tipo de recurso iosHomeScreenFolderPage
description: Uma pasta com os aplicativos na tela inicial
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 38b1d898cb4bc1eacaa427ed412b536ba40cd0f9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941958"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="0ff40-103">Tipo de recurso iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="0ff40-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="0ff40-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0ff40-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ff40-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0ff40-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ff40-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0ff40-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ff40-107">Uma pasta com os aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="0ff40-107">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="0ff40-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ff40-108">Properties</span></span>
|<span data-ttu-id="0ff40-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ff40-109">Property</span></span>|<span data-ttu-id="0ff40-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ff40-110">Type</span></span>|<span data-ttu-id="0ff40-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ff40-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ff40-112">displayName</span><span class="sxs-lookup"><span data-stu-id="0ff40-112">displayName</span></span>|<span data-ttu-id="0ff40-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ff40-113">String</span></span>|<span data-ttu-id="0ff40-114">Nome da página da pasta</span><span class="sxs-lookup"><span data-stu-id="0ff40-114">Name of the folder page</span></span>|
|<span data-ttu-id="0ff40-115">aplicativos</span><span class="sxs-lookup"><span data-stu-id="0ff40-115">apps</span></span>|<span data-ttu-id="0ff40-116">Conjunto [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="0ff40-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="0ff40-117">Uma lista de aplicativos exibidos em uma página dentro de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="0ff40-117">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="0ff40-118">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="0ff40-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ff40-119">Relações</span><span class="sxs-lookup"><span data-stu-id="0ff40-119">Relationships</span></span>
<span data-ttu-id="0ff40-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0ff40-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0ff40-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ff40-121">JSON Representation</span></span>
<span data-ttu-id="0ff40-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ff40-122">Here is a JSON representation of the resource.</span></span>
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





