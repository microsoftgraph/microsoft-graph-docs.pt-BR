---
title: Tipo de recurso androidMobileAppIdentifier
description: O identificador de um app Android.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a3d8e0c1df2b996a8ae13cbdd8ff3424f10a775a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356559"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="d321f-103">Tipo de recurso androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d321f-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="d321f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d321f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d321f-105">O identificador de um app Android.</span><span class="sxs-lookup"><span data-stu-id="d321f-105">The identifier for an Android app.</span></span>


<span data-ttu-id="d321f-106">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="d321f-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d321f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d321f-107">Properties</span></span>
|<span data-ttu-id="d321f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d321f-108">Property</span></span>|<span data-ttu-id="d321f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d321f-109">Type</span></span>|<span data-ttu-id="d321f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d321f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d321f-111">packageId</span><span class="sxs-lookup"><span data-stu-id="d321f-111">packageId</span></span>|<span data-ttu-id="d321f-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d321f-112">String</span></span>|<span data-ttu-id="d321f-113">O identificador de um app, como especificado na Play Store.</span><span class="sxs-lookup"><span data-stu-id="d321f-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d321f-114">Relações</span><span class="sxs-lookup"><span data-stu-id="d321f-114">Relationships</span></span>
<span data-ttu-id="d321f-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d321f-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d321f-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d321f-116">JSON Representation</span></span>
<span data-ttu-id="d321f-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d321f-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMobileAppIdentifier",
  "packageId": "String"
}
```




