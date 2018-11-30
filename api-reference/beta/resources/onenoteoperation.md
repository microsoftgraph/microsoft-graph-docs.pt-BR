---
title: Tipo de recurso onenoteOperation
description: O status de determinadas operações demoradas do OneNote.
ms.openlocfilehash: af7da970a148d4b70385487503e3abf6431c430a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034223"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="73aa4-103">Tipo de recurso onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="73aa4-103">onenoteOperation resource type</span></span>

> <span data-ttu-id="73aa4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="73aa4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73aa4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="73aa4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="73aa4-106">O status de determinadas operações demoradas do OneNote.</span><span class="sxs-lookup"><span data-stu-id="73aa4-106">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="73aa4-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73aa4-107">JSON representation</span></span>

<span data-ttu-id="73aa4-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="73aa4-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="73aa4-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73aa4-109">Properties</span></span>
| <span data-ttu-id="73aa4-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73aa4-110">Property</span></span>     | <span data-ttu-id="73aa4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="73aa4-111">Type</span></span>   |<span data-ttu-id="73aa4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="73aa4-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73aa4-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73aa4-113">createdDateTime</span></span>| <span data-ttu-id="73aa4-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73aa4-114">DateTimeOffset</span></span> |<span data-ttu-id="73aa4-115">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="73aa4-115">The start time of the operation.</span></span>|
|<span data-ttu-id="73aa4-116">erro</span><span class="sxs-lookup"><span data-stu-id="73aa4-116">error</span></span>|[<span data-ttu-id="73aa4-117">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="73aa4-117">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="73aa4-118">O erro retornado pela operação.</span><span class="sxs-lookup"><span data-stu-id="73aa4-118">The error returned by the operation.</span></span>|
|<span data-ttu-id="73aa4-119">id</span><span class="sxs-lookup"><span data-stu-id="73aa4-119">id</span></span>|<span data-ttu-id="73aa4-120">string</span><span class="sxs-lookup"><span data-stu-id="73aa4-120">string</span></span>|<span data-ttu-id="73aa4-121">A id da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73aa4-121">The operation id. Read-only.</span></span>|
|<span data-ttu-id="73aa4-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="73aa4-122">lastActionDateTime</span></span>| <span data-ttu-id="73aa4-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73aa4-123">DateTimeOffset</span></span> |<span data-ttu-id="73aa4-124">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="73aa4-124">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="73aa4-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="73aa4-125">resourceId</span></span>|<span data-ttu-id="73aa4-126">string</span><span class="sxs-lookup"><span data-stu-id="73aa4-126">string</span></span>|<span data-ttu-id="73aa4-127">A id do recurso.</span><span class="sxs-lookup"><span data-stu-id="73aa4-127">The resource id.</span></span>|
|<span data-ttu-id="73aa4-128">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="73aa4-128">resourceLocation</span></span>|<span data-ttu-id="73aa4-129">string</span><span class="sxs-lookup"><span data-stu-id="73aa4-129">string</span></span>|<span data-ttu-id="73aa4-p102">O URI de recurso do objeto. Por exemplo, o URI de recurso para uma seção ou página copiada.</span><span class="sxs-lookup"><span data-stu-id="73aa4-p102">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="73aa4-132">status</span><span class="sxs-lookup"><span data-stu-id="73aa4-132">status</span></span>|<span data-ttu-id="73aa4-133">string</span><span class="sxs-lookup"><span data-stu-id="73aa4-133">string</span></span>|<span data-ttu-id="73aa4-134">O status atual da operação: `notstarted`, `running`, `completed`, `failed`</span><span class="sxs-lookup"><span data-stu-id="73aa4-134">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="73aa4-135">percentComplete</span><span class="sxs-lookup"><span data-stu-id="73aa4-135">percentComplete</span></span>|<span data-ttu-id="73aa4-136">string</span><span class="sxs-lookup"><span data-stu-id="73aa4-136">string</span></span>|<span data-ttu-id="73aa4-137">A porcentagem concluída da operação se a operação ainda estiver com um status `running`</span><span class="sxs-lookup"><span data-stu-id="73aa4-137">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="73aa4-138">Relações</span><span class="sxs-lookup"><span data-stu-id="73aa4-138">Relationships</span></span>
<span data-ttu-id="73aa4-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="73aa4-139">None</span></span>


## <a name="methods"></a><span data-ttu-id="73aa4-140">Métodos</span><span class="sxs-lookup"><span data-stu-id="73aa4-140">Methods</span></span>

| <span data-ttu-id="73aa4-141">Método</span><span class="sxs-lookup"><span data-stu-id="73aa4-141">Method</span></span>           | <span data-ttu-id="73aa4-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="73aa4-142">Return Type</span></span>    |<span data-ttu-id="73aa4-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="73aa4-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="73aa4-144">Get operation</span><span class="sxs-lookup"><span data-stu-id="73aa4-144">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="73aa4-145">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="73aa4-145">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="73aa4-146">Obter o status atual da operação.</span><span class="sxs-lookup"><span data-stu-id="73aa4-146">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
