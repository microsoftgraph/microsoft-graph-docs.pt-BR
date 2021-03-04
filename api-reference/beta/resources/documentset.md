---
author: swapnil1993
title: Tipo de recurso documentSet
description: Contém metadados sobre configurações de conjunto de documentos.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 25a2b5e71c76a8a097ff9c490313ae6d319abeb8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445906"
---
# <a name="documentset-resource-type"></a><span data-ttu-id="07c80-103">Tipo de recurso documentSet</span><span class="sxs-lookup"><span data-stu-id="07c80-103">documentSet resource type</span></span>

<span data-ttu-id="07c80-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07c80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="07c80-105">Contém metadados sobre configurações de conjunto de documentos.</span><span class="sxs-lookup"><span data-stu-id="07c80-105">Contains metadata about document set settings.</span></span>

## <a name="properties"></a><span data-ttu-id="07c80-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07c80-106">Properties</span></span>

| <span data-ttu-id="07c80-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="07c80-107">Property name</span></span>  | <span data-ttu-id="07c80-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="07c80-108">Type</span></span>    | <span data-ttu-id="07c80-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="07c80-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="07c80-110">shouldPrefixNameToFile</span><span class="sxs-lookup"><span data-stu-id="07c80-110">shouldPrefixNameToFile</span></span> | <span data-ttu-id="07c80-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="07c80-111">Boolean</span></span>  | <span data-ttu-id="07c80-112">Adicione o nome do Conjunto de Documentos a cada nome de arquivo.</span><span class="sxs-lookup"><span data-stu-id="07c80-112">Add the name of the Document Set to each file name.</span></span>
| <span data-ttu-id="07c80-113">allowedContentTypes</span><span class="sxs-lookup"><span data-stu-id="07c80-113">allowedContentTypes</span></span> | <span data-ttu-id="07c80-114">Collection(microsoft.graph.contentTypeInfo)</span><span class="sxs-lookup"><span data-stu-id="07c80-114">Collection(microsoft.graph.contentTypeInfo)</span></span> | <span data-ttu-id="07c80-115">Tipos de conteúdo permitidos no conjunto de documentos.</span><span class="sxs-lookup"><span data-stu-id="07c80-115">Content types allowed in document set.</span></span>
| <span data-ttu-id="07c80-116">defaultContents</span><span class="sxs-lookup"><span data-stu-id="07c80-116">defaultContents</span></span>     | <span data-ttu-id="07c80-117">Collection(microsoft.graph.documentSetContent)</span><span class="sxs-lookup"><span data-stu-id="07c80-117">Collection(microsoft.graph.documentSetContent)</span></span> | <span data-ttu-id="07c80-118">Conteúdo padrão do conjunto de documentos.</span><span class="sxs-lookup"><span data-stu-id="07c80-118">Default contents of document set.</span></span>  
| <span data-ttu-id="07c80-119">propagateWelcomePageChanges</span><span class="sxs-lookup"><span data-stu-id="07c80-119">propagateWelcomePageChanges</span></span> | <span data-ttu-id="07c80-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="07c80-120">Boolean</span></span> | <span data-ttu-id="07c80-121">Especifica se a página de boas-vindas deve ser pressionada para tipos de conteúdo herdados.</span><span class="sxs-lookup"><span data-stu-id="07c80-121">Specifies whether to push welcome page changes to inherited content types.</span></span>  
| <span data-ttu-id="07c80-122">sharedColumns</span><span class="sxs-lookup"><span data-stu-id="07c80-122">sharedColumns</span></span>       | <span data-ttu-id="07c80-123">Collection(microsoft.graph.columnDefinition)</span><span class="sxs-lookup"><span data-stu-id="07c80-123">Collection(microsoft.graph.columnDefinition)</span></span> | <span data-ttu-id="07c80-124">Colunas editadas no conjunto de documentos que se sincronizam com todos os documentos no conjunto.</span><span class="sxs-lookup"><span data-stu-id="07c80-124">Columns edited on the document set that synchronize to all documents in the set.</span></span> <span data-ttu-id="07c80-125">Eles são somente leitura nos próprios documentos.</span><span class="sxs-lookup"><span data-stu-id="07c80-125">These are read-only on the documents themselves.</span></span> 
| <span data-ttu-id="07c80-126">welcomePageColumns</span><span class="sxs-lookup"><span data-stu-id="07c80-126">welcomePageColumns</span></span>  | <span data-ttu-id="07c80-127">Collection(microsoft.graph.columnDefinition)</span><span class="sxs-lookup"><span data-stu-id="07c80-127">Collection(microsoft.graph.columnDefinition)</span></span>  | <span data-ttu-id="07c80-128">Especifica colunas a mostrar na página de boas-vindas para o conjunto de documentos.</span><span class="sxs-lookup"><span data-stu-id="07c80-128">Specifies columns to show on the welcome page for the document set.</span></span>  
| <span data-ttu-id="07c80-129">welcomePageUrl</span><span class="sxs-lookup"><span data-stu-id="07c80-129">welcomePageUrl</span></span>      | <span data-ttu-id="07c80-130">string</span><span class="sxs-lookup"><span data-stu-id="07c80-130">string</span></span> | <span data-ttu-id="07c80-131">URL absoluta da página de boas-vindas.</span><span class="sxs-lookup"><span data-stu-id="07c80-131">Welcome page absolute URL.</span></span>  

## <a name="json-representation"></a><span data-ttu-id="07c80-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07c80-132">JSON representation</span></span>

<span data-ttu-id="07c80-133">A seguir está uma representação JSON de um **recurso documentSet.**</span><span class="sxs-lookup"><span data-stu-id="07c80-133">The following is a JSON representation of a **documentSet** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.documentSet" } -->

```json
{
  "shouldPrefixNameToFile": true,
  "allowedContentTypes": [{ "@type": "microsoft.graph.contentTypeInfo" }],
  "defaultContents": [{ "@type": "microsoft.graph.documentSetContent" }],
  "propagateWelcomePageChanges": false,
  "sharedColumns": [{ "@type": "microsoft.graph.columnDefinition" }],
  "welcomePageColumns": [{ "@type": "microsoft.graph.columnDefinition" }],
  "welcomePageUrl": "string"
}
```

[contentTypeInfo]: contentTypeInfo.md
[documentSetContent]: documentsetcontent.md
