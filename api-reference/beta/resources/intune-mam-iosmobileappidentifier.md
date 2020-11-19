---
title: Tipo de recurso iosMobileAppIdentifier
description: O identificador de um aplicativo iOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fabff3ec78d64f87eb68b961557bff3752d1339d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49297816"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="1091b-103">Tipo de recurso iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="1091b-103">iosMobileAppIdentifier resource type</span></span>

<span data-ttu-id="1091b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1091b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1091b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1091b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1091b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1091b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1091b-107">O identificador de um aplicativo iOS.</span><span class="sxs-lookup"><span data-stu-id="1091b-107">The identifier for an iOS app.</span></span>


<span data-ttu-id="1091b-108">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="1091b-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1091b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1091b-109">Properties</span></span>
|<span data-ttu-id="1091b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1091b-110">Property</span></span>|<span data-ttu-id="1091b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1091b-111">Type</span></span>|<span data-ttu-id="1091b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1091b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1091b-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="1091b-113">bundleId</span></span>|<span data-ttu-id="1091b-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1091b-114">String</span></span>|<span data-ttu-id="1091b-115">O identificador de um aplicativo, conforme especificado na App Store.</span><span class="sxs-lookup"><span data-stu-id="1091b-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1091b-116">Relações</span><span class="sxs-lookup"><span data-stu-id="1091b-116">Relationships</span></span>
<span data-ttu-id="1091b-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1091b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1091b-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1091b-118">JSON Representation</span></span>
<span data-ttu-id="1091b-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1091b-119">Here is a JSON representation of the resource.</span></span>
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




