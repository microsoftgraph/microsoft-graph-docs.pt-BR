---
title: tipo de recurso mailSearchFolder
description: Um mailSearchFolder é uma pasta virtual na caixa de correio do usuário que contém todos os itens de email correspondentes aos critérios de pesquisa especificados. mailSearchFolder herda de mailFolder.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f709347d8ba81a5b42ab512a80beae8780805f2f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009843"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="2e292-104">tipo de recurso mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="2e292-104">mailSearchFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e292-105">Um **mailSearchFolder** é uma pasta virtual na caixa de correio do usuário que contém todos os itens de email correspondentes aos critérios de pesquisa especificados.</span><span class="sxs-lookup"><span data-stu-id="2e292-105">A **mailSearchFolder** is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="2e292-106">**mailSearchFolder** herda de [mailFolder](mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="2e292-106">**mailSearchFolder** inherits from [mailFolder](mailfolder.md).</span></span> <span data-ttu-id="2e292-107">Pastas de pesquisa podem ser criadas em qualquer pasta da caixa de correio do Exchange Online de um usuário.</span><span class="sxs-lookup"><span data-stu-id="2e292-107">Search folders can be created in any folder in a user's Exchange Online mailbox.</span></span> <span data-ttu-id="2e292-108">No entanto, para que uma pasta de pesquisa apareça no Outlook, no Outlook para a Web ou no Outlook Live, a pasta deve ser criada na pasta **WellKnownFolderName. SearchFolders** .</span><span class="sxs-lookup"><span data-stu-id="2e292-108">However, for a search folder to appear in Outlook, Outlook for the web, or Outlook Live, the folder must be created in the **WellKnownFolderName.SearchFolders** folder.</span></span> 

## <a name="search-folder-lifecycle"></a><span data-ttu-id="2e292-109">Ciclo de vida da pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="2e292-109">Search folder lifecycle</span></span>

<span data-ttu-id="2e292-110">Pastas de pesquisa criadas por seu aplicativo podem ser excluídas pelo Exchange Online por uma das seguintes razões:</span><span class="sxs-lookup"><span data-stu-id="2e292-110">Search folders created by your application can be deleted by Exchange Online for one of the following reasons:</span></span>

1.  <span data-ttu-id="2e292-111">As pastas de pesquisa expiram após 45 dias sem uso.</span><span class="sxs-lookup"><span data-stu-id="2e292-111">Search folders expire after 45 days of no usage.</span></span> 
2.  <span data-ttu-id="2e292-112">Há limites no número de pastas de pesquisa que podem ser criadas por pasta de origem.</span><span class="sxs-lookup"><span data-stu-id="2e292-112">There are limits on the number of search folders that can be created per source folder.</span></span> <span data-ttu-id="2e292-113">Quando esse limite é violado, as pastas de pesquisa mais antigas são excluídas para se tornarem novas.</span><span class="sxs-lookup"><span data-stu-id="2e292-113">When this limit is breached, older search folders are deleted to make way for new ones.</span></span> 

<span data-ttu-id="2e292-114">Quando uma pasta de pesquisa é excluída, seu aplicativo deve criar um novo recurso de pasta de pesquisa e usar o mesmo.</span><span class="sxs-lookup"><span data-stu-id="2e292-114">When a search folder is deleted, your app should create a new search folder resource and use the same.</span></span>


## <a name="methods"></a><span data-ttu-id="2e292-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="2e292-115">Methods</span></span>

| <span data-ttu-id="2e292-116">Método</span><span class="sxs-lookup"><span data-stu-id="2e292-116">Method</span></span> | <span data-ttu-id="2e292-117">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2e292-117">Return Type</span></span>  | <span data-ttu-id="2e292-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e292-118">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="2e292-119">Criar uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="2e292-119">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="2e292-120">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="2e292-120">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="2e292-121">Crie uma pasta de pesquisa na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="2e292-121">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="2e292-122">Listar pastas de pesquisa</span><span class="sxs-lookup"><span data-stu-id="2e292-122">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="2e292-123">Coleção [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="2e292-123">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="2e292-124">Listar todas as pastas na caixa de correio do usuário, incluindo pastas de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="2e292-124">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="2e292-125">Obter uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="2e292-125">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="2e292-126">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="2e292-126">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="2e292-127">Obtém a pasta de pesquisa especificada.</span><span class="sxs-lookup"><span data-stu-id="2e292-127">Get the specified search folder.</span></span> |
| [<span data-ttu-id="2e292-128">Atualizar uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="2e292-128">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="2e292-129">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="2e292-129">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="2e292-130">Atualiza a pasta de pesquisa especificada.</span><span class="sxs-lookup"><span data-stu-id="2e292-130">Update the specified search folder.</span></span> |
| [<span data-ttu-id="2e292-131">Excluir uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="2e292-131">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="2e292-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2e292-132">None</span></span> | <span data-ttu-id="2e292-133">Excluir a pasta de pesquisa especificada.</span><span class="sxs-lookup"><span data-stu-id="2e292-133">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="2e292-134">Listar todas as mensagens em uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="2e292-134">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="2e292-135">Coleção [message](message.md)</span><span class="sxs-lookup"><span data-stu-id="2e292-135">[message](message.md) collection</span></span> | <span data-ttu-id="2e292-136">Listar todas as mensagens na pasta de pesquisa especificada.</span><span class="sxs-lookup"><span data-stu-id="2e292-136">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="2e292-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2e292-137">Properties</span></span>

| <span data-ttu-id="2e292-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e292-138">Property</span></span> | <span data-ttu-id="2e292-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e292-139">Type</span></span> | <span data-ttu-id="2e292-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e292-140">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="2e292-141">IsSupported</span><span class="sxs-lookup"><span data-stu-id="2e292-141">isSupported</span></span> | <span data-ttu-id="2e292-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="2e292-142">Boolean</span></span> | <span data-ttu-id="2e292-143">Indica se uma pasta de pesquisa é editável usando as APIs REST.</span><span class="sxs-lookup"><span data-stu-id="2e292-143">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="2e292-144">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="2e292-144">includeNestedFolders</span></span> | <span data-ttu-id="2e292-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="2e292-145">Boolean</span></span> | <span data-ttu-id="2e292-146">Indica como a hierarquia da pasta da caixa de correio deve ser percorrida na pesquisa.</span><span class="sxs-lookup"><span data-stu-id="2e292-146">Indicates how the mailbox folder hierarchy should be traversed in the search.</span></span> <span data-ttu-id="2e292-147">`true`significa que uma pesquisa profunda deve ser feita para incluir pastas filhas na hierarquia de cada pasta explicitamente especificada no **sourceFolderIds**.</span><span class="sxs-lookup"><span data-stu-id="2e292-147">`true` means that a deep search should be done to include child folders in the hierarchy of each folder explicitly specified in **sourceFolderIds**.</span></span> <span data-ttu-id="2e292-148">`false`significa uma pesquisa superficial de apenas cada uma das pastas explicitamente especificadas no **sourceFolderIds**.</span><span class="sxs-lookup"><span data-stu-id="2e292-148">`false` means a shallow search of only each of the folders explicitly specified in **sourceFolderIds**.</span></span> |
| <span data-ttu-id="2e292-149">sourceFolderIds</span><span class="sxs-lookup"><span data-stu-id="2e292-149">sourceFolderIds</span></span> | <span data-ttu-id="2e292-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e292-150">String collection</span></span> | <span data-ttu-id="2e292-151">As pastas de caixa de correio que devem ser minadas.</span><span class="sxs-lookup"><span data-stu-id="2e292-151">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="2e292-152">filterQuery</span><span class="sxs-lookup"><span data-stu-id="2e292-152">filterQuery</span></span> | <span data-ttu-id="2e292-153">String</span><span class="sxs-lookup"><span data-stu-id="2e292-153">String</span></span> | <span data-ttu-id="2e292-154">A consulta OData para filtrar as mensagens.</span><span class="sxs-lookup"><span data-stu-id="2e292-154">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2e292-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2e292-155">JSON representation</span></span>

<span data-ttu-id="2e292-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2e292-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailSearchFolder"
}-->

```json
{
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIds": ["string"],
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
