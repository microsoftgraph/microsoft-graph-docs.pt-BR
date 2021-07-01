---
title: Tipo de recurso driveItemUploadableProperties
description: O recurso driveItemUploadableProperties representa um item sendo carregado ao criar uma sessão de carregamento.
localization_priority: Normal
author: JeremyKelley
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 6c00270f1e86e2bb8f44af36c6c514c9b80a647d
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236205"
---
# <a name="driveitemuploadableproperties-resource-type"></a><span data-ttu-id="44722-103">Tipo de recurso driveItemUploadableProperties</span><span class="sxs-lookup"><span data-stu-id="44722-103">driveItemUploadableProperties resource type</span></span>

<span data-ttu-id="44722-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44722-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44722-105">O **recurso driveItemUploadableProperties** representa um item que está sendo carregado ao [criar uma sessão de carregamento.](../api/driveitem-createuploadsession.md)</span><span class="sxs-lookup"><span data-stu-id="44722-105">The **driveItemUploadableProperties** resource represents an item being uploaded when [creating an upload session](../api/driveitem-createuploadsession.md).</span></span>

## <a name="properties"></a><span data-ttu-id="44722-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44722-106">Properties</span></span>

| <span data-ttu-id="44722-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44722-107">Property</span></span>     | <span data-ttu-id="44722-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="44722-108">Type</span></span>                              | <span data-ttu-id="44722-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="44722-109">Description</span></span>                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|<span data-ttu-id="44722-110">description</span><span class="sxs-lookup"><span data-stu-id="44722-110">description</span></span>   |<span data-ttu-id="44722-111">String</span><span class="sxs-lookup"><span data-stu-id="44722-111">String</span></span>                             | <span data-ttu-id="44722-112">Fornece uma descrição do item visível para o usuário.</span><span class="sxs-lookup"><span data-stu-id="44722-112">Provides a user-visible description of the item.</span></span> <span data-ttu-id="44722-113">Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="44722-113">Read-write.</span></span> <span data-ttu-id="44722-114">Somente no OneDrive Pessoal.</span><span class="sxs-lookup"><span data-stu-id="44722-114">Only on OneDrive Personal.</span></span>             |
|<span data-ttu-id="44722-115">driveItemSource</span><span class="sxs-lookup"><span data-stu-id="44722-115">driveItemSource</span></span>| [<span data-ttu-id="44722-116">driveItemSource</span><span class="sxs-lookup"><span data-stu-id="44722-116">driveItemSource</span></span>](driveItemSource.md)              | <span data-ttu-id="44722-117">Informações sobre a fonte do item da unidade.</span><span class="sxs-lookup"><span data-stu-id="44722-117">Information about the drive item source.</span></span> <span data-ttu-id="44722-118">Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="44722-118">Read-write.</span></span> <span data-ttu-id="44722-119">Somente em OneDrive for Business e SharePoint.</span><span class="sxs-lookup"><span data-stu-id="44722-119">Only on OneDrive for Business and SharePoint.</span></span>  |
|<span data-ttu-id="44722-120">fileSize</span><span class="sxs-lookup"><span data-stu-id="44722-120">fileSize</span></span>      |<span data-ttu-id="44722-121">Int64</span><span class="sxs-lookup"><span data-stu-id="44722-121">Int64</span></span>                              | <span data-ttu-id="44722-122">Fornece um tamanho de arquivo esperado para executar uma verificação de cota antes de carregar.</span><span class="sxs-lookup"><span data-stu-id="44722-122">Provides an expected file size to perform a quota check prior to upload.</span></span> <span data-ttu-id="44722-123">Somente no OneDrive Pessoal.</span><span class="sxs-lookup"><span data-stu-id="44722-123">Only on OneDrive Personal.</span></span> |
|<span data-ttu-id="44722-124">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="44722-124">fileSystemInfo</span></span>|[<span data-ttu-id="44722-125">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="44722-125">fileSystemInfo</span></span>](filesysteminfo.md)| <span data-ttu-id="44722-p104">Informações do sistema de arquivos no cliente. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="44722-p104">File system information on client. Read-write.</span></span>                                                      |
|<span data-ttu-id="44722-128">mediaSource</span><span class="sxs-lookup"><span data-stu-id="44722-128">mediaSource</span></span>  | [<span data-ttu-id="44722-129">mediaSource</span><span class="sxs-lookup"><span data-stu-id="44722-129">mediaSource</span></span>](mediaSource.md)                    | <span data-ttu-id="44722-130">Informações de origem de mídia.</span><span class="sxs-lookup"><span data-stu-id="44722-130">Media source information.</span></span> <span data-ttu-id="44722-131">Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="44722-131">Read-write.</span></span> <span data-ttu-id="44722-132">Somente em OneDrive for Business e SharePoint.</span><span class="sxs-lookup"><span data-stu-id="44722-132">Only on OneDrive for Business and SharePoint.</span></span>                 |
|<span data-ttu-id="44722-133">nome</span><span class="sxs-lookup"><span data-stu-id="44722-133">name</span></span>          |<span data-ttu-id="44722-134">String</span><span class="sxs-lookup"><span data-stu-id="44722-134">String</span></span>                             | <span data-ttu-id="44722-p106">O nome do item (nome do arquivo e extensão). Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="44722-p106">The name of the item (filename and extension). Read-write.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="44722-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44722-137">JSON representation</span></span>

<span data-ttu-id="44722-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="44722-138">The following is a JSON representation of the resource.</span></span>

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

