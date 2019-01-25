---
title: tipo de recurso de mailSearchFolder
description: Um mailSearchFolder é uma pasta virtual na caixa de correio do usuário que contém todos os itens de email que correspondam a critérios de pesquisa especificado. mailSearchFolder herda de mailFolder.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ba76029b69d91be39c9d63ca755e8a4603aec0b9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520981"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="fc33a-104">tipo de recurso de mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="fc33a-104">mailSearchFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc33a-105">Um mailSearchFolder é uma pasta virtual na caixa de correio do usuário que contém todos os itens de email que correspondam a critérios de pesquisa especificado.</span><span class="sxs-lookup"><span data-stu-id="fc33a-105">A mailSearchFolder is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="fc33a-106">mailSearchFolder herda de [mailFolder](mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="fc33a-106">mailSearchFolder inherits from [mailFolder](mailfolder.md).</span></span>

## <a name="methods"></a><span data-ttu-id="fc33a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="fc33a-107">Methods</span></span>

| <span data-ttu-id="fc33a-108">Método</span><span class="sxs-lookup"><span data-stu-id="fc33a-108">Method</span></span> | <span data-ttu-id="fc33a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fc33a-109">Return Type</span></span>  | <span data-ttu-id="fc33a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc33a-110">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="fc33a-111">Crie uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="fc33a-111">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="fc33a-112">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="fc33a-112">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="fc33a-113">Crie uma pasta de pesquisa na caixa de correio desse usuário.</span><span class="sxs-lookup"><span data-stu-id="fc33a-113">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="fc33a-114">Lista as pastas de pesquisa</span><span class="sxs-lookup"><span data-stu-id="fc33a-114">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="fc33a-115">Coleção [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="fc33a-115">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="fc33a-116">Liste todas as pastas na caixa de correio do usuário, incluindo as pastas de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="fc33a-116">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="fc33a-117">Obtenha uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="fc33a-117">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="fc33a-118">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="fc33a-118">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="fc33a-119">Obtenha a pasta de pesquisa especificado.</span><span class="sxs-lookup"><span data-stu-id="fc33a-119">Get the specified search folder.</span></span> |
| [<span data-ttu-id="fc33a-120">Atualizar uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="fc33a-120">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="fc33a-121">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="fc33a-121">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="fc33a-122">Atualize a pasta de pesquisa especificado.</span><span class="sxs-lookup"><span data-stu-id="fc33a-122">Update the specified search folder.</span></span> |
| [<span data-ttu-id="fc33a-123">Excluir uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="fc33a-123">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="fc33a-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc33a-124">None</span></span> | <span data-ttu-id="fc33a-125">Exclua a pasta de pesquisa especificado.</span><span class="sxs-lookup"><span data-stu-id="fc33a-125">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="fc33a-126">Listar todas as mensagens em uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="fc33a-126">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="fc33a-127">Coleção [message](message.md)</span><span class="sxs-lookup"><span data-stu-id="fc33a-127">[message](message.md) collection</span></span> | <span data-ttu-id="fc33a-128">Liste todas as mensagens na pasta de pesquisa especificado.</span><span class="sxs-lookup"><span data-stu-id="fc33a-128">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="fc33a-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc33a-129">Properties</span></span>

| <span data-ttu-id="fc33a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc33a-130">Property</span></span> | <span data-ttu-id="fc33a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc33a-131">Type</span></span> | <span data-ttu-id="fc33a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc33a-132">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="fc33a-133">isSupported</span><span class="sxs-lookup"><span data-stu-id="fc33a-133">isSupported</span></span> | <span data-ttu-id="fc33a-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="fc33a-134">Boolean</span></span> | <span data-ttu-id="fc33a-135">Indica se uma pasta de pesquisa é editável usando APIs REST.</span><span class="sxs-lookup"><span data-stu-id="fc33a-135">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="fc33a-136">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="fc33a-136">includeNestedFolders</span></span> | <span data-ttu-id="fc33a-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="fc33a-137">Boolean</span></span> | <span data-ttu-id="fc33a-138">Indica como a hierarquia de pastas de caixa de correio deve ser percorrida.</span><span class="sxs-lookup"><span data-stu-id="fc33a-138">Indicates how the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="fc33a-139">`true`significa que uma profundidade de pesquisa deve ser feito ao `false` significa rasos de pesquisa devem ser feito em vez disso.</span><span class="sxs-lookup"><span data-stu-id="fc33a-139">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="fc33a-140">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="fc33a-140">sourceFolderIDs</span></span> | <span data-ttu-id="fc33a-141">String collection</span><span class="sxs-lookup"><span data-stu-id="fc33a-141">String collection</span></span> | <span data-ttu-id="fc33a-142">As pastas de caixa de correio que devem ser extraídas.</span><span class="sxs-lookup"><span data-stu-id="fc33a-142">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="fc33a-143">filterQuery</span><span class="sxs-lookup"><span data-stu-id="fc33a-143">filterQuery</span></span> | <span data-ttu-id="fc33a-144">String</span><span class="sxs-lookup"><span data-stu-id="fc33a-144">String</span></span> | <span data-ttu-id="fc33a-145">A consulta OData para filtrar as mensagens.</span><span class="sxs-lookup"><span data-stu-id="fc33a-145">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fc33a-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc33a-146">JSON representation</span></span>

<span data-ttu-id="fc33a-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc33a-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailSearchFolder"
}-->

```json
{
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": ["string"],
  "filterQuery": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2018-01-23 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailsearchfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
