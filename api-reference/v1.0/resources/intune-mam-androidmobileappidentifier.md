---
title: Tipo de recurso androidMobileAppIdentifier
description: O identificador de um app Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa3a0f90626ea01290ccd1d0eee3873374efb546
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261170"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="0b07a-103">Tipo de recurso androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="0b07a-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="0b07a-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0b07a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b07a-105">O identificador de um app Android.</span><span class="sxs-lookup"><span data-stu-id="0b07a-105">The identifier for an Android app.</span></span>


<span data-ttu-id="0b07a-106">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="0b07a-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0b07a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b07a-107">Properties</span></span>
|<span data-ttu-id="0b07a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b07a-108">Property</span></span>|<span data-ttu-id="0b07a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b07a-109">Type</span></span>|<span data-ttu-id="0b07a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b07a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b07a-111">packageId</span><span class="sxs-lookup"><span data-stu-id="0b07a-111">packageId</span></span>|<span data-ttu-id="0b07a-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b07a-112">String</span></span>|<span data-ttu-id="0b07a-113">O identificador de um app, como especificado na Play Store.</span><span class="sxs-lookup"><span data-stu-id="0b07a-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b07a-114">Relações</span><span class="sxs-lookup"><span data-stu-id="0b07a-114">Relationships</span></span>
<span data-ttu-id="0b07a-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b07a-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b07a-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b07a-116">JSON Representation</span></span>
<span data-ttu-id="0b07a-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b07a-117">Here is a JSON representation of the resource.</span></span>
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



