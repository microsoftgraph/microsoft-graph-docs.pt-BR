---
title: usado o tipo de recurso
description: 'Uma compreensão dos representando documentos usados por um usuário específico. As ideias retorna os documentos mais relevantes que um usuário visualizados ou acessados. Isso inclui documentos em:'
ms.openlocfilehash: 3c82d268a67ef52d0ddfdad9193558080048ad6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038991"
---
# <a name="used-resource-type"></a><span data-ttu-id="452e9-105">usado o tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="452e9-105">used resource type</span></span>

> <span data-ttu-id="452e9-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="452e9-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="452e9-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="452e9-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="452e9-108">Uma compreensão dos representando documentos usados por um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="452e9-108">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="452e9-109">As ideias retorna os documentos mais relevantes que um usuário visualizados ou acessados.</span><span class="sxs-lookup"><span data-stu-id="452e9-109">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="452e9-110">Isso inclui documentos em:</span><span class="sxs-lookup"><span data-stu-id="452e9-110">This includes documents in:</span></span>

- <span data-ttu-id="452e9-111">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="452e9-111">OneDrive for Business</span></span>
- <span data-ttu-id="452e9-112">SharePoint</span><span class="sxs-lookup"><span data-stu-id="452e9-112">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="452e9-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="452e9-113">Methods</span></span>

| <span data-ttu-id="452e9-114">Método</span><span class="sxs-lookup"><span data-stu-id="452e9-114">Method</span></span>       | <span data-ttu-id="452e9-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="452e9-115">Return Type</span></span>  |<span data-ttu-id="452e9-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="452e9-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="452e9-117">Lista usada</span><span class="sxs-lookup"><span data-stu-id="452e9-117">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="452e9-118">coleção [insights_used](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="452e9-118">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="452e9-119">Obtenha uma lista de arquivos utilizados.</span><span class="sxs-lookup"><span data-stu-id="452e9-119">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="452e9-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="452e9-120">Properties</span></span>

| <span data-ttu-id="452e9-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="452e9-121">Property</span></span>              | <span data-ttu-id="452e9-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="452e9-122">Type</span></span>                      | <span data-ttu-id="452e9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="452e9-123">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="452e9-124">id</span><span class="sxs-lookup"><span data-stu-id="452e9-124">id</span></span>                    | <span data-ttu-id="452e9-125">String</span><span class="sxs-lookup"><span data-stu-id="452e9-125">String</span></span>                    | <span data-ttu-id="452e9-126">Identificador exclusivo do relacionamento.</span><span class="sxs-lookup"><span data-stu-id="452e9-126">Unique identifier of the relationship.</span></span> <span data-ttu-id="452e9-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="452e9-127">Read only.</span></span>        |
| <span data-ttu-id="452e9-128">lastUsed</span><span class="sxs-lookup"><span data-stu-id="452e9-128">lastUsed</span></span>              | [<span data-ttu-id="452e9-129">usageDetails</span><span class="sxs-lookup"><span data-stu-id="452e9-129">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="452e9-130">Informações sobre quando o item foi último exibidos e modificados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="452e9-130">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="452e9-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="452e9-131">Read only.</span></span>     |
| <span data-ttu-id="452e9-132">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="452e9-132">resourceVisualization</span></span> | [<span data-ttu-id="452e9-133">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="452e9-133">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="452e9-134">Propriedades que você pode usar para visualizar o documento na sua experiência.</span><span class="sxs-lookup"><span data-stu-id="452e9-134">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="452e9-135">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="452e9-135">Read-only</span></span>      |
| <span data-ttu-id="452e9-136">resourceReference</span><span class="sxs-lookup"><span data-stu-id="452e9-136">resourceReference</span></span>     | [<span data-ttu-id="452e9-137">resourceReference</span><span class="sxs-lookup"><span data-stu-id="452e9-137">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="452e9-138">Propriedades de referência do documento usado, como a url e o tipo de documento.</span><span class="sxs-lookup"><span data-stu-id="452e9-138">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="452e9-139">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="452e9-139">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="452e9-140">Relações</span><span class="sxs-lookup"><span data-stu-id="452e9-140">Relationships</span></span>

| <span data-ttu-id="452e9-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="452e9-141">Property</span></span>      | <span data-ttu-id="452e9-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="452e9-142">Type</span></span>          | <span data-ttu-id="452e9-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="452e9-143">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="452e9-144">recurso</span><span class="sxs-lookup"><span data-stu-id="452e9-144">resource</span></span>      | <span data-ttu-id="452e9-145">Entidade</span><span class="sxs-lookup"><span data-stu-id="452e9-145">Entity</span></span>        | <span data-ttu-id="452e9-146">Usado para navegar até o item que foi usado.</span><span class="sxs-lookup"><span data-stu-id="452e9-146">Used for navigating to the item that was used.</span></span> <span data-ttu-id="452e9-147">Anexos de arquivo, o tipo é *fileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="452e9-147">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="452e9-148">Anexos vinculados, o tipo é *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="452e9-148">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="452e9-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="452e9-149">JSON representation</span></span>
<span data-ttu-id="452e9-150">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="452e9-150">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```