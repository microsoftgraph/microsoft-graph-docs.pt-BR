---
title: Tipo de recurso iosHomeScreenApp
description: Representa um ícone de um aplicativo na tela inicial
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de16278256e9c6860a3cdead2ab5e940d0878a1a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760075"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="6b21f-103">Tipo de recurso iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="6b21f-103">iosHomeScreenApp resource type</span></span>

<span data-ttu-id="6b21f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b21f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b21f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b21f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b21f-106">Representa um ícone de um aplicativo na tela inicial</span><span class="sxs-lookup"><span data-stu-id="6b21f-106">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="6b21f-107">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="6b21f-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6b21f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b21f-108">Properties</span></span>
|<span data-ttu-id="6b21f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b21f-109">Property</span></span>|<span data-ttu-id="6b21f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b21f-110">Type</span></span>|<span data-ttu-id="6b21f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b21f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b21f-112">displayName</span><span class="sxs-lookup"><span data-stu-id="6b21f-112">displayName</span></span>|<span data-ttu-id="6b21f-113">String</span><span class="sxs-lookup"><span data-stu-id="6b21f-113">String</span></span>|<span data-ttu-id="6b21f-114">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="6b21f-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="6b21f-115">bundleID</span><span class="sxs-lookup"><span data-stu-id="6b21f-115">bundleID</span></span>|<span data-ttu-id="6b21f-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b21f-116">String</span></span>|<span data-ttu-id="6b21f-117">BundleID do aplicativo se forWebClip for false ou a URL de um clipe da Web se forWebClip for true.</span><span class="sxs-lookup"><span data-stu-id="6b21f-117">BundleID of the app if isWebClip is false or the URL of a web clip if isWebClip is true.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b21f-118">Relações</span><span class="sxs-lookup"><span data-stu-id="6b21f-118">Relationships</span></span>
<span data-ttu-id="6b21f-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b21f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b21f-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b21f-120">JSON Representation</span></span>
<span data-ttu-id="6b21f-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b21f-121">Here is a JSON representation of the resource.</span></span>
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




