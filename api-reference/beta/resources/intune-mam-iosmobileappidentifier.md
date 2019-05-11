---
title: Tipo de recurso iosMobileAppIdentifier
description: O identificador de um aplicativo iOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c7da88947c4033f1af615f85267a23426c5e4154
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940873"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="c90e9-103">Tipo de recurso iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c90e9-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="c90e9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c90e9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c90e9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c90e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c90e9-106">O identificador de um aplicativo iOS.</span><span class="sxs-lookup"><span data-stu-id="c90e9-106">The identifier for an iOS app.</span></span>


<span data-ttu-id="c90e9-107">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="c90e9-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c90e9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c90e9-108">Properties</span></span>
|<span data-ttu-id="c90e9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c90e9-109">Property</span></span>|<span data-ttu-id="c90e9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c90e9-110">Type</span></span>|<span data-ttu-id="c90e9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c90e9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c90e9-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="c90e9-112">bundleId</span></span>|<span data-ttu-id="c90e9-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c90e9-113">String</span></span>|<span data-ttu-id="c90e9-114">O identificador de um aplicativo, conforme especificado na App Store.</span><span class="sxs-lookup"><span data-stu-id="c90e9-114">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c90e9-115">Relações</span><span class="sxs-lookup"><span data-stu-id="c90e9-115">Relationships</span></span>
<span data-ttu-id="c90e9-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c90e9-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c90e9-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c90e9-117">JSON Representation</span></span>
<span data-ttu-id="c90e9-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c90e9-118">Here is a JSON representation of the resource.</span></span>
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




