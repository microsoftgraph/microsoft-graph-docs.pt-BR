---
title: Tipo de recurso iosMobileAppIdentifier
description: O identificador de um aplicativo iOS.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb0eaade90c88cc553072f30dd36c42db4f44513
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465416"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="28a25-103">Tipo de recurso iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="28a25-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="28a25-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="28a25-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28a25-105">O identificador de um aplicativo iOS.</span><span class="sxs-lookup"><span data-stu-id="28a25-105">The identifier for an iOS app.</span></span>


<span data-ttu-id="28a25-106">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="28a25-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="28a25-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="28a25-107">Properties</span></span>
|<span data-ttu-id="28a25-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28a25-108">Property</span></span>|<span data-ttu-id="28a25-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="28a25-109">Type</span></span>|<span data-ttu-id="28a25-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="28a25-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28a25-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="28a25-111">bundleId</span></span>|<span data-ttu-id="28a25-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28a25-112">String</span></span>|<span data-ttu-id="28a25-113">O identificador de um aplicativo, conforme especificado na App Store.</span><span class="sxs-lookup"><span data-stu-id="28a25-113">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28a25-114">Relações</span><span class="sxs-lookup"><span data-stu-id="28a25-114">Relationships</span></span>
<span data-ttu-id="28a25-115">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="28a25-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28a25-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="28a25-116">JSON Representation</span></span>
<span data-ttu-id="28a25-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="28a25-117">Here is a JSON representation of the resource.</span></span>
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



