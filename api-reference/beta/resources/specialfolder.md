---
author: JeremyKelley
description: O recurso SpecialFolder agrupa itens de dados relacionados a pastas especiais em uma única estrutura.
ms.date: 09/10/2017
title: SpecialFolder
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: a4ecce871115e92bfe91d5e6229c3ddd1a3c0472
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520335"
---
# <a name="specialfolder-resource-type"></a><span data-ttu-id="5665e-103">Tipo de recurso SpecialFolder</span><span class="sxs-lookup"><span data-stu-id="5665e-103">SpecialFolder resource type</span></span>

<span data-ttu-id="5665e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5665e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5665e-105">O recurso **SpecialFolder** agrupa itens de dados relacionados a pastas especiais em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="5665e-105">The **SpecialFolder** resource groups special folder-related data items into a single structure.</span></span>

<span data-ttu-id="5665e-106">Se um **DriveItem** tiver uma faceta **specialFolder** não nula, o item representará uma pasta especial (nomeada).</span><span class="sxs-lookup"><span data-stu-id="5665e-106">If a **DriveItem** has a non-null **specialFolder** facet, the item represents a special (named) folder.</span></span>
<span data-ttu-id="5665e-107">Pastas especiais que podem ser acessadas diretamente por meio da [coleção de pastas especiais](../api/drive-get-specialfolder.md).</span><span class="sxs-lookup"><span data-stu-id="5665e-107">Special folders can be accessed directly via the [special folders collection](../api/drive-get-specialfolder.md).</span></span>

<span data-ttu-id="5665e-p102">Pastas especiais fornecem aliases simples para acessar pastas conhecidas sem a necessidade de pesquisar a pasta pelo caminho (o que exigiria a localização) ou fazer referência à pasta com uma ID. Se uma pasta especial for renomeada ou movida para outro local na unidade de disco, esta sintaxe continuará a retornar a pasta.</span><span class="sxs-lookup"><span data-stu-id="5665e-p102">Special folders provide simple aliases to access well-known folders without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to return that folder.</span></span>

<span data-ttu-id="5665e-p103">As pastas especiais são criadas automaticamente na primeira vez que um aplicativo tenta gravar em uma, caso ainda não existam. Se um usuário excluir uma, ela será recriada quando algo for gravado nela novamente.</span><span class="sxs-lookup"><span data-stu-id="5665e-p103">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

<span data-ttu-id="5665e-112">**Observação:** Se seu aplicativo solicitou apenas o escopo **Files.Read** e solicitar uma pasta especial que não exista, a resposta será um erro `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="5665e-112">**Note:** If your app has only requested **Files.Read** scope and requests a special folder that doesn't exist, the response will be a `403 Forbidden` error.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5665e-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5665e-113">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="5665e-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5665e-114">Properties</span></span>

| <span data-ttu-id="5665e-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5665e-115">Property</span></span>  | <span data-ttu-id="5665e-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="5665e-116">Type</span></span>   | <span data-ttu-id="5665e-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="5665e-117">Description</span></span>                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| <span data-ttu-id="5665e-118">nome</span><span class="sxs-lookup"><span data-stu-id="5665e-118">name</span></span>      | <span data-ttu-id="5665e-119">string</span><span class="sxs-lookup"><span data-stu-id="5665e-119">string</span></span> | <span data-ttu-id="5665e-120">O identificador exclusivo deste item na coleção `/drive/special`</span><span class="sxs-lookup"><span data-stu-id="5665e-120">The unique identifier for this item in the `/drive/special` collection</span></span> |

## <a name="special-folders"></a><span data-ttu-id="5665e-121">Pastas especiais</span><span class="sxs-lookup"><span data-stu-id="5665e-121">Special folders</span></span>

<span data-ttu-id="5665e-122">Aqui estão as pastas especiais disponíveis no OneDrive Personal e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="5665e-122">Here are the special folders available in OneDrive Personal and OneDrive for Business.</span></span>

| <span data-ttu-id="5665e-123">Nome</span><span class="sxs-lookup"><span data-stu-id="5665e-123">Name</span></span>        | <span data-ttu-id="5665e-124">Id da pasta</span><span class="sxs-lookup"><span data-stu-id="5665e-124">Folder id</span></span>    | <span data-ttu-id="5665e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="5665e-125">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="5665e-126">Raiz de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5665e-126">App Root</span></span>    | `approot`    | <span data-ttu-id="5665e-p104">Pasta pessoal do aplicativo. Geralmente em `/Apps/{Application Name}`</span><span class="sxs-lookup"><span data-stu-id="5665e-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="5665e-129">Imagens da Câmera</span><span class="sxs-lookup"><span data-stu-id="5665e-129">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="5665e-p105">A pasta de Backup de Imagens da Câmera. Não disponível no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="5665e-p105">The Camera Roll Backup folder. Not available in OneDrive for Business.</span></span>   |
| <span data-ttu-id="5665e-132">Documentos</span><span class="sxs-lookup"><span data-stu-id="5665e-132">Documents</span></span>   | `documents`  | <span data-ttu-id="5665e-133">A pasta Documentos.</span><span class="sxs-lookup"><span data-stu-id="5665e-133">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="5665e-134">Música</span><span class="sxs-lookup"><span data-stu-id="5665e-134">Music</span></span>       | `music`      | <span data-ttu-id="5665e-p106">Pasta Música. Não disponível no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="5665e-p106">The Music folder. Not available in OneDrive for Business.</span></span>                |
| <span data-ttu-id="5665e-137">Fotos</span><span class="sxs-lookup"><span data-stu-id="5665e-137">Photos</span></span>      | `photos`     | <span data-ttu-id="5665e-138">A pasta Fotos.</span><span class="sxs-lookup"><span data-stu-id="5665e-138">The Photos folder.</span></span>                                                       |

## <a name="remarks"></a><span data-ttu-id="5665e-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="5665e-139">Remarks</span></span> 

<span data-ttu-id="5665e-140">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="5665e-140">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
