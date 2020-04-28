---
title: tipo de recurso printerShare
description: Representa uma impressora que pretende ser detectável por usuários e por aplicativos de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 26715bb8eed9c671b88951bd1deb875f1d11d467
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917562"
---
# <a name="printershare-resource-type"></a><span data-ttu-id="bc1d9-103">tipo de recurso printerShare</span><span class="sxs-lookup"><span data-stu-id="bc1d9-103">printerShare resource type</span></span>

<span data-ttu-id="bc1d9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc1d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc1d9-105">Representa uma impressora que pretende ser detectável por usuários e por aplicativos de impressão.</span><span class="sxs-lookup"><span data-stu-id="bc1d9-105">Represents a printer that is intended to be discoverable by users and printing applications.</span></span>

## <a name="methods"></a><span data-ttu-id="bc1d9-106">Methods</span><span class="sxs-lookup"><span data-stu-id="bc1d9-106">Methods</span></span>

| <span data-ttu-id="bc1d9-107">Método</span><span class="sxs-lookup"><span data-stu-id="bc1d9-107">Method</span></span>       | <span data-ttu-id="bc1d9-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bc1d9-108">Return Type</span></span> | <span data-ttu-id="bc1d9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc1d9-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bc1d9-110">List</span><span class="sxs-lookup"><span data-stu-id="bc1d9-110">List</span></span>](../api/print-list-printershares.md) | <span data-ttu-id="bc1d9-111">coleção [printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="bc1d9-111">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="bc1d9-112">Obtenha uma lista de compartilhamentos de impressora no locatário.</span><span class="sxs-lookup"><span data-stu-id="bc1d9-112">Get a list of printer shares in the tenant.</span></span> |
| [<span data-ttu-id="bc1d9-113">Get</span><span class="sxs-lookup"><span data-stu-id="bc1d9-113">Get</span></span>](../api/printershare-get.md) | [<span data-ttu-id="bc1d9-114">printerShare</span><span class="sxs-lookup"><span data-stu-id="bc1d9-114">printerShare</span></span>](printershare.md) | <span data-ttu-id="bc1d9-115">Ler propriedades e relações de um objeto **printerShare** .</span><span class="sxs-lookup"><span data-stu-id="bc1d9-115">Read properties and relationships of a **printerShare** object.</span></span> |
| [<span data-ttu-id="bc1d9-116">Update</span><span class="sxs-lookup"><span data-stu-id="bc1d9-116">Update</span></span>](../api/printershare-update.md) | [<span data-ttu-id="bc1d9-117">printerShare</span><span class="sxs-lookup"><span data-stu-id="bc1d9-117">printerShare</span></span>](printershare.md) | <span data-ttu-id="bc1d9-118">Atualizar um objeto **printerShare** .</span><span class="sxs-lookup"><span data-stu-id="bc1d9-118">Update a **printerShare** object.</span></span> |
| [<span data-ttu-id="bc1d9-119">Delete</span><span class="sxs-lookup"><span data-stu-id="bc1d9-119">Delete</span></span>](../api/printershare-delete.md) | <span data-ttu-id="bc1d9-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bc1d9-120">None</span></span> | <span data-ttu-id="bc1d9-121">Descompartilhar uma impressora.</span><span class="sxs-lookup"><span data-stu-id="bc1d9-121">Unshare a printer.</span></span> |
| [<span data-ttu-id="bc1d9-122">Listar allowedUsers</span><span class="sxs-lookup"><span data-stu-id="bc1d9-122">List allowedUsers</span></span>](../api/printershare-list-allowedusers.md) | <span data-ttu-id="bc1d9-123">coleção [printUserIdentity](printuseridentity.md)</span><span class="sxs-lookup"><span data-stu-id="bc1d9-123">[printUserIdentity](printuseridentity.md) collection</span></span> | <span data-ttu-id="bc1d9-124">Recupere uma lista de usuários que receberam acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado.</span><span class="sxs-lookup"><span data-stu-id="bc1d9-124">Retrieve a list of users who have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="bc1d9-125">Adicionar allowedUser</span><span class="sxs-lookup"><span data-stu-id="bc1d9-125">Add allowedUser</span></span>](../api/printershare-post-allowedusers.md) | <span data-ttu-id="bc1d9-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bc1d9-126">None</span></span> | <span data-ttu-id="bc1d9-127">Conceda ao usuário especificado o acesso ao envio de trabalhos de impressão para o compartilhamento de impressora associado.</span><span class="sxs-lookup"><span data-stu-id="bc1d9-127">Grant the specified user access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="bc1d9-128">Remover allowedUser</span><span class="sxs-lookup"><span data-stu-id="bc1d9-128">Remove allowedUser</span></span>](../api/printershare-delete-alloweduser.md) | <span data-ttu-id="bc1d9-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bc1d9-129">None</span></span> | <span data-ttu-id="bc1d9-130">Revoga o acesso ao compartilhamento de impressora do usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="bc1d9-130">Revoke printer share access from the specified user.</span></span> |
| [<span data-ttu-id="bc1d9-131">Listar allowedGroups</span><span class="sxs-lookup"><span data-stu-id="bc1d9-131">List allowedGroups</span></span>](../api/printershare-list-allowedgroups.md) | <span data-ttu-id="bc1d9-132">coleção [Multiidentity](printidentity.md)</span><span class="sxs-lookup"><span data-stu-id="bc1d9-132">[printIdentity](printidentity.md) collection</span></span> | <span data-ttu-id="bc1d9-133">Recupere uma lista de grupos aos quais foi concedido acesso para enviar trabalhos de impressão ao compartilhamento de impressora associado.</span><span class="sxs-lookup"><span data-stu-id="bc1d9-133">Retrieve a list of groups that have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="bc1d9-134">Adicionar allowedGroup</span><span class="sxs-lookup"><span data-stu-id="bc1d9-134">Add allowedGroup</span></span>](../api/printershare-post-allowedgroups.md) | <span data-ttu-id="bc1d9-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bc1d9-135">None</span></span> | <span data-ttu-id="bc1d9-136">Conceda ao grupo especificado o acesso ao envio de trabalhos de impressão para o compartilhamento de impressora associado.</span><span class="sxs-lookup"><span data-stu-id="bc1d9-136">Grant the specified group access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="bc1d9-137">Remover allowedGroup</span><span class="sxs-lookup"><span data-stu-id="bc1d9-137">Remove allowedGroup</span></span>](../api/printershare-delete-allowedgroup.md) | <span data-ttu-id="bc1d9-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bc1d9-138">None</span></span> | <span data-ttu-id="bc1d9-139">Revoga o acesso ao compartilhamento de impressora do grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="bc1d9-139">Revoke printer share access from the specified group.</span></span> |

