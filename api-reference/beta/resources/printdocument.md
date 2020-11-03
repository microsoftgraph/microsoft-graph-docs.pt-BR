---
title: tipo de recurso de documento de documentos
description: Representa um documento que está sendo impresso.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c0bc886b618e061bee51ad82d7032737015f58ab
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849207"
---
# <a name="printdocument-resource-type"></a><span data-ttu-id="090ca-103">tipo de recurso de documento de documentos</span><span class="sxs-lookup"><span data-stu-id="090ca-103">printDocument resource type</span></span>

<span data-ttu-id="090ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="090ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="090ca-105">Representa um documento que está sendo impresso.</span><span class="sxs-lookup"><span data-stu-id="090ca-105">Represents a document being printed.</span></span>

## <a name="methods"></a><span data-ttu-id="090ca-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="090ca-106">Methods</span></span>

| <span data-ttu-id="090ca-107">Método</span><span class="sxs-lookup"><span data-stu-id="090ca-107">Method</span></span>       | <span data-ttu-id="090ca-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="090ca-108">Return Type</span></span> | <span data-ttu-id="090ca-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="090ca-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="090ca-110">Criar sessão de upload</span><span class="sxs-lookup"><span data-stu-id="090ca-110">Create upload session</span></span>](../api/printdocument-createuploadsession.md) | [<span data-ttu-id="090ca-111">uploadSession</span><span class="sxs-lookup"><span data-stu-id="090ca-111">uploadSession</span></span>](uploadsession.md) | <span data-ttu-id="090ca-112">Criar uma sessão de carregamento para carregar com interseção intervalos de arquivos binários do **documento**.</span><span class="sxs-lookup"><span data-stu-id="090ca-112">Create an upload session to iteratively upload ranges of binary file of the **printDocument**.</span></span> |
| [<span data-ttu-id="090ca-113">Baixar arquivo binário</span><span class="sxs-lookup"><span data-stu-id="090ca-113">Download binary file</span></span>](../api/printdocument-get-file.md) | <span data-ttu-id="090ca-114">URL de download</span><span class="sxs-lookup"><span data-stu-id="090ca-114">Download Url</span></span> | <span data-ttu-id="090ca-115">Baixe o arquivo binário associado ao **documento**.</span><span class="sxs-lookup"><span data-stu-id="090ca-115">Download the binary file associated with the **printDocument**.</span></span> |

## <a name="properties"></a><span data-ttu-id="090ca-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="090ca-116">Properties</span></span>
| <span data-ttu-id="090ca-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="090ca-117">Property</span></span>     | <span data-ttu-id="090ca-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="090ca-118">Type</span></span>        | <span data-ttu-id="090ca-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="090ca-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="090ca-120">id</span><span class="sxs-lookup"><span data-stu-id="090ca-120">id</span></span>|<span data-ttu-id="090ca-121">String</span><span class="sxs-lookup"><span data-stu-id="090ca-121">String</span></span>|<span data-ttu-id="090ca-122">O identificador do documento.</span><span class="sxs-lookup"><span data-stu-id="090ca-122">The document's identifier.</span></span> <span data-ttu-id="090ca-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="090ca-123">Read-only.</span></span>|
|<span data-ttu-id="090ca-124">displayName</span><span class="sxs-lookup"><span data-stu-id="090ca-124">displayName</span></span>|<span data-ttu-id="090ca-125">String</span><span class="sxs-lookup"><span data-stu-id="090ca-125">String</span></span>|<span data-ttu-id="090ca-126">O nome do documento.</span><span class="sxs-lookup"><span data-stu-id="090ca-126">The document's name.</span></span> <span data-ttu-id="090ca-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="090ca-127">Read-only.</span></span>|
|<span data-ttu-id="090ca-128">contentType</span><span class="sxs-lookup"><span data-stu-id="090ca-128">contentType</span></span>|<span data-ttu-id="090ca-129">String</span><span class="sxs-lookup"><span data-stu-id="090ca-129">String</span></span>|<span data-ttu-id="090ca-130">O tipo de conteúdo do documento (MIME).</span><span class="sxs-lookup"><span data-stu-id="090ca-130">The document's content (MIME) type.</span></span> <span data-ttu-id="090ca-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="090ca-131">Read-only.</span></span>|
|<span data-ttu-id="090ca-132">size</span><span class="sxs-lookup"><span data-stu-id="090ca-132">size</span></span>|<span data-ttu-id="090ca-133">Int64</span><span class="sxs-lookup"><span data-stu-id="090ca-133">Int64</span></span>|<span data-ttu-id="090ca-134">O tamanho do documento em bytes.</span><span class="sxs-lookup"><span data-stu-id="090ca-134">The document's size in bytes.</span></span> <span data-ttu-id="090ca-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="090ca-135">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="090ca-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="090ca-136">JSON representation</span></span>

<span data-ttu-id="090ca-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="090ca-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printDocument"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "contentType": "String",
  "size": 12345
}

```


