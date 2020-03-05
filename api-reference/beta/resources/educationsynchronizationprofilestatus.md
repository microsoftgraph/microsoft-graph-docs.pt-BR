---
title: tipo de recurso educationSynchronizationProfileStatus
description: 'Representa o status de sincronização de um perfil de sincronização de dados da escola. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 88e2f85cc4b24bd55cdfc1fbc5aeecd7bee8c461
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500027"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="2ecfc-103">tipo de recurso educationSynchronizationProfileStatus</span><span class="sxs-lookup"><span data-stu-id="2ecfc-103">educationSynchronizationProfileStatus resource type</span></span>

<span data-ttu-id="2ecfc-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2ecfc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ecfc-105">Representa o status de sincronização de um [perfil de sincronização](educationsynchronizationprofile.md)de dados da escola.</span><span class="sxs-lookup"><span data-stu-id="2ecfc-105">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="2ecfc-106">**Observação:** As atualizações do **educationSynchronizationProfileStatus** podem ser atrasadas devido à natureza assíncrona do processamento de sincronização em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="2ecfc-106">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="2ecfc-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="2ecfc-107">Methods</span></span>

| <span data-ttu-id="2ecfc-108">Método</span><span class="sxs-lookup"><span data-stu-id="2ecfc-108">Method</span></span> | <span data-ttu-id="2ecfc-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2ecfc-109">Return Type</span></span> | <span data-ttu-id="2ecfc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ecfc-110">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="2ecfc-111">Obter o status de uma sincronização</span><span class="sxs-lookup"><span data-stu-id="2ecfc-111">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="2ecfc-112">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="2ecfc-112">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="2ecfc-113">Retornar o status de um perfil de sincronização específico.</span><span class="sxs-lookup"><span data-stu-id="2ecfc-113">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="2ecfc-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ecfc-114">Properties</span></span>

| <span data-ttu-id="2ecfc-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ecfc-115">Property</span></span> | <span data-ttu-id="2ecfc-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ecfc-116">Type</span></span> | <span data-ttu-id="2ecfc-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ecfc-117">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="2ecfc-118">**status**</span><span class="sxs-lookup"><span data-stu-id="2ecfc-118">**status**</span></span> | <span data-ttu-id="2ecfc-119">educationSynchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="2ecfc-119">educationSynchronizationStatus</span></span> | <span data-ttu-id="2ecfc-120">O status de uma sincronização. Os valores possíveis são `paused`: `inProgress`, `success`, `error`, `quarantined`, `validationError`,.</span><span class="sxs-lookup"><span data-stu-id="2ecfc-120">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="2ecfc-121">**lastSynchronizationDateTime**</span><span class="sxs-lookup"><span data-stu-id="2ecfc-121">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="2ecfc-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ecfc-122">DateTimeOffset</span></span> | <span data-ttu-id="2ecfc-123">Representa a hora em que as alterações mais recentes foram observadas no diretório.</span><span class="sxs-lookup"><span data-stu-id="2ecfc-123">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="2ecfc-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ecfc-124">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```
