---
title: tipo de recurso driveItemUploadableProperties
description: O recurso driveItemUploadableProperties representa um item sendo carregado durante a criação de uma sessão de carregamento.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f8511bba850c1d165fe9b7082b7df51900b17962
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333386"
---
# <a name="driveitemuploadableproperties-resource-type"></a><span data-ttu-id="edc25-103">tipo de recurso driveItemUploadableProperties</span><span class="sxs-lookup"><span data-stu-id="edc25-103">driveItemUploadableProperties resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edc25-104">O recurso **driveItemUploadableProperties** representa um item sendo carregado durante [a criação de uma sessão de carregamento](../api/driveitem-createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="edc25-104">The **driveItemUploadableProperties** resource represents an item being uploaded when [creating an upload session](../api/driveitem-createuploadsession.md).</span></span>

## <a name="properties"></a><span data-ttu-id="edc25-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="edc25-105">Properties</span></span>

| <span data-ttu-id="edc25-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="edc25-106">Property</span></span>     | <span data-ttu-id="edc25-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="edc25-107">Type</span></span>                              | <span data-ttu-id="edc25-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="edc25-108">Description</span></span>                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|<span data-ttu-id="edc25-109">description</span><span class="sxs-lookup"><span data-stu-id="edc25-109">description</span></span>   |<span data-ttu-id="edc25-110">String</span><span class="sxs-lookup"><span data-stu-id="edc25-110">String</span></span>                             | <span data-ttu-id="edc25-111">Fornece uma descrição do item visível para o usuário.</span><span class="sxs-lookup"><span data-stu-id="edc25-111">Provides a user-visible description of the item.</span></span> <span data-ttu-id="edc25-112">Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="edc25-112">Read-write.</span></span> <span data-ttu-id="edc25-113">Somente no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="edc25-113">Only on OneDrive Personal.</span></span>             |
|<span data-ttu-id="edc25-114">Tamanho</span><span class="sxs-lookup"><span data-stu-id="edc25-114">fileSize</span></span>      |<span data-ttu-id="edc25-115">Int64</span><span class="sxs-lookup"><span data-stu-id="edc25-115">Int64</span></span>                              | <span data-ttu-id="edc25-116">Fornece um tamanho de arquivo esperado para executar uma verificação de cota antes do carregamento.</span><span class="sxs-lookup"><span data-stu-id="edc25-116">Provides an expected file size to perform a quota check prior to upload.</span></span> <span data-ttu-id="edc25-117">Somente no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="edc25-117">Only on OneDrive Personal.</span></span> |
|<span data-ttu-id="edc25-118">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="edc25-118">fileSystemInfo</span></span>|[<span data-ttu-id="edc25-119">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="edc25-119">fileSystemInfo</span></span>](filesysteminfo.md)| <span data-ttu-id="edc25-p103">Informações do sistema de arquivos no cliente. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="edc25-p103">File system information on client. Read-write.</span></span>                                                      |
|<span data-ttu-id="edc25-122">name</span><span class="sxs-lookup"><span data-stu-id="edc25-122">name</span></span>          |<span data-ttu-id="edc25-123">String</span><span class="sxs-lookup"><span data-stu-id="edc25-123">String</span></span>                             | <span data-ttu-id="edc25-p104">O nome do item (nome do arquivo e extensão). Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="edc25-p104">The name of the item (filename and extension). Read-write.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="edc25-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="edc25-126">JSON representation</span></span>

<span data-ttu-id="edc25-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="edc25-127">The following is a JSON representation of the resource.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "driveItemUploadableProperties resource",
  "keywords": "driveItemUploadableProperties,createUploadSession",
  "section": "documentation",
  "tocPath": ""
}-->