---
title: tipo de recurso mailSearchFolder
description: Um mailSearchFolder é uma pasta virtual na caixa de correio do usuário que contém todos os itens de email correspondentes aos critérios de pesquisa especificados. mailSearchFolder herda de mailFolder.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3e0c392270ac6b82462c7ffb99afb722c6e60bc9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461866"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="93649-104">tipo de recurso mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="93649-104">mailSearchFolder resource type</span></span>

<span data-ttu-id="93649-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93649-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="93649-106">Um **mailSearchFolder** é uma pasta virtual na caixa de correio do usuário que contém todos os itens de email correspondentes aos critérios de pesquisa especificados.</span><span class="sxs-lookup"><span data-stu-id="93649-106">A **mailSearchFolder** is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="93649-107">**mailSearchFolder** herda de [mailFolder](mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="93649-107">**mailSearchFolder** inherits from [mailFolder](mailfolder.md).</span></span> <span data-ttu-id="93649-108">Pastas de pesquisa podem ser criadas em qualquer pasta da caixa de correio do Exchange Online de um usuário.</span><span class="sxs-lookup"><span data-stu-id="93649-108">Search folders can be created in any folder in a user's Exchange Online mailbox.</span></span> <span data-ttu-id="93649-109">No entanto, para que uma pasta de pesquisa apareça no Outlook, no Outlook para a Web ou no Outlook Live, a pasta deve ser criada na pasta **WellKnownFolderName. SearchFolders** .</span><span class="sxs-lookup"><span data-stu-id="93649-109">However, for a search folder to appear in Outlook, Outlook for the web, or Outlook Live, the folder must be created in the **WellKnownFolderName.SearchFolders** folder.</span></span> 

## <a name="search-folder-lifecycle"></a><span data-ttu-id="93649-110">Ciclo de vida da pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="93649-110">Search folder lifecycle</span></span>

<span data-ttu-id="93649-111">Pastas de pesquisa criadas por seu aplicativo podem ser excluídas pelo Exchange Online por uma das seguintes razões:</span><span class="sxs-lookup"><span data-stu-id="93649-111">Search folders created by your application can be deleted by Exchange Online for one of the following reasons:</span></span>

1.  <span data-ttu-id="93649-112">As pastas de pesquisa expiram após 45 dias sem uso.</span><span class="sxs-lookup"><span data-stu-id="93649-112">Search folders expire after 45 days of no usage.</span></span> 
2.  <span data-ttu-id="93649-113">Há limites no número de pastas de pesquisa que podem ser criadas por pasta de origem.</span><span class="sxs-lookup"><span data-stu-id="93649-113">There are limits on the number of search folders that can be created per source folder.</span></span> <span data-ttu-id="93649-114">Quando esse limite é violado, as pastas de pesquisa mais antigas são excluídas para se tornarem novas.</span><span class="sxs-lookup"><span data-stu-id="93649-114">When this limit is breached, older search folders are deleted to make way for new ones.</span></span> 

<span data-ttu-id="93649-115">Quando uma pasta de pesquisa é excluída, seu aplicativo deve criar um novo recurso de pasta de pesquisa e usar o mesmo.</span><span class="sxs-lookup"><span data-stu-id="93649-115">When a search folder is deleted, your app should create a new search folder resource and use the same.</span></span>


## <a name="methods"></a><span data-ttu-id="93649-116">Métodos</span><span class="sxs-lookup"><span data-stu-id="93649-116">Methods</span></span>

