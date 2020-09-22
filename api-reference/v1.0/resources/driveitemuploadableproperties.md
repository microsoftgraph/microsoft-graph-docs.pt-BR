---
title: tipo de recurso driveItemUploadableProperties
description: O recurso driveItemUploadableProperties representa um item sendo carregado durante a criação de uma sessão de carregamento.
localization_priority: Normal
author: JeremyKelley
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: c05c69f0cf72f74913882ddbf75355dc37592584
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032716"
---
# <a name="driveitemuploadableproperties-resource-type"></a><span data-ttu-id="c15df-103">tipo de recurso driveItemUploadableProperties</span><span class="sxs-lookup"><span data-stu-id="c15df-103">driveItemUploadableProperties resource type</span></span>

<span data-ttu-id="c15df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c15df-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c15df-105">Representa um item que está sendo carregado ao [criar uma sessão de carregamento](../api/driveitem-createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="c15df-105">Represents an item being uploaded when [creating an upload session](../api/driveitem-createuploadsession.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="c15df-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c15df-106">JSON representation</span></span>

<span data-ttu-id="c15df-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c15df-107">The following is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="c15df-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c15df-108">Properties</span></span>

| <span data-ttu-id="c15df-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c15df-109">Property</span></span>     | <span data-ttu-id="c15df-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c15df-110">Type</span></span>                              | <span data-ttu-id="c15df-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c15df-111">Description</span></span>                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|<span data-ttu-id="c15df-112">**description**</span><span class="sxs-lookup"><span data-stu-id="c15df-112">**description**</span></span>   |<span data-ttu-id="c15df-113">String</span><span class="sxs-lookup"><span data-stu-id="c15df-113">String</span></span>                             | <span data-ttu-id="c15df-114">Fornece uma descrição do item visível para o usuário.</span><span class="sxs-lookup"><span data-stu-id="c15df-114">Provides a user-visible description of the item.</span></span> <span data-ttu-id="c15df-115">Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="c15df-115">Read-write.</span></span> <span data-ttu-id="c15df-116">Somente no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="c15df-116">Only on OneDrive Personal.</span></span>             |
|<span data-ttu-id="c15df-117">**Tamanho**</span><span class="sxs-lookup"><span data-stu-id="c15df-117">**fileSize**</span></span>      |<span data-ttu-id="c15df-118">Int64</span><span class="sxs-lookup"><span data-stu-id="c15df-118">Int64</span></span>                              | <span data-ttu-id="c15df-119">Fornece um tamanho de arquivo esperado para executar uma verificação de cota antes do carregamento.</span><span class="sxs-lookup"><span data-stu-id="c15df-119">Provides an expected file size to perform a quota check prior to upload.</span></span> <span data-ttu-id="c15df-120">Somente no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="c15df-120">Only on OneDrive Personal.</span></span> |
|<span data-ttu-id="c15df-121">**fileSystemInfo**</span><span class="sxs-lookup"><span data-stu-id="c15df-121">**fileSystemInfo**</span></span>|[<span data-ttu-id="c15df-122">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="c15df-122">fileSystemInfo</span></span>](filesysteminfo.md)| <span data-ttu-id="c15df-p103">Informações do sistema de arquivos no cliente. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="c15df-p103">File system information on client. Read-write.</span></span>                                                      |
|<span data-ttu-id="c15df-125">**name**</span><span class="sxs-lookup"><span data-stu-id="c15df-125">**name**</span></span>          |<span data-ttu-id="c15df-126">String</span><span class="sxs-lookup"><span data-stu-id="c15df-126">String</span></span>                             | <span data-ttu-id="c15df-p104">O nome do item (nome do arquivo e extensão). Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="c15df-p104">The name of the item (filename and extension). Read-write.</span></span>                                          |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "driveItemUploadableProperties resource",
  "keywords": "driveItemUploadableProperties,createUploadSession",
  "section": "documentation",
  "tocPath": ""
}-->

