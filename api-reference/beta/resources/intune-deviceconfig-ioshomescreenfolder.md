---
title: Tipo de recurso iosHomeScreenFolder
description: Uma pasta que contém as páginas de aplicativos na tela inicial
ms.openlocfilehash: 005b35f014cf6ee6967cfa5dfaa235aede155be3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039538"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="d2bf2-103">Tipo de recurso iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="d2bf2-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="d2bf2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d2bf2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2bf2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d2bf2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2bf2-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d2bf2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2bf2-107">Uma pasta que contém as páginas de aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="d2bf2-107">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="d2bf2-108">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="d2bf2-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d2bf2-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2bf2-109">Properties</span></span>
|<span data-ttu-id="d2bf2-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2bf2-110">Property</span></span>|<span data-ttu-id="d2bf2-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2bf2-111">Type</span></span>|<span data-ttu-id="d2bf2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2bf2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2bf2-113">displayName</span><span class="sxs-lookup"><span data-stu-id="d2bf2-113">displayName</span></span>|<span data-ttu-id="d2bf2-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2bf2-114">String</span></span>|<span data-ttu-id="d2bf2-115">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="d2bf2-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="d2bf2-116">páginas</span><span class="sxs-lookup"><span data-stu-id="d2bf2-116">pages</span></span>|<span data-ttu-id="d2bf2-117">Conjunto [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="d2bf2-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="d2bf2-118">Páginas de ícones de layout da tela inicial que devem ser do tipo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d2bf2-118">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="d2bf2-119">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d2bf2-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2bf2-120">Relações</span><span class="sxs-lookup"><span data-stu-id="d2bf2-120">Relationships</span></span>
<span data-ttu-id="d2bf2-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2bf2-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d2bf2-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2bf2-122">JSON Representation</span></span>
<span data-ttu-id="d2bf2-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2bf2-123">Here is a JSON representation of the resource.</span></span>
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





