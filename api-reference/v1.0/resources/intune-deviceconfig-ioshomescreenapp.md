---
title: Tipo de recurso iosHomeScreenApp
description: Representa um ícone de um aplicativo na tela inicial
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 55dacfcd7e16647c618d869fadc16d5b3c1cbc92
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984464"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="a409d-103">Tipo de recurso iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="a409d-103">iosHomeScreenApp resource type</span></span>

<span data-ttu-id="a409d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a409d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a409d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a409d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a409d-106">Representa um ícone de um aplicativo na tela inicial</span><span class="sxs-lookup"><span data-stu-id="a409d-106">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="a409d-107">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="a409d-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a409d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a409d-108">Properties</span></span>
|<span data-ttu-id="a409d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a409d-109">Property</span></span>|<span data-ttu-id="a409d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a409d-110">Type</span></span>|<span data-ttu-id="a409d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a409d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a409d-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a409d-112">displayName</span></span>|<span data-ttu-id="a409d-113">String</span><span class="sxs-lookup"><span data-stu-id="a409d-113">String</span></span>|<span data-ttu-id="a409d-114">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="a409d-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="a409d-115">bundleID</span><span class="sxs-lookup"><span data-stu-id="a409d-115">bundleID</span></span>|<span data-ttu-id="a409d-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a409d-116">String</span></span>|<span data-ttu-id="a409d-117">BundleID do aplicativo</span><span class="sxs-lookup"><span data-stu-id="a409d-117">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="a409d-118">Relações</span><span class="sxs-lookup"><span data-stu-id="a409d-118">Relationships</span></span>
<span data-ttu-id="a409d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a409d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a409d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a409d-120">JSON Representation</span></span>
<span data-ttu-id="a409d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a409d-121">Here is a JSON representation of the resource.</span></span>
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









