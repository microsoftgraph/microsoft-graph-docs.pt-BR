---
title: Tipo de recurso androidMobileAppIdentifier
description: O identificador de um app Android.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0b610cbfa4ba7296a9b8427b9bb49f7b4493f773
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474121"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="454f2-103">Tipo de recurso androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="454f2-103">androidMobileAppIdentifier resource type</span></span>

<span data-ttu-id="454f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="454f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="454f2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="454f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="454f2-106">O identificador de um app Android.</span><span class="sxs-lookup"><span data-stu-id="454f2-106">The identifier for an Android app.</span></span>


<span data-ttu-id="454f2-107">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="454f2-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="454f2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="454f2-108">Properties</span></span>
|<span data-ttu-id="454f2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="454f2-109">Property</span></span>|<span data-ttu-id="454f2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="454f2-110">Type</span></span>|<span data-ttu-id="454f2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="454f2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="454f2-112">packageId</span><span class="sxs-lookup"><span data-stu-id="454f2-112">packageId</span></span>|<span data-ttu-id="454f2-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="454f2-113">String</span></span>|<span data-ttu-id="454f2-114">O identificador de um app, como especificado na Play Store.</span><span class="sxs-lookup"><span data-stu-id="454f2-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="454f2-115">Relações</span><span class="sxs-lookup"><span data-stu-id="454f2-115">Relationships</span></span>
<span data-ttu-id="454f2-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="454f2-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="454f2-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="454f2-117">JSON Representation</span></span>
<span data-ttu-id="454f2-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="454f2-118">Here is a JSON representation of the resource.</span></span>
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