## <a name="properties"></a><span data-ttu-id="bc1d9-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc1d9-140">Properties</span></span>
| <span data-ttu-id="bc1d9-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc1d9-141">Property</span></span>     | <span data-ttu-id="bc1d9-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc1d9-142">Type</span></span>        | <span data-ttu-id="bc1d9-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc1d9-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bc1d9-144">id</span><span class="sxs-lookup"><span data-stu-id="bc1d9-144">id</span></span>|<span data-ttu-id="bc1d9-145">String</span><span class="sxs-lookup"><span data-stu-id="bc1d9-145">String</span></span>| <span data-ttu-id="bc1d9-146">O identificador do printerShare.</span><span class="sxs-lookup"><span data-stu-id="bc1d9-146">The printerShare's identifier.</span></span> <span data-ttu-id="bc1d9-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc1d9-147">Read-only.</span></span>|
|<span data-ttu-id="bc1d9-148">name</span><span class="sxs-lookup"><span data-stu-id="bc1d9-148">name</span></span>|<span data-ttu-id="bc1d9-149">String</span><span class="sxs-lookup"><span data-stu-id="bc1d9-149">String</span></span>|<span data-ttu-id="bc1d9-150">O nome do compartilhamento de impressora que os clientes de impressão devem exibir.</span><span class="sxs-lookup"><span data-stu-id="bc1d9-150">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="bc1d9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc1d9-151">createdDateTime</span></span>|<span data-ttu-id="bc1d9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc1d9-152">DateTimeOffset</span></span>|<span data-ttu-id="bc1d9-153">O DateTimeOffset quando o compartilhamento da impressora foi criado.</span><span class="sxs-lookup"><span data-stu-id="bc1d9-153">The DateTimeOffset when the printer share was created.</span></span> <span data-ttu-id="bc1d9-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc1d9-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc1d9-155">Relações</span><span class="sxs-lookup"><span data-stu-id="bc1d9-155">Relationships</span></span>
| <span data-ttu-id="bc1d9-156">Relação</span><span class="sxs-lookup"><span data-stu-id="bc1d9-156">Relationship</span></span> | <span data-ttu-id="bc1d9-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc1d9-157">Type</span></span>        | <span data-ttu-id="bc1d9-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc1d9-158">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bc1d9-159">impressora</span><span class="sxs-lookup"><span data-stu-id="bc1d9-159">printer</span></span>|[<span data-ttu-id="bc1d9-160">impressora</span><span class="sxs-lookup"><span data-stu-id="bc1d9-160">printer</span></span>](printer.md)|<span data-ttu-id="bc1d9-161">A impressora à qual esse compartilhamento de impressora está relacionado.</span><span class="sxs-lookup"><span data-stu-id="bc1d9-161">The printer that this printer share is related to.</span></span> |
|<span data-ttu-id="bc1d9-162">allowedUsers</span><span class="sxs-lookup"><span data-stu-id="bc1d9-162">allowedUsers</span></span>|<span data-ttu-id="bc1d9-163">coleção [printUserIdentity](printuseridentity.md)</span><span class="sxs-lookup"><span data-stu-id="bc1d9-163">[printUserIdentity](printuseridentity.md) collection</span></span>|<span data-ttu-id="bc1d9-164">Os usuários que têm acesso à impressão usando a impressora.</span><span class="sxs-lookup"><span data-stu-id="bc1d9-164">The users who have access to print using the printer.</span></span>|
|<span data-ttu-id="bc1d9-165">allowedGroups</span><span class="sxs-lookup"><span data-stu-id="bc1d9-165">allowedGroups</span></span>|[<span data-ttu-id="bc1d9-166">multiidentity</span><span class="sxs-lookup"><span data-stu-id="bc1d9-166">printIdentity</span></span>](printidentity.md)|<span data-ttu-id="bc1d9-167">Os grupos cujos usuários têm acesso para imprimir usando a impressora.</span><span class="sxs-lookup"><span data-stu-id="bc1d9-167">The groups whose users have access to print using the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc1d9-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc1d9-168">JSON representation</span></span>

<span data-ttu-id="bc1d9-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc1d9-169">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerShare",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerShare resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
