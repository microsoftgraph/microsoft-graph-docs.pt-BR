---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SpecialFolder
localization_priority: Normal
ms.openlocfilehash: ff1bee4ce71bf76c94951d298f80db74609710e6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582273"
---
# <a name="specialfolder-resource-type"></a><span data-ttu-id="a9250-102">Tipo de recurso SpecialFolder</span><span class="sxs-lookup"><span data-stu-id="a9250-102">SpecialFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9250-103">O recurso **SpecialFolder** agrupa itens de dados relacionados a pastas especiais em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="a9250-103">The **SpecialFolder** resource groups special folder-related data items into a single structure.</span></span>

<span data-ttu-id="a9250-104">Se um **DriveItem** tiver uma faceta **specialFolder** não nula, o item representará uma pasta especial (nomeada).</span><span class="sxs-lookup"><span data-stu-id="a9250-104">If a **DriveItem** has a non-null **specialFolder** facet, the item represents a special (named) folder.</span></span>
<span data-ttu-id="a9250-105">Pastas especiais que podem ser acessadas diretamente por meio da [coleção de pastas especiais](../api/drive-get-specialfolder.md).</span><span class="sxs-lookup"><span data-stu-id="a9250-105">Special folders can be accessed directly via the [special folders collection](../api/drive-get-specialfolder.md).</span></span>

<span data-ttu-id="a9250-p102">Pastas especiais fornecem aliases simples para acessar pastas conhecidas sem a necessidade de pesquisar a pasta pelo caminho (o que exigiria a localização) ou fazer referência à pasta com uma ID. Se uma pasta especial for renomeada ou movida para outro local na unidade de disco, esta sintaxe continuará a retornar a pasta.</span><span class="sxs-lookup"><span data-stu-id="a9250-p102">Special folders provide simple aliases to access well-known folders without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to return that folder.</span></span>

<span data-ttu-id="a9250-p103">As pastas especiais são criadas automaticamente na primeira vez que um aplicativo tenta gravar em uma, caso ainda não existam. Se um usuário excluir uma, ela será recriada quando algo for gravado nela novamente.</span><span class="sxs-lookup"><span data-stu-id="a9250-p103">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

<span data-ttu-id="a9250-110">**Observação:** Se seu aplicativo solicitou apenas o escopo **Files.Read** e solicitar uma pasta especial que não exista, a resposta será um erro `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="a9250-110">**Note:** If your app has only requested **Files.Read** scope and requests a special folder that doesn't exist, the response will be a `403 Forbidden` error.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9250-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9250-111">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="a9250-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9250-112">Properties</span></span>

| <span data-ttu-id="a9250-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9250-113">Property</span></span>  | <span data-ttu-id="a9250-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9250-114">Type</span></span>   | <span data-ttu-id="a9250-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9250-115">Description</span></span>                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| <span data-ttu-id="a9250-116">name</span><span class="sxs-lookup"><span data-stu-id="a9250-116">name</span></span>      | <span data-ttu-id="a9250-117">string</span><span class="sxs-lookup"><span data-stu-id="a9250-117">string</span></span> | <span data-ttu-id="a9250-118">O identificador exclusivo deste item na coleção `/drive/special`</span><span class="sxs-lookup"><span data-stu-id="a9250-118">The unique identifier for this item in the `/drive/special` collection</span></span> |

## <a name="special-folders"></a><span data-ttu-id="a9250-119">Pastas especiais</span><span class="sxs-lookup"><span data-stu-id="a9250-119">Special folders</span></span>

<span data-ttu-id="a9250-120">Aqui estão as pastas especiais disponíveis no OneDrive Personal e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="a9250-120">Here are the special folders available in OneDrive Personal and OneDrive for Business.</span></span>

| <span data-ttu-id="a9250-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a9250-121">Name</span></span>        | <span data-ttu-id="a9250-122">Id da pasta</span><span class="sxs-lookup"><span data-stu-id="a9250-122">Folder id</span></span>    | <span data-ttu-id="a9250-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9250-123">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="a9250-124">Raiz de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9250-124">App Root</span></span>    | `approot`    | <span data-ttu-id="a9250-p104">Pasta pessoal do aplicativo. Geralmente em `/Apps/{Application Name}`</span><span class="sxs-lookup"><span data-stu-id="a9250-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="a9250-127">Imagens da Câmera</span><span class="sxs-lookup"><span data-stu-id="a9250-127">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="a9250-p105">A pasta de Backup de Imagens da Câmera. Não disponível no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="a9250-p105">The Camera Roll Backup folder. Not available in OneDrive for Business.</span></span>   |
| <span data-ttu-id="a9250-130">Documentos</span><span class="sxs-lookup"><span data-stu-id="a9250-130">Documents</span></span>   | `documents`  | <span data-ttu-id="a9250-131">A pasta Documentos.</span><span class="sxs-lookup"><span data-stu-id="a9250-131">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="a9250-132">Música</span><span class="sxs-lookup"><span data-stu-id="a9250-132">Music</span></span>       | `music`      | <span data-ttu-id="a9250-p106">Pasta Música. Não disponível no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="a9250-p106">The Music folder. Not available in OneDrive for Business.</span></span>                |
| <span data-ttu-id="a9250-135">Fotos</span><span class="sxs-lookup"><span data-stu-id="a9250-135">Photos</span></span>      | `photos`     | <span data-ttu-id="a9250-136">A pasta Fotos.</span><span class="sxs-lookup"><span data-stu-id="a9250-136">The Photos folder.</span></span>                                                       |

## <a name="remarks"></a><span data-ttu-id="a9250-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="a9250-137">Remarks</span></span> 

<span data-ttu-id="a9250-138">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="a9250-138">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/specialfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
