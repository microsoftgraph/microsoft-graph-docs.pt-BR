---
title: tipo de recurso printerShare
description: Representa uma impressora que pretende ser detectável por usuários e por aplicativos de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 8aa9312bf8b7e8f9a2cec049b8275d4ce7a04012
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2020
ms.locfileid: "43806847"
---
# <a name="printershare-resource-type"></a><span data-ttu-id="b9569-103">tipo de recurso printerShare</span><span class="sxs-lookup"><span data-stu-id="b9569-103">printerShare resource type</span></span>

<span data-ttu-id="b9569-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9569-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9569-105">Representa uma impressora que pretende ser detectável por usuários e por aplicativos de impressão.</span><span class="sxs-lookup"><span data-stu-id="b9569-105">Represents a printer that is intended to be discoverable by users and printing applications.</span></span>

## <a name="methods"></a><span data-ttu-id="b9569-106">Methods</span><span class="sxs-lookup"><span data-stu-id="b9569-106">Methods</span></span>

| <span data-ttu-id="b9569-107">Método</span><span class="sxs-lookup"><span data-stu-id="b9569-107">Method</span></span>       | <span data-ttu-id="b9569-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b9569-108">Return Type</span></span> | <span data-ttu-id="b9569-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9569-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b9569-110">List</span><span class="sxs-lookup"><span data-stu-id="b9569-110">List</span></span>](../api/print-list-printershares.md) | <span data-ttu-id="b9569-111">coleção [printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="b9569-111">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="b9569-112">Obtenha uma lista de compartilhamentos de impressora no locatário.</span><span class="sxs-lookup"><span data-stu-id="b9569-112">Get a list of printer shares in the tenant.</span></span> |
| [<span data-ttu-id="b9569-113">Get</span><span class="sxs-lookup"><span data-stu-id="b9569-113">Get</span></span>](../api/printershare-get.md) | [<span data-ttu-id="b9569-114">printerShare</span><span class="sxs-lookup"><span data-stu-id="b9569-114">printerShare</span></span>](printershare.md) | <span data-ttu-id="b9569-115">Ler propriedades e relações de um objeto **printerShare** .</span><span class="sxs-lookup"><span data-stu-id="b9569-115">Read properties and relationships of a **printerShare** object.</span></span> |
| [<span data-ttu-id="b9569-116">Atualização</span><span class="sxs-lookup"><span data-stu-id="b9569-116">Update</span></span>](../api/printershare-update.md) | [<span data-ttu-id="b9569-117">printerShare</span><span class="sxs-lookup"><span data-stu-id="b9569-117">printerShare</span></span>](printershare.md) | <span data-ttu-id="b9569-118">Atualizar um objeto **printerShare** .</span><span class="sxs-lookup"><span data-stu-id="b9569-118">Update a **printerShare** object.</span></span> |
| [<span data-ttu-id="b9569-119">Delete</span><span class="sxs-lookup"><span data-stu-id="b9569-119">Delete</span></span>](../api/printershare-delete.md) | <span data-ttu-id="b9569-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9569-120">None</span></span> | <span data-ttu-id="b9569-121">Descompartilhar uma impressora.</span><span class="sxs-lookup"><span data-stu-id="b9569-121">Unshare a printer.</span></span> |
| [<span data-ttu-id="b9569-122">Listar allowedUsers</span><span class="sxs-lookup"><span data-stu-id="b9569-122">List allowedUsers</span></span>](../api/printershare-list-allowedusers.md) | <span data-ttu-id="b9569-123">coleção [UserIdentity](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="b9569-123">[userIdentity](useridentity.md) collection</span></span> | <span data-ttu-id="b9569-124">Recupere uma lista de usuários que receberam acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado.</span><span class="sxs-lookup"><span data-stu-id="b9569-124">Retrieve a list of users who have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="b9569-125">Adicionar allowedUser</span><span class="sxs-lookup"><span data-stu-id="b9569-125">Add allowedUser</span></span>](../api/printershare-post-allowedusers.md) | <span data-ttu-id="b9569-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9569-126">None</span></span> | <span data-ttu-id="b9569-127">Conceda ao usuário especificado o acesso ao envio de trabalhos de impressão para o compartilhamento de impressora associado.</span><span class="sxs-lookup"><span data-stu-id="b9569-127">Grant the specified user access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="b9569-128">Remover allowedUser</span><span class="sxs-lookup"><span data-stu-id="b9569-128">Remove allowedUser</span></span>](../api/printershare-delete-alloweduser.md) | <span data-ttu-id="b9569-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9569-129">None</span></span> | <span data-ttu-id="b9569-130">Revoga o acesso ao compartilhamento de impressora do usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="b9569-130">Revoke printer share access from the specified user.</span></span> |
| [<span data-ttu-id="b9569-131">Listar allowedGroups</span><span class="sxs-lookup"><span data-stu-id="b9569-131">List allowedGroups</span></span>](../api/printershare-list-allowedgroups.md) | <span data-ttu-id="b9569-132">coleção [Identity](identity.md)</span><span class="sxs-lookup"><span data-stu-id="b9569-132">[identity](identity.md) collection</span></span> | <span data-ttu-id="b9569-133">Recupere uma lista de grupos aos quais foi concedido acesso para enviar trabalhos de impressão ao compartilhamento de impressora associado.</span><span class="sxs-lookup"><span data-stu-id="b9569-133">Retrieve a list of groups that have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="b9569-134">Adicionar allowedGroup</span><span class="sxs-lookup"><span data-stu-id="b9569-134">Add allowedGroup</span></span>](../api/printershare-post-allowedgroups.md) | <span data-ttu-id="b9569-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9569-135">None</span></span> | <span data-ttu-id="b9569-136">Conceda ao grupo especificado o acesso ao envio de trabalhos de impressão para o compartilhamento de impressora associado.</span><span class="sxs-lookup"><span data-stu-id="b9569-136">Grant the specified group access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="b9569-137">Remover allowedGroup</span><span class="sxs-lookup"><span data-stu-id="b9569-137">Remove allowedGroup</span></span>](../api/printershare-delete-allowedgroup.md) | <span data-ttu-id="b9569-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9569-138">None</span></span> | <span data-ttu-id="b9569-139">Revoga o acesso ao compartilhamento de impressora do grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="b9569-139">Revoke printer share access from the specified group.</span></span> |

