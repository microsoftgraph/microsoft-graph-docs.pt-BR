---
title: Tipo de recurso iosMobileAppIdentifier
description: O identificador de um aplicativo iOS.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5e9305963654356c56bff31f6ffb9f97129f4980
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922785"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="0ea92-103">Tipo de recurso iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="0ea92-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="0ea92-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0ea92-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ea92-105">O identificador de um aplicativo iOS.</span><span class="sxs-lookup"><span data-stu-id="0ea92-105">The identifier for an iOS app.</span></span>

<span data-ttu-id="0ea92-106">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="0ea92-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0ea92-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ea92-107">Properties</span></span>
|<span data-ttu-id="0ea92-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ea92-108">Property</span></span>|<span data-ttu-id="0ea92-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ea92-109">Type</span></span>|<span data-ttu-id="0ea92-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ea92-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ea92-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="0ea92-111">bundleId</span></span>|<span data-ttu-id="0ea92-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ea92-112">String</span></span>|<span data-ttu-id="0ea92-113">O identificador de um aplicativo, conforme especificado na App Store.</span><span class="sxs-lookup"><span data-stu-id="0ea92-113">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ea92-114">Relações</span><span class="sxs-lookup"><span data-stu-id="0ea92-114">Relationships</span></span>
<span data-ttu-id="0ea92-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0ea92-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0ea92-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ea92-116">JSON Representation</span></span>
<span data-ttu-id="0ea92-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ea92-117">Here is a JSON representation of the resource.</span></span>
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



