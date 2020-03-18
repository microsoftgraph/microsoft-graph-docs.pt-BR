---
title: Tipo de recurso androidMobileAppIdentifier
description: O identificador de um app Android.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bc998a09d30d94b42c6c118a51dc028b8251e134
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42782661"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="b0ce6-103">Tipo de recurso androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b0ce6-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="b0ce6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0ce6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0ce6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0ce6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0ce6-106">O identificador de um app Android.</span><span class="sxs-lookup"><span data-stu-id="b0ce6-106">The identifier for an Android app.</span></span>


<span data-ttu-id="b0ce6-107">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="b0ce6-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b0ce6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0ce6-108">Properties</span></span>
|<span data-ttu-id="b0ce6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0ce6-109">Property</span></span>|<span data-ttu-id="b0ce6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0ce6-110">Type</span></span>|<span data-ttu-id="b0ce6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0ce6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0ce6-112">packageId</span><span class="sxs-lookup"><span data-stu-id="b0ce6-112">packageId</span></span>|<span data-ttu-id="b0ce6-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0ce6-113">String</span></span>|<span data-ttu-id="b0ce6-114">O identificador de um app, como especificado na Play Store.</span><span class="sxs-lookup"><span data-stu-id="b0ce6-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0ce6-115">Relações</span><span class="sxs-lookup"><span data-stu-id="b0ce6-115">Relationships</span></span>
<span data-ttu-id="b0ce6-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0ce6-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0ce6-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0ce6-117">JSON Representation</span></span>
<span data-ttu-id="b0ce6-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0ce6-118">Here is a JSON representation of the resource.</span></span>
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



