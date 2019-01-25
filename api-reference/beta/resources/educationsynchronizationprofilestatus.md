---
title: tipo de recurso de educationSynchronizationProfileStatus
description: 'Representa o status da sincronização de um perfil de sincronização de dados escola. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 12908f6454cb27c673935f1e4c64c921b7ff0dcd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523537"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="ef5c0-103">tipo de recurso de educationSynchronizationProfileStatus</span><span class="sxs-lookup"><span data-stu-id="ef5c0-103">educationSynchronizationProfileStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef5c0-104">Representa o status da sincronização de um [perfil de sincronização](educationsynchronizationprofile.md)de dados do escola.</span><span class="sxs-lookup"><span data-stu-id="ef5c0-104">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="ef5c0-105">**Observação:** Atualizações para o **educationSynchronizationProfileStatus** podem ser atrasadas devido a natureza assíncrona do processamento de sincronização em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="ef5c0-105">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="ef5c0-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ef5c0-106">Methods</span></span>

| <span data-ttu-id="ef5c0-107">Método</span><span class="sxs-lookup"><span data-stu-id="ef5c0-107">Method</span></span> | <span data-ttu-id="ef5c0-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ef5c0-108">Return Type</span></span> | <span data-ttu-id="ef5c0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef5c0-109">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="ef5c0-110">Obter o status de uma sincronização</span><span class="sxs-lookup"><span data-stu-id="ef5c0-110">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="ef5c0-111">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="ef5c0-111">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="ef5c0-112">Retorna o status de um perfil de sincronização específico.</span><span class="sxs-lookup"><span data-stu-id="ef5c0-112">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="ef5c0-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ef5c0-113">Properties</span></span>

| <span data-ttu-id="ef5c0-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef5c0-114">Property</span></span> | <span data-ttu-id="ef5c0-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef5c0-115">Type</span></span> | <span data-ttu-id="ef5c0-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef5c0-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="ef5c0-117">**status**</span><span class="sxs-lookup"><span data-stu-id="ef5c0-117">**status**</span></span> | <span data-ttu-id="ef5c0-118">educationSynchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="ef5c0-118">educationSynchronizationStatus</span></span> | <span data-ttu-id="ef5c0-119">O status de uma sincronização. Os valores possíveis são: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span><span class="sxs-lookup"><span data-stu-id="ef5c0-119">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="ef5c0-120">**lastSynchronizationDateTime**</span><span class="sxs-lookup"><span data-stu-id="ef5c0-120">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="ef5c0-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef5c0-121">DateTimeOffset</span></span> | <span data-ttu-id="ef5c0-122">Representa a hora quando as alterações mais recentes têm foi observadas no diretório.</span><span class="sxs-lookup"><span data-stu-id="ef5c0-122">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="ef5c0-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ef5c0-123">JSON representation</span></span>
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
