---
author: swapnil1993
title: Tipo de recurso documentSetContent
description: O recurso documentSetContent contém metadados sobre um arquivo presente no local de conteúdo padrão de um conteúdo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8597dfb8a762d2166a9253fb4e806b9c2fcf5223
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445907"
---
# <a name="documentsetcontent-resource-type"></a><span data-ttu-id="fd01f-103">Tipo de recurso documentSetContent</span><span class="sxs-lookup"><span data-stu-id="fd01f-103">documentSetContent resource type</span></span>

<span data-ttu-id="fd01f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd01f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="fd01f-105">Contém metadados sobre um arquivo presente no local de conteúdo padrão de um tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="fd01f-105">Contains metadata about a file present in default content location of a content type.</span></span>

## <a name="properties"></a><span data-ttu-id="fd01f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd01f-106">Properties</span></span>

| <span data-ttu-id="fd01f-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="fd01f-107">Property name</span></span>  | <span data-ttu-id="fd01f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd01f-108">Type</span></span>    | <span data-ttu-id="fd01f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd01f-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="fd01f-110">contentType</span><span class="sxs-lookup"><span data-stu-id="fd01f-110">contentType</span></span>    | <span data-ttu-id="fd01f-111">microsoft.graph.contentTypeInfo</span><span class="sxs-lookup"><span data-stu-id="fd01f-111">microsoft.graph.contentTypeInfo</span></span> | <span data-ttu-id="fd01f-112">Informações de tipo de conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="fd01f-112">Content type information of the file.</span></span> 
| <span data-ttu-id="fd01f-113">fileName</span><span class="sxs-lookup"><span data-stu-id="fd01f-113">fileName</span></span>      | <span data-ttu-id="fd01f-114">string</span><span class="sxs-lookup"><span data-stu-id="fd01f-114">string</span></span>  | <span data-ttu-id="fd01f-115">Nome do arquivo na pasta de recursos que deve ser adicionado como um conteúdo padrão ou um modelo no conjunto de documentos</span><span class="sxs-lookup"><span data-stu-id="fd01f-115">Name of the file in resource folder that should be added as a default content or a template in the document set</span></span>  
| <span data-ttu-id="fd01f-116">folderName</span><span class="sxs-lookup"><span data-stu-id="fd01f-116">folderName</span></span>         | <span data-ttu-id="fd01f-117">string</span><span class="sxs-lookup"><span data-stu-id="fd01f-117">string</span></span>  | <span data-ttu-id="fd01f-118">Nome da pasta no qual o arquivo será colocado quando um novo conjunto de documentos for criado na biblioteca.</span><span class="sxs-lookup"><span data-stu-id="fd01f-118">Folder name in which the file will be placed when a new document set is created in the library.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd01f-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd01f-119">JSON representation</span></span>

<span data-ttu-id="fd01f-120">Aqui está uma representação JSON de um **recurso documentSetContent.**</span><span class="sxs-lookup"><span data-stu-id="fd01f-120">Here is a JSON representation of a **documentSetContent** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.documentSetContent" } -->

```json
{
  "contentType": { "@type": "microsoft.graph.contentTypeInfo" },
  "fileName": "string",
  "folderName": "string"
}
```