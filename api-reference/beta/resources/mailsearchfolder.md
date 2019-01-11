---
title: tipo de recurso de mailSearchFolder
description: Um mailSearchFolder é uma pasta virtual na caixa de correio do usuário que contém todos os itens de email que correspondam a critérios de pesquisa especificado. mailSearchFolder herda de mailFolder.
localization_priority: Normal
ms.openlocfilehash: 62d4d8569977c99690e317a39a43bbc9d9dca3f1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870389"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="68b0d-104">tipo de recurso de mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="68b0d-104">mailSearchFolder resource type</span></span>

> <span data-ttu-id="68b0d-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="68b0d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68b0d-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="68b0d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="68b0d-107">Um mailSearchFolder é uma pasta virtual na caixa de correio do usuário que contém todos os itens de email que correspondam a critérios de pesquisa especificado.</span><span class="sxs-lookup"><span data-stu-id="68b0d-107">A mailSearchFolder is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="68b0d-108">mailSearchFolder herda de [mailFolder](mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="68b0d-108">mailSearchFolder inherits from [mailFolder](mailfolder.md).</span></span>

## <a name="methods"></a><span data-ttu-id="68b0d-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="68b0d-109">Methods</span></span>

| <span data-ttu-id="68b0d-110">Método</span><span class="sxs-lookup"><span data-stu-id="68b0d-110">Method</span></span> | <span data-ttu-id="68b0d-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="68b0d-111">Return Type</span></span>  | <span data-ttu-id="68b0d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="68b0d-112">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="68b0d-113">Crie uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="68b0d-113">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="68b0d-114">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="68b0d-114">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="68b0d-115">Crie uma pasta de pesquisa na caixa de correio desse usuário.</span><span class="sxs-lookup"><span data-stu-id="68b0d-115">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="68b0d-116">Lista as pastas de pesquisa</span><span class="sxs-lookup"><span data-stu-id="68b0d-116">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="68b0d-117">Coleção [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="68b0d-117">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="68b0d-118">Liste todas as pastas na caixa de correio do usuário, incluindo as pastas de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="68b0d-118">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="68b0d-119">Obtenha uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="68b0d-119">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="68b0d-120">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="68b0d-120">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="68b0d-121">Obtenha a pasta de pesquisa especificado.</span><span class="sxs-lookup"><span data-stu-id="68b0d-121">Get the specified search folder.</span></span> |
| [<span data-ttu-id="68b0d-122">Atualizar uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="68b0d-122">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="68b0d-123">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="68b0d-123">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="68b0d-124">Atualize a pasta de pesquisa especificado.</span><span class="sxs-lookup"><span data-stu-id="68b0d-124">Update the specified search folder.</span></span> |
| [<span data-ttu-id="68b0d-125">Excluir uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="68b0d-125">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="68b0d-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="68b0d-126">None</span></span> | <span data-ttu-id="68b0d-127">Exclua a pasta de pesquisa especificado.</span><span class="sxs-lookup"><span data-stu-id="68b0d-127">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="68b0d-128">Listar todas as mensagens em uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="68b0d-128">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="68b0d-129">Coleção [message](message.md)</span><span class="sxs-lookup"><span data-stu-id="68b0d-129">[message](message.md) collection</span></span> | <span data-ttu-id="68b0d-130">Liste todas as mensagens na pasta de pesquisa especificado.</span><span class="sxs-lookup"><span data-stu-id="68b0d-130">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="68b0d-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68b0d-131">Properties</span></span>

| <span data-ttu-id="68b0d-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68b0d-132">Property</span></span> | <span data-ttu-id="68b0d-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="68b0d-133">Type</span></span> | <span data-ttu-id="68b0d-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="68b0d-134">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="68b0d-135">isSupported</span><span class="sxs-lookup"><span data-stu-id="68b0d-135">isSupported</span></span> | <span data-ttu-id="68b0d-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="68b0d-136">Boolean</span></span> | <span data-ttu-id="68b0d-137">Indica se uma pasta de pesquisa é editável usando APIs REST.</span><span class="sxs-lookup"><span data-stu-id="68b0d-137">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="68b0d-138">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="68b0d-138">includeNestedFolders</span></span> | <span data-ttu-id="68b0d-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="68b0d-139">Boolean</span></span> | <span data-ttu-id="68b0d-140">Indica como a hierarquia de pastas de caixa de correio deve ser percorrida.</span><span class="sxs-lookup"><span data-stu-id="68b0d-140">Indicates how the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="68b0d-141">`true`significa que uma profundidade de pesquisa deve ser feito ao `false` significa rasos de pesquisa devem ser feito em vez disso.</span><span class="sxs-lookup"><span data-stu-id="68b0d-141">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="68b0d-142">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="68b0d-142">sourceFolderIDs</span></span> | <span data-ttu-id="68b0d-143">String collection</span><span class="sxs-lookup"><span data-stu-id="68b0d-143">String collection</span></span> | <span data-ttu-id="68b0d-144">As pastas de caixa de correio que devem ser extraídas.</span><span class="sxs-lookup"><span data-stu-id="68b0d-144">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="68b0d-145">filterQuery</span><span class="sxs-lookup"><span data-stu-id="68b0d-145">filterQuery</span></span> | <span data-ttu-id="68b0d-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68b0d-146">String</span></span> | <span data-ttu-id="68b0d-147">A consulta OData para filtrar as mensagens.</span><span class="sxs-lookup"><span data-stu-id="68b0d-147">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="68b0d-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68b0d-148">JSON representation</span></span>

<span data-ttu-id="68b0d-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="68b0d-149">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
