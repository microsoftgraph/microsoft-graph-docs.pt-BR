---
title: tipo de recurso appleOwnerTypeEnrollmentType
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fb4cb2787389e632fef73132f701010d0353aa0c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783575"
---
# <a name="appleownertypeenrollmenttype-resource-type"></a><span data-ttu-id="fa5a6-103">tipo de recurso appleOwnerTypeEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="fa5a6-103">appleOwnerTypeEnrollmentType resource type</span></span>

> <span data-ttu-id="fa5a6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fa5a6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa5a6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fa5a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa5a6-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fa5a6-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="fa5a6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa5a6-107">Properties</span></span>
|<span data-ttu-id="fa5a6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa5a6-108">Property</span></span>|<span data-ttu-id="fa5a6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa5a6-109">Type</span></span>|<span data-ttu-id="fa5a6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa5a6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa5a6-111">ownerType</span><span class="sxs-lookup"><span data-stu-id="fa5a6-111">ownerType</span></span>|[<span data-ttu-id="fa5a6-112">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="fa5a6-112">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="fa5a6-113">O tipo de proprietário.</span><span class="sxs-lookup"><span data-stu-id="fa5a6-113">The owner type.</span></span> <span data-ttu-id="fa5a6-114">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="fa5a6-114">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="fa5a6-115">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="fa5a6-115">enrollmentType</span></span>|[<span data-ttu-id="fa5a6-116">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="fa5a6-116">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="fa5a6-117">O tipo de registro.</span><span class="sxs-lookup"><span data-stu-id="fa5a6-117">The enrollment type.</span></span> <span data-ttu-id="fa5a6-118">Os valores possíveis são: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="fa5a6-118">Possible values are: `unknown`, `device`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa5a6-119">Relações</span><span class="sxs-lookup"><span data-stu-id="fa5a6-119">Relationships</span></span>
<span data-ttu-id="fa5a6-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fa5a6-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa5a6-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa5a6-121">JSON Representation</span></span>
<span data-ttu-id="fa5a6-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fa5a6-122">Here is a JSON representation of the resource.</span></span>
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



