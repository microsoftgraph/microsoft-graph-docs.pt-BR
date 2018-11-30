---
title: tipo de recurso de office365GroupsActivityStorage
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 23ff4d112373f52c4c19d6631ac89bac22399b29
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039922"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="df46a-103">tipo de recurso de office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="df46a-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="df46a-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df46a-104">Properties</span></span>

| <span data-ttu-id="df46a-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df46a-105">Property</span></span>                  | <span data-ttu-id="df46a-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="df46a-106">Type</span></span>   | <span data-ttu-id="df46a-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="df46a-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="df46a-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="df46a-108">reportRefreshDate</span></span>         | <span data-ttu-id="df46a-109">Data</span><span class="sxs-lookup"><span data-stu-id="df46a-109">Date</span></span>   | <span data-ttu-id="df46a-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="df46a-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="df46a-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="df46a-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="df46a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="df46a-112">Int64</span></span>  | <span data-ttu-id="df46a-113">O armazenamento utilizado na caixa de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="df46a-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="df46a-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="df46a-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="df46a-115">Int64</span><span class="sxs-lookup"><span data-stu-id="df46a-115">Int64</span></span>  | <span data-ttu-id="df46a-116">O armazenamento usado na biblioteca de documentos do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="df46a-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="df46a-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="df46a-117">reportDate</span></span>                | <span data-ttu-id="df46a-118">Data</span><span class="sxs-lookup"><span data-stu-id="df46a-118">Date</span></span>   | <span data-ttu-id="df46a-119">A data de instantâneo do Exchange e SharePoint usou o armazenamento.</span><span class="sxs-lookup"><span data-stu-id="df46a-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="df46a-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="df46a-120">reportPeriod</span></span>              | <span data-ttu-id="df46a-121">String</span><span class="sxs-lookup"><span data-stu-id="df46a-121">String</span></span> | <span data-ttu-id="df46a-122">O número de dias que abrange o relatório.</span><span class="sxs-lookup"><span data-stu-id="df46a-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="df46a-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df46a-123">JSON representation</span></span>

<span data-ttu-id="df46a-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df46a-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailboxStorageUsedInBytes": 1024, 
  "siteStorageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
