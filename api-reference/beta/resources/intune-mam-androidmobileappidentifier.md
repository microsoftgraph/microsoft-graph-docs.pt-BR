---
title: Tipo de recurso androidMobileAppIdentifier
description: O identificador de um app Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ca2a2d9d548a94651514d1b3db2b385b5dc64bd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940901"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="65684-103">Tipo de recurso androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="65684-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="65684-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="65684-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65684-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="65684-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65684-106">O identificador de um app Android.</span><span class="sxs-lookup"><span data-stu-id="65684-106">The identifier for an Android app.</span></span>


<span data-ttu-id="65684-107">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="65684-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="65684-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65684-108">Properties</span></span>
|<span data-ttu-id="65684-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65684-109">Property</span></span>|<span data-ttu-id="65684-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="65684-110">Type</span></span>|<span data-ttu-id="65684-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="65684-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65684-112">packageId</span><span class="sxs-lookup"><span data-stu-id="65684-112">packageId</span></span>|<span data-ttu-id="65684-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65684-113">String</span></span>|<span data-ttu-id="65684-114">O identificador de um app, como especificado na Play Store.</span><span class="sxs-lookup"><span data-stu-id="65684-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65684-115">Relações</span><span class="sxs-lookup"><span data-stu-id="65684-115">Relationships</span></span>
<span data-ttu-id="65684-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="65684-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65684-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65684-117">JSON Representation</span></span>
<span data-ttu-id="65684-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65684-118">Here is a JSON representation of the resource.</span></span>
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




