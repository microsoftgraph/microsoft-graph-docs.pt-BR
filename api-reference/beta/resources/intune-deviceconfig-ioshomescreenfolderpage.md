---
title: Tipo de recurso iosHomeScreenFolderPage
description: Uma pasta com os aplicativos na tela inicial
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1fa9462f8fb0640584515d1c209abd03de0e6200
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424172"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="33d43-103">Tipo de recurso iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="33d43-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="33d43-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="33d43-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="33d43-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="33d43-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33d43-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="33d43-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33d43-107">Uma pasta com os aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="33d43-107">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="33d43-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="33d43-108">Properties</span></span>
|<span data-ttu-id="33d43-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33d43-109">Property</span></span>|<span data-ttu-id="33d43-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="33d43-110">Type</span></span>|<span data-ttu-id="33d43-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="33d43-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33d43-112">displayName</span><span class="sxs-lookup"><span data-stu-id="33d43-112">displayName</span></span>|<span data-ttu-id="33d43-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="33d43-113">String</span></span>|<span data-ttu-id="33d43-114">Nome da página da pasta</span><span class="sxs-lookup"><span data-stu-id="33d43-114">Name of the folder page</span></span>|
|<span data-ttu-id="33d43-115">aplicativos</span><span class="sxs-lookup"><span data-stu-id="33d43-115">apps</span></span>|<span data-ttu-id="33d43-116">Conjunto [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="33d43-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="33d43-117">Uma lista de aplicativos exibidos em uma página dentro de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="33d43-117">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="33d43-118">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="33d43-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33d43-119">Relações</span><span class="sxs-lookup"><span data-stu-id="33d43-119">Relationships</span></span>
<span data-ttu-id="33d43-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="33d43-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="33d43-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="33d43-121">JSON Representation</span></span>
<span data-ttu-id="33d43-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="33d43-122">Here is a JSON representation of the resource.</span></span>
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




