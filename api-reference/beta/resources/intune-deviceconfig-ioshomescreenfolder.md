---
title: Tipo de recurso iosHomeScreenFolder
description: Uma pasta que contém as páginas de aplicativos na tela inicial
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 36ea4a00b9310623027179e1d6d2e1c64888c470
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407505"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="a3537-103">Tipo de recurso iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="a3537-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="a3537-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="a3537-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a3537-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a3537-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3537-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="a3537-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3537-107">Uma pasta que contém as páginas de aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="a3537-107">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="a3537-108">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="a3537-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a3537-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a3537-109">Properties</span></span>
|<span data-ttu-id="a3537-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3537-110">Property</span></span>|<span data-ttu-id="a3537-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3537-111">Type</span></span>|<span data-ttu-id="a3537-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3537-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3537-113">displayName</span><span class="sxs-lookup"><span data-stu-id="a3537-113">displayName</span></span>|<span data-ttu-id="a3537-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3537-114">String</span></span>|<span data-ttu-id="a3537-115">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="a3537-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="a3537-116">páginas</span><span class="sxs-lookup"><span data-stu-id="a3537-116">pages</span></span>|<span data-ttu-id="a3537-117">Conjunto [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="a3537-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="a3537-118">Páginas de ícones de layout da tela inicial que devem ser do tipo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a3537-118">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="a3537-119">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="a3537-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3537-120">Relações</span><span class="sxs-lookup"><span data-stu-id="a3537-120">Relationships</span></span>
<span data-ttu-id="a3537-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a3537-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3537-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a3537-122">JSON Representation</span></span>
<span data-ttu-id="a3537-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a3537-123">Here is a JSON representation of the resource.</span></span>
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




