---
title: Tipo de recurso iosHomeScreenApp
description: Representa um ícone de um aplicativo na tela inicial
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 67c11096414db0dccad2ccf56ec184a4e3f30397
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554734"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="21fe5-103">Tipo de recurso iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="21fe5-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="21fe5-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21fe5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21fe5-105">Representa um ícone de um aplicativo na tela inicial</span><span class="sxs-lookup"><span data-stu-id="21fe5-105">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="21fe5-106">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="21fe5-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="21fe5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21fe5-107">Properties</span></span>
|<span data-ttu-id="21fe5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21fe5-108">Property</span></span>|<span data-ttu-id="21fe5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="21fe5-109">Type</span></span>|<span data-ttu-id="21fe5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="21fe5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21fe5-111">displayName</span><span class="sxs-lookup"><span data-stu-id="21fe5-111">displayName</span></span>|<span data-ttu-id="21fe5-112">String</span><span class="sxs-lookup"><span data-stu-id="21fe5-112">String</span></span>|<span data-ttu-id="21fe5-113">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="21fe5-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="21fe5-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="21fe5-114">bundleID</span></span>|<span data-ttu-id="21fe5-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21fe5-115">String</span></span>|<span data-ttu-id="21fe5-116">BundleID do aplicativo</span><span class="sxs-lookup"><span data-stu-id="21fe5-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="21fe5-117">Relações</span><span class="sxs-lookup"><span data-stu-id="21fe5-117">Relationships</span></span>
<span data-ttu-id="21fe5-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="21fe5-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21fe5-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21fe5-119">JSON Representation</span></span>
<span data-ttu-id="21fe5-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21fe5-120">Here is a JSON representation of the resource.</span></span>
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



