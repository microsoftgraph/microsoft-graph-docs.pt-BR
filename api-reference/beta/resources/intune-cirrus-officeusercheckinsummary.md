---
title: tipo de recurso officeUserCheckinSummary
description: Entidade que descreve as estatísticas de check-in do locatário.
localization_priority: Normal
author: davidmu1
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9ef202194c8817e500d27a96ae3dbf4e5e1a8359
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797294"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="6e662-103">tipo de recurso officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="6e662-103">officeUserCheckinSummary resource type</span></span>

> <span data-ttu-id="6e662-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6e662-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e662-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6e662-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e662-106">Entidade que descreve as estatísticas de check-in do locatário.</span><span class="sxs-lookup"><span data-stu-id="6e662-106">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="6e662-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e662-107">Properties</span></span>
|<span data-ttu-id="6e662-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e662-108">Property</span></span>|<span data-ttu-id="6e662-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e662-109">Type</span></span>|<span data-ttu-id="6e662-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e662-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e662-111">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="6e662-111">succeededUserCount</span></span>|<span data-ttu-id="6e662-112">Int32</span><span class="sxs-lookup"><span data-stu-id="6e662-112">Int32</span></span>|<span data-ttu-id="6e662-113">Total de check-ins de verificação de usuários bem-sucedidos nos últimos três meses.</span><span class="sxs-lookup"><span data-stu-id="6e662-113">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="6e662-114">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="6e662-114">failedUserCount</span></span>|<span data-ttu-id="6e662-115">Int32</span><span class="sxs-lookup"><span data-stu-id="6e662-115">Int32</span></span>|<span data-ttu-id="6e662-116">Total de check-ins com falha do usuário nos últimos três meses.</span><span class="sxs-lookup"><span data-stu-id="6e662-116">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e662-117">Relações</span><span class="sxs-lookup"><span data-stu-id="6e662-117">Relationships</span></span>
<span data-ttu-id="6e662-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e662-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e662-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e662-119">JSON Representation</span></span>
<span data-ttu-id="6e662-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e662-120">Here is a JSON representation of the resource.</span></span>
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



