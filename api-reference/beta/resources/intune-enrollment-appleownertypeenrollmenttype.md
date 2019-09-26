---
title: tipo de recurso appleOwnerTypeEnrollmentType
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 42ca89d265c65b49239e8272e0bd91f0666dc08a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199665"
---
# <a name="appleownertypeenrollmenttype-resource-type"></a><span data-ttu-id="230bb-103">tipo de recurso appleOwnerTypeEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="230bb-103">appleOwnerTypeEnrollmentType resource type</span></span>

> <span data-ttu-id="230bb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="230bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="230bb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="230bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="230bb-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="230bb-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="230bb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="230bb-107">Properties</span></span>
|<span data-ttu-id="230bb-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="230bb-108">Property</span></span>|<span data-ttu-id="230bb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="230bb-109">Type</span></span>|<span data-ttu-id="230bb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="230bb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="230bb-111">ownerType</span><span class="sxs-lookup"><span data-stu-id="230bb-111">ownerType</span></span>|[<span data-ttu-id="230bb-112">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="230bb-112">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="230bb-113">O tipo de proprietário.</span><span class="sxs-lookup"><span data-stu-id="230bb-113">The owner type.</span></span> <span data-ttu-id="230bb-114">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="230bb-114">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="230bb-115">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="230bb-115">enrollmentType</span></span>|[<span data-ttu-id="230bb-116">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="230bb-116">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="230bb-117">O tipo de registro.</span><span class="sxs-lookup"><span data-stu-id="230bb-117">The enrollment type.</span></span> <span data-ttu-id="230bb-118">Os valores possíveis são: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="230bb-118">Possible values are: `unknown`, `device`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="230bb-119">Relações</span><span class="sxs-lookup"><span data-stu-id="230bb-119">Relationships</span></span>
<span data-ttu-id="230bb-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="230bb-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="230bb-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="230bb-121">JSON Representation</span></span>
<span data-ttu-id="230bb-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="230bb-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleOwnerTypeEnrollmentType",
  "ownerType": "String",
  "enrollmentType": "String"
}
```



