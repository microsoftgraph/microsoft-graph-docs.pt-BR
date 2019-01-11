---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SpecialFolder
localization_priority: Normal
ms.openlocfilehash: 4c1facae90ea8981b1e83087d11e2d81a0354617
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820094"
---
# <a name="specialfolder-resource-type"></a><span data-ttu-id="32271-102">Tipo de recurso SpecialFolder</span><span class="sxs-lookup"><span data-stu-id="32271-102">SpecialFolder resource type</span></span>

<span data-ttu-id="32271-103">O recurso **SpecialFolder** agrupa itens de dados relacionados a pastas especiais em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="32271-103">The **SpecialFolder** resource groups special folder-related data items into a single structure.</span></span>

<span data-ttu-id="32271-104">Se um **DriveItem** tiver uma faceta **specialFolder** não nula, o item representará uma pasta especial (nomeada).</span><span class="sxs-lookup"><span data-stu-id="32271-104">If a **DriveItem** has a non-null **specialFolder** facet, the item represents a special (named) folder.</span></span>
<span data-ttu-id="32271-105">Pastas especiais que podem ser acessadas diretamente por meio da [coleção de pastas especiais](../api/drive-get-specialfolder.md).</span><span class="sxs-lookup"><span data-stu-id="32271-105">Special folders can be accessed directly via the [special folders collection](../api/drive-get-specialfolder.md).</span></span>

<span data-ttu-id="32271-p102">Pastas especiais fornecem aliases simples para acessar pastas conhecidas sem a necessidade de pesquisar a pasta pelo caminho (o que exigiria a localização) ou fazer referência à pasta com uma ID. Se uma pasta especial for renomeada ou movida para outro local na unidade de disco, esta sintaxe continuará a retornar a pasta.</span><span class="sxs-lookup"><span data-stu-id="32271-p102">Special folders provide simple aliases to access well-known folders without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to return that folder.</span></span>

<span data-ttu-id="32271-p103">As pastas especiais são criadas automaticamente na primeira vez que um aplicativo tenta gravar em uma, caso ainda não existam. Se um usuário excluir uma, ela será recriada quando algo for gravado nela novamente.</span><span class="sxs-lookup"><span data-stu-id="32271-p103">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

<span data-ttu-id="32271-110">**Observação:** Se seu aplicativo solicitou apenas o escopo **Files.Read** e solicitar uma pasta especial que não exista, a resposta será um erro `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="32271-110">**Note:** If your app has only requested **Files.Read** scope and requests a special folder that doesn't exist, the response will be a `403 Forbidden` error.</span></span>

## <a name="json-representation"></a><span data-ttu-id="32271-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32271-111">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.specialFolder"
}-->
```json
{
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="32271-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32271-112">Properties</span></span>

| <span data-ttu-id="32271-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32271-113">Property</span></span>  | <span data-ttu-id="32271-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="32271-114">Type</span></span>   | <span data-ttu-id="32271-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="32271-115">Description</span></span>                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| <span data-ttu-id="32271-116">name</span><span class="sxs-lookup"><span data-stu-id="32271-116">name</span></span>      | <span data-ttu-id="32271-117">string</span><span class="sxs-lookup"><span data-stu-id="32271-117">string</span></span> | <span data-ttu-id="32271-118">O identificador exclusivo deste item na coleção `/drive/special`</span><span class="sxs-lookup"><span data-stu-id="32271-118">The unique identifier for this item in the `/drive/special` collection</span></span> |

## <a name="special-folders"></a><span data-ttu-id="32271-119">Pastas especiais</span><span class="sxs-lookup"><span data-stu-id="32271-119">Special folders</span></span>

<span data-ttu-id="32271-120">Aqui estão as pastas especiais disponíveis no OneDrive Personal e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="32271-120">Here are the special folders available in OneDrive Personal and OneDrive for Business.</span></span>

| <span data-ttu-id="32271-121">Nome</span><span class="sxs-lookup"><span data-stu-id="32271-121">Name</span></span>        | <span data-ttu-id="32271-122">Id da pasta</span><span class="sxs-lookup"><span data-stu-id="32271-122">Folder id</span></span>    | <span data-ttu-id="32271-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="32271-123">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="32271-124">Raiz de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32271-124">App Root</span></span>    | `approot`    | <span data-ttu-id="32271-p104">Pasta pessoal do aplicativo. Geralmente em `/Apps/{Application Name}`</span><span class="sxs-lookup"><span data-stu-id="32271-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="32271-127">Imagens da Câmera</span><span class="sxs-lookup"><span data-stu-id="32271-127">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="32271-p105">A pasta de Backup de Imagens da Câmera. Não disponível no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="32271-p105">The Camera Roll Backup folder. Not available in OneDrive for Business.</span></span>   |
| <span data-ttu-id="32271-130">Documentos</span><span class="sxs-lookup"><span data-stu-id="32271-130">Documents</span></span>   | `documents`  | <span data-ttu-id="32271-131">A pasta Documentos.</span><span class="sxs-lookup"><span data-stu-id="32271-131">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="32271-132">Música</span><span class="sxs-lookup"><span data-stu-id="32271-132">Music</span></span>       | `music`      | <span data-ttu-id="32271-p106">Pasta Música. Não disponível no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="32271-p106">The Music folder. Not available in OneDrive for Business.</span></span>                |
| <span data-ttu-id="32271-135">Fotos</span><span class="sxs-lookup"><span data-stu-id="32271-135">Photos</span></span>      | `photos`     | <span data-ttu-id="32271-136">A pasta Fotos.</span><span class="sxs-lookup"><span data-stu-id="32271-136">The Photos folder.</span></span>                                                       |

## <a name="remarks"></a><span data-ttu-id="32271-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="32271-137">Remarks</span></span> 

<span data-ttu-id="32271-138">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="32271-138">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SpecialFolder"
} -->
