---
title: Tipo de recurso onenoteOperation
description: O status de determinadas operações demoradas do OneNote.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 7632186c3e44afbfe0d6cbf3d079ad0758514b38
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860260"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="f20b5-103">Tipo de recurso onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="f20b5-103">onenoteOperation resource type</span></span>

> <span data-ttu-id="f20b5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f20b5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f20b5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f20b5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f20b5-106">O status de determinadas operações demoradas do OneNote.</span><span class="sxs-lookup"><span data-stu-id="f20b5-106">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f20b5-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f20b5-107">JSON representation</span></span>

<span data-ttu-id="f20b5-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f20b5-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "error": {"@odata.type": "microsoft.graph.onenoteOperationError"},
  "id": "string (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resourceId": "string",
  "resourceLocation": "string",
  "status": "string",
  "percentComplete": "string"
}

```
## <a name="properties"></a><span data-ttu-id="f20b5-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f20b5-109">Properties</span></span>
| <span data-ttu-id="f20b5-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f20b5-110">Property</span></span>     | <span data-ttu-id="f20b5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f20b5-111">Type</span></span>   |<span data-ttu-id="f20b5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f20b5-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f20b5-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f20b5-113">createdDateTime</span></span>| <span data-ttu-id="f20b5-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f20b5-114">DateTimeOffset</span></span> |<span data-ttu-id="f20b5-115">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="f20b5-115">The start time of the operation.</span></span>|
|<span data-ttu-id="f20b5-116">erro</span><span class="sxs-lookup"><span data-stu-id="f20b5-116">error</span></span>|[<span data-ttu-id="f20b5-117">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="f20b5-117">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="f20b5-118">O erro retornado pela operação.</span><span class="sxs-lookup"><span data-stu-id="f20b5-118">The error returned by the operation.</span></span>|
|<span data-ttu-id="f20b5-119">id</span><span class="sxs-lookup"><span data-stu-id="f20b5-119">id</span></span>|<span data-ttu-id="f20b5-120">string</span><span class="sxs-lookup"><span data-stu-id="f20b5-120">string</span></span>|<span data-ttu-id="f20b5-121">A id da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f20b5-121">The operation id. Read-only.</span></span>|
|<span data-ttu-id="f20b5-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="f20b5-122">lastActionDateTime</span></span>| <span data-ttu-id="f20b5-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f20b5-123">DateTimeOffset</span></span> |<span data-ttu-id="f20b5-124">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="f20b5-124">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="f20b5-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="f20b5-125">resourceId</span></span>|<span data-ttu-id="f20b5-126">string</span><span class="sxs-lookup"><span data-stu-id="f20b5-126">string</span></span>|<span data-ttu-id="f20b5-127">A id do recurso.</span><span class="sxs-lookup"><span data-stu-id="f20b5-127">The resource id.</span></span>|
|<span data-ttu-id="f20b5-128">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="f20b5-128">resourceLocation</span></span>|<span data-ttu-id="f20b5-129">string</span><span class="sxs-lookup"><span data-stu-id="f20b5-129">string</span></span>|<span data-ttu-id="f20b5-p102">O URI de recurso do objeto. Por exemplo, o URI de recurso para uma seção ou página copiada.</span><span class="sxs-lookup"><span data-stu-id="f20b5-p102">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="f20b5-132">status</span><span class="sxs-lookup"><span data-stu-id="f20b5-132">status</span></span>|<span data-ttu-id="f20b5-133">string</span><span class="sxs-lookup"><span data-stu-id="f20b5-133">string</span></span>|<span data-ttu-id="f20b5-134">O status atual da operação: `notstarted`, `running`, `completed`, `failed`</span><span class="sxs-lookup"><span data-stu-id="f20b5-134">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="f20b5-135">percentComplete</span><span class="sxs-lookup"><span data-stu-id="f20b5-135">percentComplete</span></span>|<span data-ttu-id="f20b5-136">string</span><span class="sxs-lookup"><span data-stu-id="f20b5-136">string</span></span>|<span data-ttu-id="f20b5-137">A porcentagem concluída da operação se a operação ainda estiver com um status `running`</span><span class="sxs-lookup"><span data-stu-id="f20b5-137">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="f20b5-138">Relações</span><span class="sxs-lookup"><span data-stu-id="f20b5-138">Relationships</span></span>
<span data-ttu-id="f20b5-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f20b5-139">None</span></span>


## <a name="methods"></a><span data-ttu-id="f20b5-140">Métodos</span><span class="sxs-lookup"><span data-stu-id="f20b5-140">Methods</span></span>

| <span data-ttu-id="f20b5-141">Método</span><span class="sxs-lookup"><span data-stu-id="f20b5-141">Method</span></span>           | <span data-ttu-id="f20b5-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f20b5-142">Return Type</span></span>    |<span data-ttu-id="f20b5-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="f20b5-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f20b5-144">Get operation</span><span class="sxs-lookup"><span data-stu-id="f20b5-144">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="f20b5-145">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="f20b5-145">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="f20b5-146">Obter o status atual da operação.</span><span class="sxs-lookup"><span data-stu-id="f20b5-146">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
