---
title: Tipo de recurso androidMobileAppIdentifier
description: O identificador de um app Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a26d5ec654749b23a78052d1e9a392857462b8c5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030566"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="c33a8-103">Tipo de recurso androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c33a8-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="c33a8-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c33a8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c33a8-105">O identificador de um app Android.</span><span class="sxs-lookup"><span data-stu-id="c33a8-105">The identifier for an Android app.</span></span>


<span data-ttu-id="c33a8-106">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="c33a8-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c33a8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c33a8-107">Properties</span></span>
|<span data-ttu-id="c33a8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c33a8-108">Property</span></span>|<span data-ttu-id="c33a8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c33a8-109">Type</span></span>|<span data-ttu-id="c33a8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c33a8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c33a8-111">packageId</span><span class="sxs-lookup"><span data-stu-id="c33a8-111">packageId</span></span>|<span data-ttu-id="c33a8-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c33a8-112">String</span></span>|<span data-ttu-id="c33a8-113">O identificador de um app, como especificado na Play Store.</span><span class="sxs-lookup"><span data-stu-id="c33a8-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c33a8-114">Relações</span><span class="sxs-lookup"><span data-stu-id="c33a8-114">Relationships</span></span>
<span data-ttu-id="c33a8-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c33a8-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c33a8-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c33a8-116">JSON Representation</span></span>
<span data-ttu-id="c33a8-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c33a8-117">Here is a JSON representation of the resource.</span></span>
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



