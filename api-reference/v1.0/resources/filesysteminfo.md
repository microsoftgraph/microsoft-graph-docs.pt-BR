---
author: JeremyKelley
ms.date: 09/10/2017
title: FileSystemInfo
localization_priority: Normal
description: O recurso FileSystemInfo contém propriedades que são relatadas pelo sistema de arquivos local do dispositivo para a versão local de um item.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f080e6222555f2bc9fcea8cb8a3a157a8e2eb096
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240056"
---
# <a name="filesysteminfo-facet"></a><span data-ttu-id="712a4-103">Faceta fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="712a4-103">FileSystemInfo facet</span></span>

<span data-ttu-id="712a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="712a4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="712a4-p101">O recurso **FileSystemInfo** contém propriedades que são relatadas pelo sistema de arquivos local do dispositivo para a versão local de um item. Esta faceta pode ser usada para especificar a data da última modificação ou a data de criação do item como estava no dispositivo local.</span><span class="sxs-lookup"><span data-stu-id="712a4-p101">The **FileSystemInfo** resource contains properties that are reported by the device's local file system for the local version of an item. This facet can be used to specify the last modified date or created date of the item as it was on the local device.</span></span>

<span data-ttu-id="712a4-107">Ele está disponível na propriedade fileSystemInfo dos [recursos driveItem.][item-resource]</span><span class="sxs-lookup"><span data-stu-id="712a4-107">It is available on the fileSystemInfo property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="712a4-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="712a4-108">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "lastAccessedDateTime"
  ],
  "@odata.type": "microsoft.graph.fileSystemInfo"
}-->

```json
{
  "createdDateTime" : "datetime",
  "lastAccessedDateTime": "datetime",
  "lastModifiedDateTime" : "datetime"
}
```

## <a name="properties"></a><span data-ttu-id="712a4-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="712a4-109">Properties</span></span>

| <span data-ttu-id="712a4-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="712a4-110">Property</span></span>                 | <span data-ttu-id="712a4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="712a4-111">Type</span></span>           | <span data-ttu-id="712a4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="712a4-112">Description</span></span>                                                                                                          |
| :----------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="712a4-113">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="712a4-113">**createdDateTime**</span></span>      | <span data-ttu-id="712a4-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="712a4-114">DateTimeOffset</span></span> | <span data-ttu-id="712a4-115">A data e a hora UTC da criação do arquivo em um cliente.</span><span class="sxs-lookup"><span data-stu-id="712a4-115">The UTC date and time the file was created on a client.</span></span>                                                              |
| <span data-ttu-id="712a4-116">**lastAccessedDateTime**</span><span class="sxs-lookup"><span data-stu-id="712a4-116">**lastAccessedDateTime**</span></span> | <span data-ttu-id="712a4-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="712a4-117">DateTimeOffset</span></span> | <span data-ttu-id="712a4-118">A data e hora UTC em que o arquivo foi acessado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="712a4-118">The UTC date and time the file was last accessed.</span></span> <span data-ttu-id="712a4-119">Disponível para o [lista de arquivos recentes](../api/drive-recent.md) apenas.</span><span class="sxs-lookup"><span data-stu-id="712a4-119">Available for the [recent file list](../api/drive-recent.md) only.</span></span> |
| <span data-ttu-id="712a4-120">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="712a4-120">**lastModifiedDateTime**</span></span> | <span data-ttu-id="712a4-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="712a4-121">DateTimeOffset</span></span> | <span data-ttu-id="712a4-122">A data e hora UTC em que o arquivo foi modificado pela última vez em um cliente.</span><span class="sxs-lookup"><span data-stu-id="712a4-122">The UTC date and time the file was last modified on a client.</span></span>                                                        |

## <a name="notes"></a><span data-ttu-id="712a4-123">Observações</span><span class="sxs-lookup"><span data-stu-id="712a4-123">Notes</span></span>

<span data-ttu-id="712a4-p103">Os valores para **createdDateTime** e **lastModifiedDateTime** variam em relação às mesmas propriedades no recurso [DriveItem](driveitem.md). Os valores no recurso DriveItem são a data e a hora de criação e modificação, como visto do serviço. Os valores armazenados no recurso **FileSystemInfo** são fornecidos pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="712a4-p103">Values for **createdDateTime** and **lastModifiedDateTime** vary from the same properties on the [DriveItem](driveitem.md) resource. The values on the DriveItem resource are the created and modified date and time as seen from the service. The values stored in the **FileSystemInfo** resource are provided by the client.</span></span>

<span data-ttu-id="712a4-p104">Por exemplo, se um arquivo foi criado no dispositivo na segunda-feira, mas não foi carregado no serviço até terça-feira, o cliente que carrega o arquivo deve gravar a faceta `fileSystemInfo` para incluir a data de criação na segunda-feira. Quando os metadados de item forem recuperados, a data de criação do item refletirá terça-feira, mas a faceta `fileSystemInfo` mostrará a data de criação original na segunda-feira.</span><span class="sxs-lookup"><span data-stu-id="712a4-p104">For example, if a file was created on the device on Monday, but not uploaded to the service until Tuesday, the client that uploads the file should write the `fileSystemInfo` facet to include the created date on Monday. When the item metadata is retrieved, the created date for the item will reflect Tuesday, but the `fileSystemInfo` facet will show the original created date on Monday.</span></span>

<span data-ttu-id="712a4-p105">Estas propriedades são somente leitura. Se estiver carregando um arquivo e souber os valores do cliente local para estes campos, você deverá incluí-los na solicitação.</span><span class="sxs-lookup"><span data-stu-id="712a4-p105">These properties are read/write. If you are uploading a file and know the local client values for these fields, you should include them in the request.</span></span>

<span data-ttu-id="712a4-131">Se o conteúdo do arquivo for atualizado e estas propriedades não forem fornecidas, **lastModifiedDateTime** será redefinido automaticamente como a hora atual.</span><span class="sxs-lookup"><span data-stu-id="712a4-131">If the file's content is updated and these properties are not provided, **lastModifiedDateTime** automatically resets to the current time.</span></span>

## <a name="remarks"></a><span data-ttu-id="712a4-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="712a4-132">Remarks</span></span>

* <span data-ttu-id="712a4-133">**lastAccessedDateTime** não está disponível para itens no SharePoint Online ou OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="712a4-133">**lastAccessedDateTime** is not available for items in SharePoint online or OneDrive for Business.</span></span>

<span data-ttu-id="712a4-134">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="712a4-134">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The fileSystemInfo facet provides information about date created and modified by clients.",
  "keywords": "fileSystemInfo,client,system info,onedrive",
  "section": "documentation",
  "tocPath": "Facets/FileSystemInfo"
} -->

