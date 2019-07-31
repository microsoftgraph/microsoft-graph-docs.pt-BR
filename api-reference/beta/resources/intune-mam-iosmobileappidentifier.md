---
title: Tipo de recurso iosMobileAppIdentifier
description: O identificador de um aplicativo iOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 690703b5355a20a609363cc7c0ffd7a4574b903f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010879"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="c5851-103">Tipo de recurso iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c5851-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="c5851-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c5851-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5851-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c5851-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5851-106">O identificador de um aplicativo iOS.</span><span class="sxs-lookup"><span data-stu-id="c5851-106">The identifier for an iOS app.</span></span>


<span data-ttu-id="c5851-107">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="c5851-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c5851-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5851-108">Properties</span></span>
|<span data-ttu-id="c5851-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5851-109">Property</span></span>|<span data-ttu-id="c5851-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5851-110">Type</span></span>|<span data-ttu-id="c5851-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5851-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5851-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="c5851-112">bundleId</span></span>|<span data-ttu-id="c5851-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5851-113">String</span></span>|<span data-ttu-id="c5851-114">O identificador de um aplicativo, conforme especificado na App Store.</span><span class="sxs-lookup"><span data-stu-id="c5851-114">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5851-115">Relações</span><span class="sxs-lookup"><span data-stu-id="c5851-115">Relationships</span></span>
<span data-ttu-id="c5851-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c5851-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5851-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5851-117">JSON Representation</span></span>
<span data-ttu-id="c5851-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c5851-118">Here is a JSON representation of the resource.</span></span>
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





