---
title: Tipo de recurso onenoteOperation
description: O status de determinadas operações demoradas do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 9fb490d38b975291b8f3b710f5e2f702f0fee7df
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962258"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="65508-103">Tipo de recurso onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="65508-103">onenoteOperation resource type</span></span>

> <span data-ttu-id="65508-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="65508-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65508-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="65508-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65508-106">O status de determinadas operações demoradas do OneNote.</span><span class="sxs-lookup"><span data-stu-id="65508-106">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="65508-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65508-107">JSON representation</span></span>

<span data-ttu-id="65508-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65508-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="65508-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65508-109">Properties</span></span>
| <span data-ttu-id="65508-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65508-110">Property</span></span>     | <span data-ttu-id="65508-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="65508-111">Type</span></span>   |<span data-ttu-id="65508-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="65508-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65508-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65508-113">createdDateTime</span></span>| <span data-ttu-id="65508-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65508-114">DateTimeOffset</span></span> |<span data-ttu-id="65508-115">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="65508-115">The start time of the operation.</span></span>|
|<span data-ttu-id="65508-116">erro</span><span class="sxs-lookup"><span data-stu-id="65508-116">error</span></span>|[<span data-ttu-id="65508-117">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="65508-117">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="65508-118">O erro retornado pela operação.</span><span class="sxs-lookup"><span data-stu-id="65508-118">The error returned by the operation.</span></span>|
|<span data-ttu-id="65508-119">id</span><span class="sxs-lookup"><span data-stu-id="65508-119">id</span></span>|<span data-ttu-id="65508-120">string</span><span class="sxs-lookup"><span data-stu-id="65508-120">string</span></span>|<span data-ttu-id="65508-121">A id da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="65508-121">The operation id. Read-only.</span></span>|
|<span data-ttu-id="65508-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="65508-122">lastActionDateTime</span></span>| <span data-ttu-id="65508-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65508-123">DateTimeOffset</span></span> |<span data-ttu-id="65508-124">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="65508-124">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="65508-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="65508-125">resourceId</span></span>|<span data-ttu-id="65508-126">string</span><span class="sxs-lookup"><span data-stu-id="65508-126">string</span></span>|<span data-ttu-id="65508-127">A id do recurso.</span><span class="sxs-lookup"><span data-stu-id="65508-127">The resource id.</span></span>|
|<span data-ttu-id="65508-128">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="65508-128">resourceLocation</span></span>|<span data-ttu-id="65508-129">string</span><span class="sxs-lookup"><span data-stu-id="65508-129">string</span></span>|<span data-ttu-id="65508-p102">O URI de recurso do objeto. Por exemplo, o URI de recurso para uma seção ou página copiada.</span><span class="sxs-lookup"><span data-stu-id="65508-p102">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="65508-132">status</span><span class="sxs-lookup"><span data-stu-id="65508-132">status</span></span>|<span data-ttu-id="65508-133">string</span><span class="sxs-lookup"><span data-stu-id="65508-133">string</span></span>|<span data-ttu-id="65508-134">O status atual da operação: `notstarted`, `running`, `completed`, `failed`</span><span class="sxs-lookup"><span data-stu-id="65508-134">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="65508-135">percentComplete</span><span class="sxs-lookup"><span data-stu-id="65508-135">percentComplete</span></span>|<span data-ttu-id="65508-136">string</span><span class="sxs-lookup"><span data-stu-id="65508-136">string</span></span>|<span data-ttu-id="65508-137">A porcentagem concluída da operação se a operação ainda estiver com um status `running`</span><span class="sxs-lookup"><span data-stu-id="65508-137">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="65508-138">Relações</span><span class="sxs-lookup"><span data-stu-id="65508-138">Relationships</span></span>
<span data-ttu-id="65508-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="65508-139">None</span></span>


## <a name="methods"></a><span data-ttu-id="65508-140">Métodos</span><span class="sxs-lookup"><span data-stu-id="65508-140">Methods</span></span>

| <span data-ttu-id="65508-141">Método</span><span class="sxs-lookup"><span data-stu-id="65508-141">Method</span></span>           | <span data-ttu-id="65508-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="65508-142">Return Type</span></span>    |<span data-ttu-id="65508-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="65508-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="65508-144">Get operation</span><span class="sxs-lookup"><span data-stu-id="65508-144">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="65508-145">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="65508-145">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="65508-146">Obter o status atual da operação.</span><span class="sxs-lookup"><span data-stu-id="65508-146">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
