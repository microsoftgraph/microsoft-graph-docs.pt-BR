---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FileSystemInfo
ms.openlocfilehash: 9a5214f9c5e161de0be66ac634c7c5538b203772
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="filesysteminfo-facet"></a><span data-ttu-id="071d0-102">Faceta fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="071d0-102">FileSystemInfo facet</span></span>

<span data-ttu-id="071d0-103">O recurso **FileSystemInfo** contém propriedades que são relatadas pelo sistema de arquivos local do dispositivo para a versão local de um item.</span><span class="sxs-lookup"><span data-stu-id="071d0-103">The **FileSystemInfo** resource contains properties that are reported by the device's local file system for the local version of an item. This facet can be used to specify the last modified date or created date of the item as it was on the local device.</span></span>
<span data-ttu-id="071d0-104">Esta faceta pode ser usada para especificar a data da última modificação ou a data de criação do item como estava no dispositivo local.</span><span class="sxs-lookup"><span data-stu-id="071d0-104">The FileSystemInfo facet contains properties that are reported by the device's local file system for the local version of an item. This facet can be used to specify the last modified date or created date of the item as it was on the local device.</span></span>

<span data-ttu-id="071d0-105">Ele está disponível na propriedade fileSystemInfo dos recursos [driveItem] [ item-resource].</span><span class="sxs-lookup"><span data-stu-id="071d0-105">It is available on the fileSystemInfo property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="071d0-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="071d0-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="071d0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="071d0-107">Properties</span></span>

| <span data-ttu-id="071d0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="071d0-108">Property</span></span>                 | <span data-ttu-id="071d0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="071d0-109">Type</span></span>           | <span data-ttu-id="071d0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="071d0-110">Description</span></span>                                                                                                          |
| :----------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="071d0-111">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="071d0-111">**createdDateTime**</span></span>      | <span data-ttu-id="071d0-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="071d0-112">DateTimeOffset</span></span> | <span data-ttu-id="071d0-113">A data e a hora UTC da criação do arquivo em um cliente.</span><span class="sxs-lookup"><span data-stu-id="071d0-113">The UTC date and time the file was created on a client.</span></span>                                                              |
| <span data-ttu-id="071d0-114">**lastAccessedDateTime**</span><span class="sxs-lookup"><span data-stu-id="071d0-114">**lastAccessedDateTime**</span></span> | <span data-ttu-id="071d0-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="071d0-115">DateTimeOffset</span></span> | <span data-ttu-id="071d0-116">A data e hora UTC em que o arquivo foi acessado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="071d0-116">The UTC date and time the file was last accessed on a client.</span></span> <span data-ttu-id="071d0-117">Disponível para o [lista de arquivos recentes](../api/drive_recent.md) apenas.</span><span class="sxs-lookup"><span data-stu-id="071d0-117">Available for the [recent file list](../api/drive_recent.md) only.</span></span> |
| <span data-ttu-id="071d0-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="071d0-118">**lastModifiedDateTime**</span></span> | <span data-ttu-id="071d0-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="071d0-119">DateTimeOffset</span></span> | <span data-ttu-id="071d0-120">A data e hora UTC em que o arquivo foi modificado pela última vez em um cliente.</span><span class="sxs-lookup"><span data-stu-id="071d0-120">The UTC date and time the file was last modified on a client.</span></span>                                                        |

## <a name="notes"></a><span data-ttu-id="071d0-121">Observações</span><span class="sxs-lookup"><span data-stu-id="071d0-121">Notes</span></span>

<span data-ttu-id="071d0-122">Os valores para **createdDateTime** e **lastModifiedDateTime** variam em relação às mesmas propriedades no recurso [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="071d0-122">Values for **createdDateTime** and **lastModifiedDateTime** vary from the same properties on the [DriveItem](driveitem.md) resource.</span></span>
<span data-ttu-id="071d0-123">Os valores no recurso DriveItem são a data e a hora de criação e modificação, como visto do serviço.</span><span class="sxs-lookup"><span data-stu-id="071d0-123">The properties on the driveItem resource are the created and modified date and time from the perspective of when the service saw the file.</span></span>
<span data-ttu-id="071d0-124">Os valores armazenados no recurso **FileSystemInfo** são fornecidos pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="071d0-124">The values stored in the **FileSystemInfo** facet are provided by the client are are the values displayed to the user if they exist.</span></span>

<span data-ttu-id="071d0-125">Por exemplo, se um arquivo foi criado no dispositivo na segunda-feira, mas não foi carregado no serviço até terça-feira, o cliente que carrega o arquivo deve gravar a faceta `fileSystemInfo` para incluir a data de criação na segunda-feira.</span><span class="sxs-lookup"><span data-stu-id="071d0-125">For example, if a file was created on the device on Monday, but not uploaded to the service until Tuesday, the client that uploads the file should write the `fileSystemInfo` facet to include the created date on Monday. When the item metadata is retrieved, the created date for the item will reflect Tuesday, but the  facet will show the original created date on Monday.</span></span> <span data-ttu-id="071d0-126">Quando os metadados de item forem recuperados, a data de criação do item refletirá terça-feira, mas a faceta `fileSystemInfo` mostrará a data de criação original na segunda-feira.</span><span class="sxs-lookup"><span data-stu-id="071d0-126">When the item metadata is retrieved, the created date for the item will reflect Tuesday, but the `fileSystemInfo` facet will show the original created date on Monday.</span></span>

<span data-ttu-id="071d0-p105">Estas propriedades são somente leitura. Se estiver carregando um arquivo e souber os valores do cliente local para estes campos, você deverá incluí-los na solicitação.</span><span class="sxs-lookup"><span data-stu-id="071d0-p105">These properties are read/write. If you are uploading a file and know the local client values for these fields, you should include them in the request.</span></span>

<span data-ttu-id="071d0-129">Se o conteúdo do arquivo for atualizado e estas propriedades não forem fornecidas, **lastModifiedDateTime** será redefinido automaticamente como a hora atual.</span><span class="sxs-lookup"><span data-stu-id="071d0-129">If the file's content is updated and these properties are not provided, **lastModifiedDateTime** automatically resets to the current time.</span></span>

## <a name="remarks"></a><span data-ttu-id="071d0-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="071d0-130">Remarks</span></span>

* <span data-ttu-id="071d0-131">**lastAccessedDateTime** não está disponível para itens no SharePoint Online ou OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="071d0-131">**lastAccessedDateTime** is not available for items in SharePoint online, OneDrive for Business, or SharePoint Server 2016.</span></span>

<span data-ttu-id="071d0-132">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="071d0-132">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The fileSystemInfo facet provides information about date created and modified by clients.",
  "keywords": "fileSystemInfo,client,system info,onedrive",
  "section": "documentation",
  "tocPath": "Facets/FileSystemInfo"
} -->
