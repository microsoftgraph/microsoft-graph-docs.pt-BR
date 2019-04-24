---
title: tipo de recurso educationSynchronizationProfileStatus
description: 'Representa o status de sincronização de um perfil de sincronização de dados da escola. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 12908f6454cb27c673935f1e4c64c921b7ff0dcd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507088"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="2eff1-103">tipo de recurso educationSynchronizationProfileStatus</span><span class="sxs-lookup"><span data-stu-id="2eff1-103">educationSynchronizationProfileStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2eff1-104">Representa o status de sincronização de um [perfil de sincronização](educationsynchronizationprofile.md)de dados da escola.</span><span class="sxs-lookup"><span data-stu-id="2eff1-104">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="2eff1-105">**Observação:** As atualizações do **educationSynchronizationProfileStatus** podem ser atrasadas devido à natureza assíncrona do processamento de sincronização em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="2eff1-105">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="2eff1-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="2eff1-106">Methods</span></span>

| <span data-ttu-id="2eff1-107">Método</span><span class="sxs-lookup"><span data-stu-id="2eff1-107">Method</span></span> | <span data-ttu-id="2eff1-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2eff1-108">Return Type</span></span> | <span data-ttu-id="2eff1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2eff1-109">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="2eff1-110">Obter o status de uma sincronização</span><span class="sxs-lookup"><span data-stu-id="2eff1-110">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="2eff1-111">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="2eff1-111">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="2eff1-112">Retornar o status de um perfil de sincronização específico.</span><span class="sxs-lookup"><span data-stu-id="2eff1-112">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="2eff1-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2eff1-113">Properties</span></span>

| <span data-ttu-id="2eff1-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2eff1-114">Property</span></span> | <span data-ttu-id="2eff1-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="2eff1-115">Type</span></span> | <span data-ttu-id="2eff1-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="2eff1-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="2eff1-117">**status**</span><span class="sxs-lookup"><span data-stu-id="2eff1-117">**status**</span></span> | <span data-ttu-id="2eff1-118">educationSynchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="2eff1-118">educationSynchronizationStatus</span></span> | <span data-ttu-id="2eff1-119">O status de uma sincronização. Os valores possíveis são `paused`: `inProgress`, `success`, `error`, `quarantined`, `validationError`,.</span><span class="sxs-lookup"><span data-stu-id="2eff1-119">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="2eff1-120">**lastSynchronizationDateTime**</span><span class="sxs-lookup"><span data-stu-id="2eff1-120">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="2eff1-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2eff1-121">DateTimeOffset</span></span> | <span data-ttu-id="2eff1-122">Representa a hora em que as alterações mais recentes foram observadas no diretório.</span><span class="sxs-lookup"><span data-stu-id="2eff1-122">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="2eff1-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2eff1-123">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationprofilestatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
