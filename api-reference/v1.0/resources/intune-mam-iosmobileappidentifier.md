---
title: Tipo de recurso iosMobileAppIdentifier
description: O identificador de um aplicativo iOS.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 088f5507051676d587334966b91d4d4d1e8a135c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468559"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="710b6-103">Tipo de recurso iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="710b6-103">iosMobileAppIdentifier resource type</span></span>

<span data-ttu-id="710b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="710b6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="710b6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="710b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="710b6-106">O identificador de um aplicativo iOS.</span><span class="sxs-lookup"><span data-stu-id="710b6-106">The identifier for an iOS app.</span></span>


<span data-ttu-id="710b6-107">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="710b6-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="710b6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="710b6-108">Properties</span></span>
|<span data-ttu-id="710b6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="710b6-109">Property</span></span>|<span data-ttu-id="710b6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="710b6-110">Type</span></span>|<span data-ttu-id="710b6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="710b6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="710b6-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="710b6-112">bundleId</span></span>|<span data-ttu-id="710b6-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="710b6-113">String</span></span>|<span data-ttu-id="710b6-114">O identificador de um aplicativo, conforme especificado na App Store.</span><span class="sxs-lookup"><span data-stu-id="710b6-114">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="710b6-115">Relações</span><span class="sxs-lookup"><span data-stu-id="710b6-115">Relationships</span></span>
<span data-ttu-id="710b6-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="710b6-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="710b6-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="710b6-117">JSON Representation</span></span>
<span data-ttu-id="710b6-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="710b6-118">Here is a JSON representation of the resource.</span></span>
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







