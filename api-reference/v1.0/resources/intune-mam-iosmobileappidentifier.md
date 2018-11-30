---
title: Tipo de recurso iosMobileAppIdentifier
description: O identificador de um aplicativo iOS.
ms.openlocfilehash: dbf37da4f225a42b1686896e3fa1fafa472b4a67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006686"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="5eac4-103">Tipo de recurso iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="5eac4-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="5eac4-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5eac4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5eac4-105">O identificador de um aplicativo iOS.</span><span class="sxs-lookup"><span data-stu-id="5eac4-105">The identifier for an iOS app.</span></span>

<span data-ttu-id="5eac4-106">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="5eac4-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5eac4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5eac4-107">Properties</span></span>
|<span data-ttu-id="5eac4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5eac4-108">Property</span></span>|<span data-ttu-id="5eac4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5eac4-109">Type</span></span>|<span data-ttu-id="5eac4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5eac4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5eac4-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="5eac4-111">bundleId</span></span>|<span data-ttu-id="5eac4-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5eac4-112">String</span></span>|<span data-ttu-id="5eac4-113">O identificador de um aplicativo, conforme especificado na App Store.</span><span class="sxs-lookup"><span data-stu-id="5eac4-113">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5eac4-114">Relações</span><span class="sxs-lookup"><span data-stu-id="5eac4-114">Relationships</span></span>
<span data-ttu-id="5eac4-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5eac4-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5eac4-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5eac4-116">JSON Representation</span></span>
<span data-ttu-id="5eac4-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5eac4-117">Here is a JSON representation of the resource.</span></span>
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



