---
title: Tipo de recurso androidMobileAppIdentifier
description: O identificador de um app Android.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4d7c0f5d18d19fee11b7485e7e4aefc24ba94429
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43374299"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="88ff4-103">Tipo de recurso androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="88ff4-103">androidMobileAppIdentifier resource type</span></span>

<span data-ttu-id="88ff4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88ff4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88ff4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="88ff4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88ff4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88ff4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88ff4-107">O identificador de um app Android.</span><span class="sxs-lookup"><span data-stu-id="88ff4-107">The identifier for an Android app.</span></span>


<span data-ttu-id="88ff4-108">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="88ff4-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="88ff4-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88ff4-109">Properties</span></span>
|<span data-ttu-id="88ff4-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88ff4-110">Property</span></span>|<span data-ttu-id="88ff4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="88ff4-111">Type</span></span>|<span data-ttu-id="88ff4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="88ff4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88ff4-113">packageId</span><span class="sxs-lookup"><span data-stu-id="88ff4-113">packageId</span></span>|<span data-ttu-id="88ff4-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88ff4-114">String</span></span>|<span data-ttu-id="88ff4-115">O identificador de um app, como especificado na Play Store.</span><span class="sxs-lookup"><span data-stu-id="88ff4-115">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88ff4-116">Relações</span><span class="sxs-lookup"><span data-stu-id="88ff4-116">Relationships</span></span>
<span data-ttu-id="88ff4-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="88ff4-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88ff4-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88ff4-118">JSON Representation</span></span>
<span data-ttu-id="88ff4-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88ff4-119">Here is a JSON representation of the resource.</span></span>
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



