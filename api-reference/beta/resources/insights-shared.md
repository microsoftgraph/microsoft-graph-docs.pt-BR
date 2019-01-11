---
title: tipo de recurso compartilhado
description: 'Uma compreensão dos representando arquivos compartilhados com ou por um usuário específico. Há suporte para os seguintes arquivos compartilhados:'
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 289523f836d7b8080f7317e4d11301c71314ba93
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880609"
---
# <a name="shared-resource-type"></a><span data-ttu-id="bd24c-104">tipo de recurso compartilhado</span><span class="sxs-lookup"><span data-stu-id="bd24c-104">shared resource type</span></span>

> <span data-ttu-id="bd24c-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bd24c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd24c-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bd24c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bd24c-107">Uma compreensão dos representando arquivos compartilhados com ou por um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="bd24c-107">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="bd24c-108">Há suporte para os seguintes arquivos compartilhados:</span><span class="sxs-lookup"><span data-stu-id="bd24c-108">The following shared files are supported:</span></span>

- <span data-ttu-id="bd24c-109">Arquivos anexados diretamente em um email ou uma reunião convidem.</span><span class="sxs-lookup"><span data-stu-id="bd24c-109">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="bd24c-110">OneDrive para Bussiness e SharePoint modernos anexos - arquivos armazenados no OneDrive para negócios e do SharePoint que os usuários compartilhem como links em um email.</span><span class="sxs-lookup"><span data-stu-id="bd24c-110">OneDrive for Bussiness and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="bd24c-111">**Observação**: estamos atualmente trabalhando em preencher os resultados da API compartilhados com dados.</span><span class="sxs-lookup"><span data-stu-id="bd24c-111">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="bd24c-112">Pode haver alguns dados ausentes nas semanas primeira depois do lançamento.</span><span class="sxs-lookup"><span data-stu-id="bd24c-112">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="bd24c-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="bd24c-113">Methods</span></span>

| <span data-ttu-id="bd24c-114">Método</span><span class="sxs-lookup"><span data-stu-id="bd24c-114">Method</span></span>       | <span data-ttu-id="bd24c-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bd24c-115">Return Type</span></span>  |<span data-ttu-id="bd24c-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd24c-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bd24c-117">Lista compartilhada</span><span class="sxs-lookup"><span data-stu-id="bd24c-117">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="bd24c-118">coleção [insights_shared](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="bd24c-118">[insights_shared](insights-shared.md) collection</span></span>| <span data-ttu-id="bd24c-119">Obtenha uma lista de arquivos compartilhados.</span><span class="sxs-lookup"><span data-stu-id="bd24c-119">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="bd24c-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bd24c-120">Properties</span></span>

| <span data-ttu-id="bd24c-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd24c-121">Property</span></span>              | <span data-ttu-id="bd24c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd24c-122">Type</span></span>                      | <span data-ttu-id="bd24c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd24c-123">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="bd24c-124">id</span><span class="sxs-lookup"><span data-stu-id="bd24c-124">id</span></span>                    | <span data-ttu-id="bd24c-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd24c-125">String</span></span>                    | <span data-ttu-id="bd24c-126">Identificador exclusivo do relacionamento.</span><span class="sxs-lookup"><span data-stu-id="bd24c-126">Unique identifier of the relationship.</span></span> <span data-ttu-id="bd24c-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bd24c-127">Read only.</span></span>        |
| <span data-ttu-id="bd24c-128">lastShared</span><span class="sxs-lookup"><span data-stu-id="bd24c-128">lastShared</span></span>            | [<span data-ttu-id="bd24c-129">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="bd24c-129">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="bd24c-130">Detalhes sobre o item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="bd24c-130">Details about the shared item.</span></span> <span data-ttu-id="bd24c-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bd24c-131">Read only.</span></span>        |
| <span data-ttu-id="bd24c-132">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="bd24c-132">resourceVisualization</span></span> | [<span data-ttu-id="bd24c-133">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="bd24c-133">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="bd24c-134">Propriedades que você pode usar para visualizar o documento na sua experiência.</span><span class="sxs-lookup"><span data-stu-id="bd24c-134">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="bd24c-135">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="bd24c-135">Read-only</span></span>      |
| <span data-ttu-id="bd24c-136">resourceReference</span><span class="sxs-lookup"><span data-stu-id="bd24c-136">resourceReference</span></span>     | [<span data-ttu-id="bd24c-137">resourceReference</span><span class="sxs-lookup"><span data-stu-id="bd24c-137">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="bd24c-138">Propriedades de referência do documento compartilhado, como a url e o tipo de documento.</span><span class="sxs-lookup"><span data-stu-id="bd24c-138">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="bd24c-139">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="bd24c-139">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="bd24c-140">Relações</span><span class="sxs-lookup"><span data-stu-id="bd24c-140">Relationships</span></span>

| <span data-ttu-id="bd24c-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd24c-141">Property</span></span>      | <span data-ttu-id="bd24c-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd24c-142">Type</span></span>          | <span data-ttu-id="bd24c-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd24c-143">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="bd24c-144">recurso</span><span class="sxs-lookup"><span data-stu-id="bd24c-144">resource</span></span>      | <span data-ttu-id="bd24c-145">Entity</span><span class="sxs-lookup"><span data-stu-id="bd24c-145">Entity</span></span>        | <span data-ttu-id="bd24c-146">Usado para navegar até o item que foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="bd24c-146">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="bd24c-147">Anexos de arquivo, o tipo é *fileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="bd24c-147">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="bd24c-148">Anexos vinculados, o tipo é *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="bd24c-148">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bd24c-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bd24c-149">JSON representation</span></span>
<span data-ttu-id="bd24c-150">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bd24c-150">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
