---
title: tipo de recurso driveItemUploadableProperties
description: O recurso driveItemUploadableProperties representa um item sendo carregado durante a criação de uma sessão de carregamento.
localization_priority: Normal
author: JeremyKelley
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 1f3ef83f36af70aa2efd3cce8d0215d705114e50
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863870"
---
# <a name="driveitemuploadableproperties-resource-type"></a><span data-ttu-id="3aefc-103">tipo de recurso driveItemUploadableProperties</span><span class="sxs-lookup"><span data-stu-id="3aefc-103">driveItemUploadableProperties resource type</span></span>

<span data-ttu-id="3aefc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3aefc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3aefc-105">Representa um item que está sendo carregado ao [criar uma sessão de carregamento](../api/driveitem-createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="3aefc-105">Represents an item being uploaded when [creating an upload session](../api/driveitem-createuploadsession.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="3aefc-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3aefc-106">JSON representation</span></span>

<span data-ttu-id="3aefc-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3aefc-107">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.driveItemUploadableProperties",
  "baseType": null
}-->

```json
{
  "description": "String",
  "fileSize": 1024,
  "fileSystemInfo": {"@odata.type": "microsoft.graph.fileSystemInfo"},
  "name": "String"
}
```

## <a name="properties"></a><span data-ttu-id="3aefc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3aefc-108">Properties</span></span>

| <span data-ttu-id="3aefc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3aefc-109">Property</span></span>     | <span data-ttu-id="3aefc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3aefc-110">Type</span></span>                              | <span data-ttu-id="3aefc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3aefc-111">Description</span></span>                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|<span data-ttu-id="3aefc-112">**description**</span><span class="sxs-lookup"><span data-stu-id="3aefc-112">**description**</span></span>   |<span data-ttu-id="3aefc-113">String</span><span class="sxs-lookup"><span data-stu-id="3aefc-113">String</span></span>                             | <span data-ttu-id="3aefc-114">Fornece uma descrição do item visível para o usuário.</span><span class="sxs-lookup"><span data-stu-id="3aefc-114">Provides a user-visible description of the item.</span></span> <span data-ttu-id="3aefc-115">Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="3aefc-115">Read-write.</span></span> <span data-ttu-id="3aefc-116">Somente no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="3aefc-116">Only on OneDrive Personal.</span></span>             |
|<span data-ttu-id="3aefc-117">**Tamanho**</span><span class="sxs-lookup"><span data-stu-id="3aefc-117">**fileSize**</span></span>      |<span data-ttu-id="3aefc-118">Int64</span><span class="sxs-lookup"><span data-stu-id="3aefc-118">Int64</span></span>                              | <span data-ttu-id="3aefc-119">Fornece um tamanho de arquivo esperado para executar uma verificação de cota antes do carregamento.</span><span class="sxs-lookup"><span data-stu-id="3aefc-119">Provides an expected file size to perform a quota check prior to upload.</span></span> <span data-ttu-id="3aefc-120">Somente no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="3aefc-120">Only on OneDrive Personal.</span></span> |
|<span data-ttu-id="3aefc-121">**fileSystemInfo**</span><span class="sxs-lookup"><span data-stu-id="3aefc-121">**fileSystemInfo**</span></span>|[<span data-ttu-id="3aefc-122">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="3aefc-122">fileSystemInfo</span></span>](filesysteminfo.md)| <span data-ttu-id="3aefc-123">File system information on client.</span><span class="sxs-lookup"><span data-stu-id="3aefc-123">File system information on client.</span></span> <span data-ttu-id="3aefc-124">Read-write.</span><span class="sxs-lookup"><span data-stu-id="3aefc-124">Read-write.</span></span>                                                      |
|<span data-ttu-id="3aefc-125">**name**</span><span class="sxs-lookup"><span data-stu-id="3aefc-125">**name**</span></span>          |<span data-ttu-id="3aefc-126">String</span><span class="sxs-lookup"><span data-stu-id="3aefc-126">String</span></span>                             | <span data-ttu-id="3aefc-127">The name of the item (filename and extension).</span><span class="sxs-lookup"><span data-stu-id="3aefc-127">The name of the item (filename and extension).</span></span> <span data-ttu-id="3aefc-128">Read-write.</span><span class="sxs-lookup"><span data-stu-id="3aefc-128">Read-write.</span></span>                                          |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "driveItemUploadableProperties resource",
  "keywords": "driveItemUploadableProperties,createUploadSession",
  "section": "documentation",
  "tocPath": ""
}-->
