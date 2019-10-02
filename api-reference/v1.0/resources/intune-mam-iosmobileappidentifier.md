---
title: Tipo de recurso iosMobileAppIdentifier
description: O identificador de um aplicativo iOS.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c85d0f1a2bedffe8525c2012487646c4364ec2ff
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356496"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="ddab8-103">Tipo de recurso iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ddab8-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="ddab8-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ddab8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddab8-105">O identificador de um aplicativo iOS.</span><span class="sxs-lookup"><span data-stu-id="ddab8-105">The identifier for an iOS app.</span></span>


<span data-ttu-id="ddab8-106">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="ddab8-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ddab8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ddab8-107">Properties</span></span>
|<span data-ttu-id="ddab8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ddab8-108">Property</span></span>|<span data-ttu-id="ddab8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddab8-109">Type</span></span>|<span data-ttu-id="ddab8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddab8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddab8-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="ddab8-111">bundleId</span></span>|<span data-ttu-id="ddab8-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddab8-112">String</span></span>|<span data-ttu-id="ddab8-113">O identificador de um aplicativo, conforme especificado na App Store.</span><span class="sxs-lookup"><span data-stu-id="ddab8-113">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddab8-114">Relações</span><span class="sxs-lookup"><span data-stu-id="ddab8-114">Relationships</span></span>
<span data-ttu-id="ddab8-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ddab8-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ddab8-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ddab8-116">JSON Representation</span></span>
<span data-ttu-id="ddab8-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ddab8-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppIdentifier",
  "bundleId": "String"
}
```