| <span data-ttu-id="93649-117">Método</span><span class="sxs-lookup"><span data-stu-id="93649-117">Method</span></span> | <span data-ttu-id="93649-118">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="93649-118">Return Type</span></span>  | <span data-ttu-id="93649-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="93649-119">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="93649-120">Criar uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="93649-120">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="93649-121">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="93649-121">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="93649-122">Crie uma pasta de pesquisa na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="93649-122">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="93649-123">Listar pastas de pesquisa</span><span class="sxs-lookup"><span data-stu-id="93649-123">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="93649-124">Coleção [mailFolder](mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="93649-124">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="93649-125">Listar todas as pastas na caixa de correio do usuário, incluindo pastas de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="93649-125">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="93649-126">Obter uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="93649-126">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="93649-127">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="93649-127">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="93649-128">Obtém a pasta de pesquisa especificada.</span><span class="sxs-lookup"><span data-stu-id="93649-128">Get the specified search folder.</span></span> |
| [<span data-ttu-id="93649-129">Atualizar uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="93649-129">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="93649-130">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="93649-130">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="93649-131">Atualiza a pasta de pesquisa especificada.</span><span class="sxs-lookup"><span data-stu-id="93649-131">Update the specified search folder.</span></span> |
| [<span data-ttu-id="93649-132">Excluir uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="93649-132">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="93649-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="93649-133">None</span></span> | <span data-ttu-id="93649-134">Excluir a pasta de pesquisa especificada.</span><span class="sxs-lookup"><span data-stu-id="93649-134">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="93649-135">Listar todas as mensagens em uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="93649-135">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="93649-136">Coleção [message](message.md)</span><span class="sxs-lookup"><span data-stu-id="93649-136">[message](message.md) collection</span></span> | <span data-ttu-id="93649-137">Listar todas as mensagens na pasta de pesquisa especificada.</span><span class="sxs-lookup"><span data-stu-id="93649-137">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="93649-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93649-138">Properties</span></span>

| <span data-ttu-id="93649-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93649-139">Property</span></span> | <span data-ttu-id="93649-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="93649-140">Type</span></span> | <span data-ttu-id="93649-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="93649-141">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="93649-142">IsSupported</span><span class="sxs-lookup"><span data-stu-id="93649-142">isSupported</span></span> | <span data-ttu-id="93649-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="93649-143">Boolean</span></span> | <span data-ttu-id="93649-144">Indica se uma pasta de pesquisa é editável usando as APIs REST.</span><span class="sxs-lookup"><span data-stu-id="93649-144">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="93649-145">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="93649-145">includeNestedFolders</span></span> | <span data-ttu-id="93649-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="93649-146">Boolean</span></span> | <span data-ttu-id="93649-147">Indica como a hierarquia da pasta da caixa de correio deve ser percorrida na pesquisa.</span><span class="sxs-lookup"><span data-stu-id="93649-147">Indicates how the mailbox folder hierarchy should be traversed in the search.</span></span> <span data-ttu-id="93649-148">`true`significa que uma pesquisa profunda deve ser feita para incluir pastas filhas na hierarquia de cada pasta explicitamente especificada no **sourceFolderIds**.</span><span class="sxs-lookup"><span data-stu-id="93649-148">`true` means that a deep search should be done to include child folders in the hierarchy of each folder explicitly specified in **sourceFolderIds**.</span></span> <span data-ttu-id="93649-149">`false`significa uma pesquisa superficial de apenas cada uma das pastas explicitamente especificadas no **sourceFolderIds**.</span><span class="sxs-lookup"><span data-stu-id="93649-149">`false` means a shallow search of only each of the folders explicitly specified in **sourceFolderIds**.</span></span> |
| <span data-ttu-id="93649-150">sourceFolderIds</span><span class="sxs-lookup"><span data-stu-id="93649-150">sourceFolderIds</span></span> | <span data-ttu-id="93649-151">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="93649-151">String collection</span></span> | <span data-ttu-id="93649-152">As pastas de caixa de correio que devem ser minadas.</span><span class="sxs-lookup"><span data-stu-id="93649-152">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="93649-153">filterQuery</span><span class="sxs-lookup"><span data-stu-id="93649-153">filterQuery</span></span> | <span data-ttu-id="93649-154">String</span><span class="sxs-lookup"><span data-stu-id="93649-154">String</span></span> | <span data-ttu-id="93649-155">A consulta OData para filtrar as mensagens.</span><span class="sxs-lookup"><span data-stu-id="93649-155">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="93649-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93649-156">JSON representation</span></span>

<span data-ttu-id="93649-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93649-157">The following is a JSON representation of the resource.</span></span>

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
