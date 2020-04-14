---
title: tipo de recurso officeUserCheckinSummary
description: Entidade que descreve as estatísticas de check-in do locatário.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8564f7d0d2fb06218b141b7e9369f2096bdec982
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462516"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="689d0-103">tipo de recurso officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="689d0-103">officeUserCheckinSummary resource type</span></span>

<span data-ttu-id="689d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="689d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="689d0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="689d0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="689d0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="689d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="689d0-107">Entidade que descreve as estatísticas de check-in do locatário.</span><span class="sxs-lookup"><span data-stu-id="689d0-107">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="689d0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="689d0-108">Properties</span></span>
|<span data-ttu-id="689d0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="689d0-109">Property</span></span>|<span data-ttu-id="689d0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="689d0-110">Type</span></span>|<span data-ttu-id="689d0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="689d0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="689d0-112">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="689d0-112">succeededUserCount</span></span>|<span data-ttu-id="689d0-113">Int32</span><span class="sxs-lookup"><span data-stu-id="689d0-113">Int32</span></span>|<span data-ttu-id="689d0-114">Total de check-ins de verificação de usuários bem-sucedidos nos últimos três meses.</span><span class="sxs-lookup"><span data-stu-id="689d0-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="689d0-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="689d0-115">failedUserCount</span></span>|<span data-ttu-id="689d0-116">Int32</span><span class="sxs-lookup"><span data-stu-id="689d0-116">Int32</span></span>|<span data-ttu-id="689d0-117">Total de check-ins com falha do usuário nos últimos três meses.</span><span class="sxs-lookup"><span data-stu-id="689d0-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="689d0-118">Relações</span><span class="sxs-lookup"><span data-stu-id="689d0-118">Relationships</span></span>
<span data-ttu-id="689d0-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="689d0-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="689d0-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="689d0-120">JSON Representation</span></span>
<span data-ttu-id="689d0-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="689d0-121">Here is a JSON representation of the resource.</span></span>
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



