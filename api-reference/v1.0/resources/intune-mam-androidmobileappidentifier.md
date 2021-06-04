---
title: Tipo de recurso androidMobileAppIdentifier
description: O identificador de um app Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 07dcc1bd7480439f5c1dd71afa36e18a5df0eb14
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754529"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="97688-103">Tipo de recurso androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="97688-103">androidMobileAppIdentifier resource type</span></span>

<span data-ttu-id="97688-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97688-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97688-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="97688-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97688-106">O identificador de um app Android.</span><span class="sxs-lookup"><span data-stu-id="97688-106">The identifier for an Android app.</span></span>


<span data-ttu-id="97688-107">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="97688-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="97688-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="97688-108">Properties</span></span>
|<span data-ttu-id="97688-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97688-109">Property</span></span>|<span data-ttu-id="97688-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="97688-110">Type</span></span>|<span data-ttu-id="97688-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="97688-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97688-112">packageId</span><span class="sxs-lookup"><span data-stu-id="97688-112">packageId</span></span>|<span data-ttu-id="97688-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97688-113">String</span></span>|<span data-ttu-id="97688-114">O identificador de um app, como especificado na Play Store.</span><span class="sxs-lookup"><span data-stu-id="97688-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97688-115">Relações</span><span class="sxs-lookup"><span data-stu-id="97688-115">Relationships</span></span>
<span data-ttu-id="97688-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="97688-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97688-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97688-117">JSON Representation</span></span>
<span data-ttu-id="97688-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="97688-118">Here is a JSON representation of the resource.</span></span>
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




