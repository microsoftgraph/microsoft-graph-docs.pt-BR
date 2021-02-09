---
title: Tipo de recurso macAppIdentifier
description: O identificador de um aplicativo do Mac.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b4ee44dc2fe288d7a1605660ef95dc7d88f600fb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160176"
---
# <a name="macappidentifier-resource-type"></a><span data-ttu-id="3ffc5-103">Tipo de recurso macAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="3ffc5-103">macAppIdentifier resource type</span></span>

<span data-ttu-id="3ffc5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ffc5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ffc5-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3ffc5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ffc5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3ffc5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ffc5-107">O identificador de um aplicativo do Mac.</span><span class="sxs-lookup"><span data-stu-id="3ffc5-107">The identifier for a Mac app.</span></span>


<span data-ttu-id="3ffc5-108">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="3ffc5-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3ffc5-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ffc5-109">Properties</span></span>
|<span data-ttu-id="3ffc5-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ffc5-110">Property</span></span>|<span data-ttu-id="3ffc5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ffc5-111">Type</span></span>|<span data-ttu-id="3ffc5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ffc5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ffc5-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="3ffc5-113">bundleId</span></span>|<span data-ttu-id="3ffc5-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ffc5-114">String</span></span>|<span data-ttu-id="3ffc5-115">O identificador de um aplicativo, conforme especificado na App Store.</span><span class="sxs-lookup"><span data-stu-id="3ffc5-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ffc5-116">Relações</span><span class="sxs-lookup"><span data-stu-id="3ffc5-116">Relationships</span></span>
<span data-ttu-id="3ffc5-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3ffc5-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ffc5-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ffc5-118">JSON Representation</span></span>
<span data-ttu-id="3ffc5-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3ffc5-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macAppIdentifier",
  "bundleId": "String"
}
```




