---
title: tipo de recurso officeUserCheckinSummary
description: Entidade que descreve as estatísticas de check-in do locatário.
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: 9ee53bbdbb02a3d5716f49941ec108e23a09ae88
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949266"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="b8731-103">tipo de recurso officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="b8731-103">officeUserCheckinSummary resource type</span></span>

> <span data-ttu-id="b8731-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b8731-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8731-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8731-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8731-106">Entidade que descreve as estatísticas de check-in do locatário.</span><span class="sxs-lookup"><span data-stu-id="b8731-106">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="b8731-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8731-107">Properties</span></span>
|<span data-ttu-id="b8731-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8731-108">Property</span></span>|<span data-ttu-id="b8731-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8731-109">Type</span></span>|<span data-ttu-id="b8731-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8731-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8731-111">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="b8731-111">succeededUserCount</span></span>|<span data-ttu-id="b8731-112">Int32</span><span class="sxs-lookup"><span data-stu-id="b8731-112">Int32</span></span>|<span data-ttu-id="b8731-113">Total de check-ins de verificação de usuários bem-sucedidos nos últimos três meses.</span><span class="sxs-lookup"><span data-stu-id="b8731-113">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="b8731-114">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="b8731-114">failedUserCount</span></span>|<span data-ttu-id="b8731-115">Int32</span><span class="sxs-lookup"><span data-stu-id="b8731-115">Int32</span></span>|<span data-ttu-id="b8731-116">Total de check-ins com falha do usuário nos últimos três meses.</span><span class="sxs-lookup"><span data-stu-id="b8731-116">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8731-117">Relações</span><span class="sxs-lookup"><span data-stu-id="b8731-117">Relationships</span></span>
<span data-ttu-id="b8731-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8731-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8731-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8731-119">JSON Representation</span></span>
<span data-ttu-id="b8731-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8731-120">Here is a JSON representation of the resource.</span></span>
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



