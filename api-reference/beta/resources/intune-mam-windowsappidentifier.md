---
title: Tipo de recurso windowsAppIdentifier
description: O identificador de um aplicativo do Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fd94a5cbd893c4f65dd726191f7a40198ca7750d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160100"
---
# <a name="windowsappidentifier-resource-type"></a><span data-ttu-id="6eff3-103">Tipo de recurso windowsAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="6eff3-103">windowsAppIdentifier resource type</span></span>

<span data-ttu-id="6eff3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6eff3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6eff3-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6eff3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6eff3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6eff3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6eff3-107">O identificador de um aplicativo do Windows.</span><span class="sxs-lookup"><span data-stu-id="6eff3-107">The identifier for a Windows app.</span></span>


<span data-ttu-id="6eff3-108">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="6eff3-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6eff3-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6eff3-109">Properties</span></span>
|<span data-ttu-id="6eff3-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6eff3-110">Property</span></span>|<span data-ttu-id="6eff3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="6eff3-111">Type</span></span>|<span data-ttu-id="6eff3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6eff3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6eff3-113">windowsAppId</span><span class="sxs-lookup"><span data-stu-id="6eff3-113">windowsAppId</span></span>|<span data-ttu-id="6eff3-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6eff3-114">String</span></span>|<span data-ttu-id="6eff3-115">O identificador de um aplicativo, conforme especificado na App Store.</span><span class="sxs-lookup"><span data-stu-id="6eff3-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6eff3-116">Relações</span><span class="sxs-lookup"><span data-stu-id="6eff3-116">Relationships</span></span>
<span data-ttu-id="6eff3-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6eff3-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6eff3-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6eff3-118">JSON Representation</span></span>
<span data-ttu-id="6eff3-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6eff3-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAppIdentifier",
  "windowsAppId": "String"
}
```




