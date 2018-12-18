---
title: usado o tipo de recurso
description: Uma compreensão dos representando documentos usados por um usuário específico. As ideias retorna os documentos mais relevantes que um usuário visualizados ou acessados.
author: simonhult
ms.openlocfilehash: 89eac33ad954905c77a26df669bb15a2cf471edd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323482"
---
# <a name="used-resource-type"></a><span data-ttu-id="99a3d-104">usado o tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="99a3d-104">used resource type</span></span>

> <span data-ttu-id="99a3d-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="99a3d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99a3d-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="99a3d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99a3d-107">Uma compreensão dos representando documentos usados por um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="99a3d-107">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="99a3d-108">As ideias retorna os documentos mais relevantes que um usuário visualizados ou acessados.</span><span class="sxs-lookup"><span data-stu-id="99a3d-108">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="99a3d-109">Isso inclui documentos em:</span><span class="sxs-lookup"><span data-stu-id="99a3d-109">This includes documents in:</span></span>

- <span data-ttu-id="99a3d-110">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="99a3d-110">OneDrive for Business</span></span>
- <span data-ttu-id="99a3d-111">SharePoint</span><span class="sxs-lookup"><span data-stu-id="99a3d-111">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="99a3d-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="99a3d-112">Methods</span></span>

| <span data-ttu-id="99a3d-113">Método</span><span class="sxs-lookup"><span data-stu-id="99a3d-113">Method</span></span>       | <span data-ttu-id="99a3d-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="99a3d-114">Return Type</span></span>  |<span data-ttu-id="99a3d-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="99a3d-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="99a3d-116">Lista usada</span><span class="sxs-lookup"><span data-stu-id="99a3d-116">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="99a3d-117">coleção [insights_used](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="99a3d-117">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="99a3d-118">Obtenha uma lista de arquivos utilizados.</span><span class="sxs-lookup"><span data-stu-id="99a3d-118">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="99a3d-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99a3d-119">Properties</span></span>

| <span data-ttu-id="99a3d-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99a3d-120">Property</span></span>              | <span data-ttu-id="99a3d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="99a3d-121">Type</span></span>                      | <span data-ttu-id="99a3d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="99a3d-122">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="99a3d-123">id</span><span class="sxs-lookup"><span data-stu-id="99a3d-123">id</span></span>                    | <span data-ttu-id="99a3d-124">String</span><span class="sxs-lookup"><span data-stu-id="99a3d-124">String</span></span>                    | <span data-ttu-id="99a3d-125">Identificador exclusivo do relacionamento.</span><span class="sxs-lookup"><span data-stu-id="99a3d-125">Unique identifier of the relationship.</span></span> <span data-ttu-id="99a3d-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="99a3d-126">Read only.</span></span>        |
| <span data-ttu-id="99a3d-127">lastUsed</span><span class="sxs-lookup"><span data-stu-id="99a3d-127">lastUsed</span></span>              | [<span data-ttu-id="99a3d-128">usageDetails</span><span class="sxs-lookup"><span data-stu-id="99a3d-128">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="99a3d-129">Informações sobre quando o item foi último exibidos e modificados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="99a3d-129">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="99a3d-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="99a3d-130">Read only.</span></span>     |
| <span data-ttu-id="99a3d-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="99a3d-131">resourceVisualization</span></span> | [<span data-ttu-id="99a3d-132">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="99a3d-132">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="99a3d-133">Propriedades que você pode usar para visualizar o documento na sua experiência.</span><span class="sxs-lookup"><span data-stu-id="99a3d-133">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="99a3d-134">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="99a3d-134">Read-only</span></span>      |
| <span data-ttu-id="99a3d-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="99a3d-135">resourceReference</span></span>     | [<span data-ttu-id="99a3d-136">resourceReference</span><span class="sxs-lookup"><span data-stu-id="99a3d-136">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="99a3d-137">Propriedades de referência do documento usado, como a url e o tipo de documento.</span><span class="sxs-lookup"><span data-stu-id="99a3d-137">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="99a3d-138">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="99a3d-138">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="99a3d-139">Relações</span><span class="sxs-lookup"><span data-stu-id="99a3d-139">Relationships</span></span>

| <span data-ttu-id="99a3d-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99a3d-140">Property</span></span>      | <span data-ttu-id="99a3d-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="99a3d-141">Type</span></span>          | <span data-ttu-id="99a3d-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="99a3d-142">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="99a3d-143">recurso</span><span class="sxs-lookup"><span data-stu-id="99a3d-143">resource</span></span>      | <span data-ttu-id="99a3d-144">Entity</span><span class="sxs-lookup"><span data-stu-id="99a3d-144">Entity</span></span>        | <span data-ttu-id="99a3d-145">Usado para navegar até o item que foi usado.</span><span class="sxs-lookup"><span data-stu-id="99a3d-145">Used for navigating to the item that was used.</span></span> <span data-ttu-id="99a3d-146">Anexos de arquivo, o tipo é *fileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="99a3d-146">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="99a3d-147">Anexos vinculados, o tipo é *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="99a3d-147">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="99a3d-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99a3d-148">JSON representation</span></span>
<span data-ttu-id="99a3d-149">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="99a3d-149">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```