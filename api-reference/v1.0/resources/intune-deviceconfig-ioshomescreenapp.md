---
title: Tipo de recurso iosHomeScreenApp
description: Representa um ícone de um aplicativo na tela inicial
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cc4e94071e7b81fab82044f65da809f7b17e5b3f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028214"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="da1d6-103">Tipo de recurso iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="da1d6-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="da1d6-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="da1d6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da1d6-105">Representa um ícone de um aplicativo na tela inicial</span><span class="sxs-lookup"><span data-stu-id="da1d6-105">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="da1d6-106">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="da1d6-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="da1d6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da1d6-107">Properties</span></span>
|<span data-ttu-id="da1d6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da1d6-108">Property</span></span>|<span data-ttu-id="da1d6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="da1d6-109">Type</span></span>|<span data-ttu-id="da1d6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="da1d6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da1d6-111">displayName</span><span class="sxs-lookup"><span data-stu-id="da1d6-111">displayName</span></span>|<span data-ttu-id="da1d6-112">String</span><span class="sxs-lookup"><span data-stu-id="da1d6-112">String</span></span>|<span data-ttu-id="da1d6-113">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="da1d6-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="da1d6-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="da1d6-114">bundleID</span></span>|<span data-ttu-id="da1d6-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="da1d6-115">String</span></span>|<span data-ttu-id="da1d6-116">BundleID do aplicativo</span><span class="sxs-lookup"><span data-stu-id="da1d6-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="da1d6-117">Relações</span><span class="sxs-lookup"><span data-stu-id="da1d6-117">Relationships</span></span>
<span data-ttu-id="da1d6-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="da1d6-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da1d6-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da1d6-119">JSON Representation</span></span>
<span data-ttu-id="da1d6-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da1d6-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```



