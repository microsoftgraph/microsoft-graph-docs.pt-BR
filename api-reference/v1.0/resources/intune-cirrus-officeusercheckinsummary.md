---
title: Tipo de recurso officeUserCheckinSummary
description: Entidade que descreve as estatísticas de check-in do locatário.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ed81c3c152b0d81cfcdf15388fdc4db3a7612052
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759442"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="ef90b-103">Tipo de recurso officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="ef90b-103">officeUserCheckinSummary resource type</span></span>

<span data-ttu-id="ef90b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef90b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef90b-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ef90b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef90b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ef90b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef90b-107">Entidade que descreve as estatísticas de check-in do locatário.</span><span class="sxs-lookup"><span data-stu-id="ef90b-107">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="ef90b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ef90b-108">Properties</span></span>
|<span data-ttu-id="ef90b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef90b-109">Property</span></span>|<span data-ttu-id="ef90b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef90b-110">Type</span></span>|<span data-ttu-id="ef90b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef90b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef90b-112">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="ef90b-112">succeededUserCount</span></span>|<span data-ttu-id="ef90b-113">Int32</span><span class="sxs-lookup"><span data-stu-id="ef90b-113">Int32</span></span>|<span data-ttu-id="ef90b-114">Total de check-ins bem-sucedidos do usuário nos últimos três meses.</span><span class="sxs-lookup"><span data-stu-id="ef90b-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="ef90b-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="ef90b-115">failedUserCount</span></span>|<span data-ttu-id="ef90b-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ef90b-116">Int32</span></span>|<span data-ttu-id="ef90b-117">Total de check-ins de usuário com falha nos últimos 3 meses.</span><span class="sxs-lookup"><span data-stu-id="ef90b-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef90b-118">Relações</span><span class="sxs-lookup"><span data-stu-id="ef90b-118">Relationships</span></span>
<span data-ttu-id="ef90b-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ef90b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef90b-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ef90b-120">JSON Representation</span></span>
<span data-ttu-id="ef90b-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ef90b-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeUserCheckinSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeUserCheckinSummary",
  "succeededUserCount": 1024,
  "failedUserCount": 1024
}
```




