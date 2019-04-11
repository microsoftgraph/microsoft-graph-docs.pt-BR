---
title: Tipo de recurso androidMobileAppIdentifier
description: O identificador de um app Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8106475817a333838a9f7e6a591f15ddd2ce111d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805730"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="d7aa5-103">Tipo de recurso androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d7aa5-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="d7aa5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d7aa5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7aa5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d7aa5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7aa5-106">O identificador de um app Android.</span><span class="sxs-lookup"><span data-stu-id="d7aa5-106">The identifier for an Android app.</span></span>


<span data-ttu-id="d7aa5-107">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="d7aa5-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d7aa5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d7aa5-108">Properties</span></span>
|<span data-ttu-id="d7aa5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7aa5-109">Property</span></span>|<span data-ttu-id="d7aa5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7aa5-110">Type</span></span>|<span data-ttu-id="d7aa5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7aa5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7aa5-112">packageId</span><span class="sxs-lookup"><span data-stu-id="d7aa5-112">packageId</span></span>|<span data-ttu-id="d7aa5-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7aa5-113">String</span></span>|<span data-ttu-id="d7aa5-114">O identificador de um app, como especificado na Play Store.</span><span class="sxs-lookup"><span data-stu-id="d7aa5-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7aa5-115">Relações</span><span class="sxs-lookup"><span data-stu-id="d7aa5-115">Relationships</span></span>
<span data-ttu-id="d7aa5-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d7aa5-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7aa5-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d7aa5-117">JSON Representation</span></span>
<span data-ttu-id="d7aa5-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d7aa5-118">Here is a JSON representation of the resource.</span></span>
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





