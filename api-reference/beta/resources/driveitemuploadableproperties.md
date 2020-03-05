---
title: tipo de recurso driveItemUploadableProperties
description: O recurso driveItemUploadableProperties representa um item sendo carregado durante a criação de uma sessão de carregamento.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a68180476910051dc3633ee5dce7363c77eb60ae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505557"
---
# <a name="driveitemuploadableproperties-resource-type"></a><span data-ttu-id="70aea-103">tipo de recurso driveItemUploadableProperties</span><span class="sxs-lookup"><span data-stu-id="70aea-103">driveItemUploadableProperties resource type</span></span>

<span data-ttu-id="70aea-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="70aea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70aea-105">O recurso **driveItemUploadableProperties** representa um item sendo carregado durante [a criação de uma sessão de carregamento](../api/driveitem-createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="70aea-105">The **driveItemUploadableProperties** resource represents an item being uploaded when [creating an upload session](../api/driveitem-createuploadsession.md).</span></span>

## <a name="properties"></a><span data-ttu-id="70aea-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70aea-106">Properties</span></span>

| <span data-ttu-id="70aea-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70aea-107">Property</span></span>     | <span data-ttu-id="70aea-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="70aea-108">Type</span></span>                              | <span data-ttu-id="70aea-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="70aea-109">Description</span></span>                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|<span data-ttu-id="70aea-110">description</span><span class="sxs-lookup"><span data-stu-id="70aea-110">description</span></span>   |<span data-ttu-id="70aea-111">String</span><span class="sxs-lookup"><span data-stu-id="70aea-111">String</span></span>                             | <span data-ttu-id="70aea-112">Fornece uma descrição do item visível para o usuário.</span><span class="sxs-lookup"><span data-stu-id="70aea-112">Provides a user-visible description of the item.</span></span> <span data-ttu-id="70aea-113">Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="70aea-113">Read-write.</span></span> <span data-ttu-id="70aea-114">Somente no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="70aea-114">Only on OneDrive Personal.</span></span>             |
|<span data-ttu-id="70aea-115">Tamanho</span><span class="sxs-lookup"><span data-stu-id="70aea-115">fileSize</span></span>      |<span data-ttu-id="70aea-116">Int64</span><span class="sxs-lookup"><span data-stu-id="70aea-116">Int64</span></span>                              | <span data-ttu-id="70aea-117">Fornece um tamanho de arquivo esperado para executar uma verificação de cota antes do carregamento.</span><span class="sxs-lookup"><span data-stu-id="70aea-117">Provides an expected file size to perform a quota check prior to upload.</span></span> <span data-ttu-id="70aea-118">Somente no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="70aea-118">Only on OneDrive Personal.</span></span> |
|<span data-ttu-id="70aea-119">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="70aea-119">fileSystemInfo</span></span>|[<span data-ttu-id="70aea-120">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="70aea-120">fileSystemInfo</span></span>](filesysteminfo.md)| <span data-ttu-id="70aea-p103">Informações do sistema de arquivos no cliente. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="70aea-p103">File system information on client. Read-write.</span></span>                                                      |
|<span data-ttu-id="70aea-123">name</span><span class="sxs-lookup"><span data-stu-id="70aea-123">name</span></span>          |<span data-ttu-id="70aea-124">String</span><span class="sxs-lookup"><span data-stu-id="70aea-124">String</span></span>                             | <span data-ttu-id="70aea-p104">O nome do item (nome do arquivo e extensão). Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="70aea-p104">The name of the item (filename and extension). Read-write.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="70aea-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70aea-127">JSON representation</span></span>

<span data-ttu-id="70aea-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="70aea-128">The following is a JSON representation of the resource.</span></span>

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