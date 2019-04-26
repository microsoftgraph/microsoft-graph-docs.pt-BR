---
title: tipo de recurso mailSearchFolder
description: Um mailSearchFolder é uma pasta virtual na caixa de correio do usuário que contém todos os itens de email correspondentes aos critérios de pesquisa especificados. mailSearchFolder herda de mailFolder.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 15f334f2910c962c367242965bd2104c8f3edb79
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342742"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="83495-104">tipo de recurso mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="83495-104">mailSearchFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83495-105">Um mailSearchFolder é uma pasta virtual na caixa de correio do usuário que contém todos os itens de email correspondentes aos critérios de pesquisa especificados.</span><span class="sxs-lookup"><span data-stu-id="83495-105">A mailSearchFolder is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="83495-106">mailSearchFolder herda de [mailFolder](mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="83495-106">mailSearchFolder inherits from [mailFolder](mailfolder.md).</span></span>

## <a name="methods"></a><span data-ttu-id="83495-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="83495-107">Methods</span></span>

| <span data-ttu-id="83495-108">Método</span><span class="sxs-lookup"><span data-stu-id="83495-108">Method</span></span> | <span data-ttu-id="83495-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="83495-109">Return Type</span></span>  | <span data-ttu-id="83495-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="83495-110">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="83495-111">Criar uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="83495-111">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="83495-112">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="83495-112">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="83495-113">Crie uma pasta de pesquisa na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="83495-113">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="83495-114">Listar pastas de pesquisa</span><span class="sxs-lookup"><span data-stu-id="83495-114">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="83495-115">Coleção [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="83495-115">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="83495-116">Listar todas as pastas na caixa de correio do usuário, incluindo pastas de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="83495-116">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="83495-117">Obter uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="83495-117">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="83495-118">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="83495-118">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="83495-119">Obtém a pasta de pesquisa especificada.</span><span class="sxs-lookup"><span data-stu-id="83495-119">Get the specified search folder.</span></span> |
| [<span data-ttu-id="83495-120">Atualizar uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="83495-120">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="83495-121">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="83495-121">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="83495-122">Atualiza a pasta de pesquisa especificada.</span><span class="sxs-lookup"><span data-stu-id="83495-122">Update the specified search folder.</span></span> |
| [<span data-ttu-id="83495-123">Excluir uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="83495-123">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="83495-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="83495-124">None</span></span> | <span data-ttu-id="83495-125">Excluir a pasta de pesquisa especificada.</span><span class="sxs-lookup"><span data-stu-id="83495-125">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="83495-126">Listar todas as mensagens em uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="83495-126">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="83495-127">Coleção [message](message.md)</span><span class="sxs-lookup"><span data-stu-id="83495-127">[message](message.md) collection</span></span> | <span data-ttu-id="83495-128">Listar todas as mensagens na pasta de pesquisa especificada.</span><span class="sxs-lookup"><span data-stu-id="83495-128">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="83495-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83495-129">Properties</span></span>

| <span data-ttu-id="83495-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83495-130">Property</span></span> | <span data-ttu-id="83495-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="83495-131">Type</span></span> | <span data-ttu-id="83495-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="83495-132">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="83495-133">isSupported</span><span class="sxs-lookup"><span data-stu-id="83495-133">isSupported</span></span> | <span data-ttu-id="83495-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="83495-134">Boolean</span></span> | <span data-ttu-id="83495-135">Indica se uma pasta de pesquisa é editável usando as APIs REST.</span><span class="sxs-lookup"><span data-stu-id="83495-135">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="83495-136">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="83495-136">includeNestedFolders</span></span> | <span data-ttu-id="83495-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="83495-137">Boolean</span></span> | <span data-ttu-id="83495-138">Indica como a hierarquia da pasta da caixa de correio deve ser percorrida.</span><span class="sxs-lookup"><span data-stu-id="83495-138">Indicates how the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="83495-139">`true`significa que uma pesquisa profunda deve ser feita enquanto `false` uma pesquisa superficial deve ser realizada.</span><span class="sxs-lookup"><span data-stu-id="83495-139">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="83495-140">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="83495-140">sourceFolderIDs</span></span> | <span data-ttu-id="83495-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="83495-141">String collection</span></span> | <span data-ttu-id="83495-142">As pastas de caixa de correio que devem ser minadas.</span><span class="sxs-lookup"><span data-stu-id="83495-142">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="83495-143">filterQuery</span><span class="sxs-lookup"><span data-stu-id="83495-143">filterQuery</span></span> | <span data-ttu-id="83495-144">String</span><span class="sxs-lookup"><span data-stu-id="83495-144">String</span></span> | <span data-ttu-id="83495-145">A consulta OData para filtrar as mensagens.</span><span class="sxs-lookup"><span data-stu-id="83495-145">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="83495-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83495-146">JSON representation</span></span>

<span data-ttu-id="83495-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83495-147">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
