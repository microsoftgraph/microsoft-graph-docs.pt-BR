---
title: Tipo de recurso androidMobileAppIdentifier
description: O identificador de um app Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 44bd4e889ccf7311b9d7b2807000167f9612d89a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49297984"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="9c5e0-103">Tipo de recurso androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9c5e0-103">androidMobileAppIdentifier resource type</span></span>

<span data-ttu-id="9c5e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c5e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c5e0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9c5e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c5e0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9c5e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c5e0-107">O identificador de um app Android.</span><span class="sxs-lookup"><span data-stu-id="9c5e0-107">The identifier for an Android app.</span></span>


<span data-ttu-id="9c5e0-108">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="9c5e0-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9c5e0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c5e0-109">Properties</span></span>
|<span data-ttu-id="9c5e0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c5e0-110">Property</span></span>|<span data-ttu-id="9c5e0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c5e0-111">Type</span></span>|<span data-ttu-id="9c5e0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c5e0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c5e0-113">packageId</span><span class="sxs-lookup"><span data-stu-id="9c5e0-113">packageId</span></span>|<span data-ttu-id="9c5e0-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c5e0-114">String</span></span>|<span data-ttu-id="9c5e0-115">O identificador de um app, como especificado na Play Store.</span><span class="sxs-lookup"><span data-stu-id="9c5e0-115">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c5e0-116">Relações</span><span class="sxs-lookup"><span data-stu-id="9c5e0-116">Relationships</span></span>
<span data-ttu-id="9c5e0-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c5e0-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c5e0-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c5e0-118">JSON Representation</span></span>
<span data-ttu-id="9c5e0-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c5e0-119">Here is a JSON representation of the resource.</span></span>
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