## <a name="properties"></a><span data-ttu-id="b9569-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9569-140">Properties</span></span>
| <span data-ttu-id="b9569-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9569-141">Property</span></span>     | <span data-ttu-id="b9569-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9569-142">Type</span></span>        | <span data-ttu-id="b9569-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9569-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b9569-144">id</span><span class="sxs-lookup"><span data-stu-id="b9569-144">id</span></span>|<span data-ttu-id="b9569-145">String</span><span class="sxs-lookup"><span data-stu-id="b9569-145">String</span></span>| <span data-ttu-id="b9569-146">O identificador do printerShare.</span><span class="sxs-lookup"><span data-stu-id="b9569-146">The printerShare's identifier.</span></span> <span data-ttu-id="b9569-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b9569-147">Read-only.</span></span>|
|<span data-ttu-id="b9569-148">name</span><span class="sxs-lookup"><span data-stu-id="b9569-148">name</span></span>|<span data-ttu-id="b9569-149">String</span><span class="sxs-lookup"><span data-stu-id="b9569-149">String</span></span>|<span data-ttu-id="b9569-150">O nome do compartilhamento de impressora que os clientes de impressão devem exibir.</span><span class="sxs-lookup"><span data-stu-id="b9569-150">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="b9569-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9569-151">createdDateTime</span></span>|<span data-ttu-id="b9569-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9569-152">DateTimeOffset</span></span>|<span data-ttu-id="b9569-153">O DateTimeOffset quando o compartilhamento da impressora foi criado.</span><span class="sxs-lookup"><span data-stu-id="b9569-153">The DateTimeOffset when the printer share was created.</span></span> <span data-ttu-id="b9569-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b9569-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9569-155">Relações</span><span class="sxs-lookup"><span data-stu-id="b9569-155">Relationships</span></span>
| <span data-ttu-id="b9569-156">Relação</span><span class="sxs-lookup"><span data-stu-id="b9569-156">Relationship</span></span> | <span data-ttu-id="b9569-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9569-157">Type</span></span>        | <span data-ttu-id="b9569-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9569-158">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b9569-159">impressora</span><span class="sxs-lookup"><span data-stu-id="b9569-159">printer</span></span>|[<span data-ttu-id="b9569-160">impressora</span><span class="sxs-lookup"><span data-stu-id="b9569-160">printer</span></span>](printer.md)|<span data-ttu-id="b9569-161">A impressora à qual esse compartilhamento de impressora está relacionado.</span><span class="sxs-lookup"><span data-stu-id="b9569-161">The printer that this printer share is related to.</span></span> |
|<span data-ttu-id="b9569-162">allowedUsers</span><span class="sxs-lookup"><span data-stu-id="b9569-162">allowedUsers</span></span>|<span data-ttu-id="b9569-163">coleção [UserIdentity](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="b9569-163">[userIdentity](useridentity.md) collection</span></span>|<span data-ttu-id="b9569-164">Os usuários que têm acesso à impressão usando a impressora.</span><span class="sxs-lookup"><span data-stu-id="b9569-164">The users who have access to print using the printer.</span></span>|
|<span data-ttu-id="b9569-165">allowedGroups</span><span class="sxs-lookup"><span data-stu-id="b9569-165">allowedGroups</span></span>|[<span data-ttu-id="b9569-166">identity</span><span class="sxs-lookup"><span data-stu-id="b9569-166">identity</span></span>](identity.md)|<span data-ttu-id="b9569-167">Os grupos cujos usuários têm acesso para imprimir usando a impressora.</span><span class="sxs-lookup"><span data-stu-id="b9569-167">The groups whose users have access to print using the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9569-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9569-168">JSON representation</span></span>

<span data-ttu-id="b9569-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9569-169">The following is a JSON representation of the resource.</span></span>

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
