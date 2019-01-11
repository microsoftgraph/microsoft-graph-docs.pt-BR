---
title: usado o tipo de recurso
description: Uma compreensão dos representando documentos usados por um usuário específico. As ideias retorna os documentos mais relevantes que um usuário visualizados ou acessados.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: cb41fcb7cef5c9e39f9100ebd1d8c2640f06e2d0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885530"
---
# <a name="used-resource-type"></a><span data-ttu-id="4bcc6-104">usado o tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="4bcc6-104">used resource type</span></span>

> <span data-ttu-id="4bcc6-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4bcc6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4bcc6-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4bcc6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4bcc6-107">Uma compreensão dos representando documentos usados por um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="4bcc6-107">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="4bcc6-108">As ideias retorna os documentos mais relevantes que um usuário visualizados ou acessados.</span><span class="sxs-lookup"><span data-stu-id="4bcc6-108">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="4bcc6-109">Isso inclui documentos em:</span><span class="sxs-lookup"><span data-stu-id="4bcc6-109">This includes documents in:</span></span>

- <span data-ttu-id="4bcc6-110">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="4bcc6-110">OneDrive for Business</span></span>
- <span data-ttu-id="4bcc6-111">SharePoint</span><span class="sxs-lookup"><span data-stu-id="4bcc6-111">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="4bcc6-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="4bcc6-112">Methods</span></span>

| <span data-ttu-id="4bcc6-113">Método</span><span class="sxs-lookup"><span data-stu-id="4bcc6-113">Method</span></span>       | <span data-ttu-id="4bcc6-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4bcc6-114">Return Type</span></span>  |<span data-ttu-id="4bcc6-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bcc6-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4bcc6-116">Lista usada</span><span class="sxs-lookup"><span data-stu-id="4bcc6-116">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="4bcc6-117">coleção [insights_used](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="4bcc6-117">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="4bcc6-118">Obtenha uma lista de arquivos utilizados.</span><span class="sxs-lookup"><span data-stu-id="4bcc6-118">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="4bcc6-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4bcc6-119">Properties</span></span>

| <span data-ttu-id="4bcc6-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4bcc6-120">Property</span></span>              | <span data-ttu-id="4bcc6-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bcc6-121">Type</span></span>                      | <span data-ttu-id="4bcc6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bcc6-122">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="4bcc6-123">id</span><span class="sxs-lookup"><span data-stu-id="4bcc6-123">id</span></span>                    | <span data-ttu-id="4bcc6-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4bcc6-124">String</span></span>                    | <span data-ttu-id="4bcc6-125">Identificador exclusivo do relacionamento.</span><span class="sxs-lookup"><span data-stu-id="4bcc6-125">Unique identifier of the relationship.</span></span> <span data-ttu-id="4bcc6-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4bcc6-126">Read only.</span></span>        |
| <span data-ttu-id="4bcc6-127">lastUsed</span><span class="sxs-lookup"><span data-stu-id="4bcc6-127">lastUsed</span></span>              | [<span data-ttu-id="4bcc6-128">usageDetails</span><span class="sxs-lookup"><span data-stu-id="4bcc6-128">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="4bcc6-129">Informações sobre quando o item foi último exibidos e modificados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="4bcc6-129">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="4bcc6-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4bcc6-130">Read only.</span></span>     |
| <span data-ttu-id="4bcc6-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="4bcc6-131">resourceVisualization</span></span> | [<span data-ttu-id="4bcc6-132">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="4bcc6-132">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="4bcc6-133">Propriedades que você pode usar para visualizar o documento na sua experiência.</span><span class="sxs-lookup"><span data-stu-id="4bcc6-133">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="4bcc6-134">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="4bcc6-134">Read-only</span></span>      |
| <span data-ttu-id="4bcc6-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="4bcc6-135">resourceReference</span></span>     | [<span data-ttu-id="4bcc6-136">resourceReference</span><span class="sxs-lookup"><span data-stu-id="4bcc6-136">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="4bcc6-137">Propriedades de referência do documento usado, como a url e o tipo de documento.</span><span class="sxs-lookup"><span data-stu-id="4bcc6-137">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="4bcc6-138">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="4bcc6-138">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="4bcc6-139">Relações</span><span class="sxs-lookup"><span data-stu-id="4bcc6-139">Relationships</span></span>

| <span data-ttu-id="4bcc6-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4bcc6-140">Property</span></span>      | <span data-ttu-id="4bcc6-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bcc6-141">Type</span></span>          | <span data-ttu-id="4bcc6-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bcc6-142">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="4bcc6-143">recurso</span><span class="sxs-lookup"><span data-stu-id="4bcc6-143">resource</span></span>      | <span data-ttu-id="4bcc6-144">Entity</span><span class="sxs-lookup"><span data-stu-id="4bcc6-144">Entity</span></span>        | <span data-ttu-id="4bcc6-145">Usado para navegar até o item que foi usado.</span><span class="sxs-lookup"><span data-stu-id="4bcc6-145">Used for navigating to the item that was used.</span></span> <span data-ttu-id="4bcc6-146">Anexos de arquivo, o tipo é *fileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="4bcc6-146">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="4bcc6-147">Anexos vinculados, o tipo é *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="4bcc6-147">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4bcc6-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4bcc6-148">JSON representation</span></span>
<span data-ttu-id="4bcc6-149">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="4bcc6-149">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
