---
title: Tipo de recurso androidMobileAppIdentifier
description: O identificador de um app Android.
ms.openlocfilehash: 16f142c40083b9410f84e128951680ced269ea12
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005856"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="92a01-103">Tipo de recurso androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="92a01-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="92a01-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="92a01-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92a01-105">O identificador de um app Android.</span><span class="sxs-lookup"><span data-stu-id="92a01-105">The identifier for an Android app.</span></span>

<span data-ttu-id="92a01-106">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="92a01-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="92a01-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="92a01-107">Properties</span></span>
|<span data-ttu-id="92a01-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92a01-108">Property</span></span>|<span data-ttu-id="92a01-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="92a01-109">Type</span></span>|<span data-ttu-id="92a01-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="92a01-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92a01-111">packageId</span><span class="sxs-lookup"><span data-stu-id="92a01-111">packageId</span></span>|<span data-ttu-id="92a01-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92a01-112">String</span></span>|<span data-ttu-id="92a01-113">O identificador de um app, como especificado na Play Store.</span><span class="sxs-lookup"><span data-stu-id="92a01-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92a01-114">Relações</span><span class="sxs-lookup"><span data-stu-id="92a01-114">Relationships</span></span>
<span data-ttu-id="92a01-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="92a01-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="92a01-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="92a01-116">JSON Representation</span></span>
<span data-ttu-id="92a01-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="92a01-117">Here is a JSON representation of the resource.</span></span>
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



