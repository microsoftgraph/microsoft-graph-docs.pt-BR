---
title: Tipo de recurso androidMobileAppIdentifier
description: O identificador de um app Android.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9cc203cc9268849e8b7b46d994c166378252df59
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871740"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="f0075-103">Tipo de recurso androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="f0075-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="f0075-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f0075-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0075-105">O identificador de um app Android.</span><span class="sxs-lookup"><span data-stu-id="f0075-105">The identifier for an Android app.</span></span>

<span data-ttu-id="f0075-106">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="f0075-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f0075-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0075-107">Properties</span></span>
|<span data-ttu-id="f0075-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0075-108">Property</span></span>|<span data-ttu-id="f0075-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0075-109">Type</span></span>|<span data-ttu-id="f0075-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0075-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0075-111">packageId</span><span class="sxs-lookup"><span data-stu-id="f0075-111">packageId</span></span>|<span data-ttu-id="f0075-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0075-112">String</span></span>|<span data-ttu-id="f0075-113">O identificador de um app, como especificado na Play Store.</span><span class="sxs-lookup"><span data-stu-id="f0075-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0075-114">Relações</span><span class="sxs-lookup"><span data-stu-id="f0075-114">Relationships</span></span>
<span data-ttu-id="f0075-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f0075-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f0075-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0075-116">JSON Representation</span></span>
<span data-ttu-id="f0075-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0075-117">Here is a JSON representation of the resource.</span></span>
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



