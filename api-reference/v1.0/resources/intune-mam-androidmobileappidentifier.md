---
title: Tipo de recurso androidMobileAppIdentifier
description: O identificador de um app Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3d34ff19e37a3453458621fb0876cb1a04b55308
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978010"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="e75cd-103">Tipo de recurso androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="e75cd-103">androidMobileAppIdentifier resource type</span></span>

<span data-ttu-id="e75cd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e75cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e75cd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e75cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e75cd-106">O identificador de um app Android.</span><span class="sxs-lookup"><span data-stu-id="e75cd-106">The identifier for an Android app.</span></span>


<span data-ttu-id="e75cd-107">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="e75cd-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e75cd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e75cd-108">Properties</span></span>
|<span data-ttu-id="e75cd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e75cd-109">Property</span></span>|<span data-ttu-id="e75cd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e75cd-110">Type</span></span>|<span data-ttu-id="e75cd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e75cd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e75cd-112">packageId</span><span class="sxs-lookup"><span data-stu-id="e75cd-112">packageId</span></span>|<span data-ttu-id="e75cd-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e75cd-113">String</span></span>|<span data-ttu-id="e75cd-114">O identificador de um app, como especificado na Play Store.</span><span class="sxs-lookup"><span data-stu-id="e75cd-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e75cd-115">Relações</span><span class="sxs-lookup"><span data-stu-id="e75cd-115">Relationships</span></span>
<span data-ttu-id="e75cd-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e75cd-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e75cd-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e75cd-117">JSON Representation</span></span>
<span data-ttu-id="e75cd-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e75cd-118">Here is a JSON representation of the resource.</span></span>
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









