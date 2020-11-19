---
title: tipo de recurso officeUserCheckinSummary
description: Entidade que descreve as estatísticas de check-in do locatário.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ed81c3c152b0d81cfcdf15388fdc4db3a7612052
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294974"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="b2320-103">tipo de recurso officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="b2320-103">officeUserCheckinSummary resource type</span></span>

<span data-ttu-id="b2320-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2320-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2320-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b2320-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2320-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2320-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2320-107">Entidade que descreve as estatísticas de check-in do locatário.</span><span class="sxs-lookup"><span data-stu-id="b2320-107">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="b2320-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2320-108">Properties</span></span>
|<span data-ttu-id="b2320-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2320-109">Property</span></span>|<span data-ttu-id="b2320-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2320-110">Type</span></span>|<span data-ttu-id="b2320-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2320-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2320-112">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="b2320-112">succeededUserCount</span></span>|<span data-ttu-id="b2320-113">Int32</span><span class="sxs-lookup"><span data-stu-id="b2320-113">Int32</span></span>|<span data-ttu-id="b2320-114">Total de check-ins de verificação de usuários bem-sucedidos nos últimos três meses.</span><span class="sxs-lookup"><span data-stu-id="b2320-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="b2320-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="b2320-115">failedUserCount</span></span>|<span data-ttu-id="b2320-116">Int32</span><span class="sxs-lookup"><span data-stu-id="b2320-116">Int32</span></span>|<span data-ttu-id="b2320-117">Total de check-ins com falha do usuário nos últimos três meses.</span><span class="sxs-lookup"><span data-stu-id="b2320-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2320-118">Relações</span><span class="sxs-lookup"><span data-stu-id="b2320-118">Relationships</span></span>
<span data-ttu-id="b2320-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2320-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2320-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2320-120">JSON Representation</span></span>
<span data-ttu-id="b2320-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b2320-121">Here is a JSON representation of the resource.</span></span>
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




