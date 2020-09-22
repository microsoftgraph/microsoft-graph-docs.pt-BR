---
title: Tipo de recurso iosMobileAppIdentifier
description: O identificador de um aplicativo iOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b106811c802571edfd4da28134ea99883869c129
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030462"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="379b9-103">Tipo de recurso iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="379b9-103">iosMobileAppIdentifier resource type</span></span>

<span data-ttu-id="379b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="379b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="379b9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="379b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="379b9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="379b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="379b9-107">O identificador de um aplicativo iOS.</span><span class="sxs-lookup"><span data-stu-id="379b9-107">The identifier for an iOS app.</span></span>


<span data-ttu-id="379b9-108">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="379b9-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="379b9-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="379b9-109">Properties</span></span>
|<span data-ttu-id="379b9-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="379b9-110">Property</span></span>|<span data-ttu-id="379b9-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="379b9-111">Type</span></span>|<span data-ttu-id="379b9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="379b9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="379b9-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="379b9-113">bundleId</span></span>|<span data-ttu-id="379b9-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="379b9-114">String</span></span>|<span data-ttu-id="379b9-115">O identificador de um aplicativo, conforme especificado na App Store.</span><span class="sxs-lookup"><span data-stu-id="379b9-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="379b9-116">Relações</span><span class="sxs-lookup"><span data-stu-id="379b9-116">Relationships</span></span>
<span data-ttu-id="379b9-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="379b9-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="379b9-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="379b9-118">JSON Representation</span></span>
<span data-ttu-id="379b9-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="379b9-119">Here is a JSON representation of the resource.</span></span>
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






