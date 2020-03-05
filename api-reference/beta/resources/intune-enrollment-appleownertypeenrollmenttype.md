---
title: tipo de recurso appleOwnerTypeEnrollmentType
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 03b8457573a88ade90bdf09289715727ffc9d6b7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528356"
---
# <a name="appleownertypeenrollmenttype-resource-type"></a><span data-ttu-id="a540b-103">tipo de recurso appleOwnerTypeEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a540b-103">appleOwnerTypeEnrollmentType resource type</span></span>

<span data-ttu-id="a540b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a540b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a540b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a540b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a540b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a540b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a540b-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a540b-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a540b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a540b-108">Properties</span></span>
|<span data-ttu-id="a540b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a540b-109">Property</span></span>|<span data-ttu-id="a540b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a540b-110">Type</span></span>|<span data-ttu-id="a540b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a540b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a540b-112">ownerType</span><span class="sxs-lookup"><span data-stu-id="a540b-112">ownerType</span></span>|[<span data-ttu-id="a540b-113">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="a540b-113">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="a540b-114">O tipo de proprietário.</span><span class="sxs-lookup"><span data-stu-id="a540b-114">The owner type.</span></span> <span data-ttu-id="a540b-115">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="a540b-115">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="a540b-116">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="a540b-116">enrollmentType</span></span>|[<span data-ttu-id="a540b-117">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a540b-117">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="a540b-118">O tipo de registro.</span><span class="sxs-lookup"><span data-stu-id="a540b-118">The enrollment type.</span></span> <span data-ttu-id="a540b-119">Os valores possíveis são: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="a540b-119">Possible values are: `unknown`, `device`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a540b-120">Relações</span><span class="sxs-lookup"><span data-stu-id="a540b-120">Relationships</span></span>
<span data-ttu-id="a540b-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a540b-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a540b-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a540b-122">JSON Representation</span></span>
<span data-ttu-id="a540b-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a540b-123">Here is a JSON representation of the resource.</span></span>
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



