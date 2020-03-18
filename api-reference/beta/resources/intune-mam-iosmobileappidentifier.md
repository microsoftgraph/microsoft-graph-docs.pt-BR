---
title: Tipo de recurso iosMobileAppIdentifier
description: O identificador de um aplicativo iOS.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 10744d417738baf6f0d83a287a5e518fa6e55b60
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42782360"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="d5e0c-103">Tipo de recurso iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d5e0c-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="d5e0c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d5e0c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5e0c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d5e0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5e0c-106">O identificador de um aplicativo iOS.</span><span class="sxs-lookup"><span data-stu-id="d5e0c-106">The identifier for an iOS app.</span></span>


<span data-ttu-id="d5e0c-107">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="d5e0c-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d5e0c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5e0c-108">Properties</span></span>
|<span data-ttu-id="d5e0c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5e0c-109">Property</span></span>|<span data-ttu-id="d5e0c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5e0c-110">Type</span></span>|<span data-ttu-id="d5e0c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5e0c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5e0c-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="d5e0c-112">bundleId</span></span>|<span data-ttu-id="d5e0c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5e0c-113">String</span></span>|<span data-ttu-id="d5e0c-114">O identificador de um aplicativo, conforme especificado na App Store.</span><span class="sxs-lookup"><span data-stu-id="d5e0c-114">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5e0c-115">Relações</span><span class="sxs-lookup"><span data-stu-id="d5e0c-115">Relationships</span></span>
<span data-ttu-id="d5e0c-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5e0c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5e0c-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5e0c-117">JSON Representation</span></span>
<span data-ttu-id="d5e0c-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5e0c-118">Here is a JSON representation of the resource.</span></span>
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



