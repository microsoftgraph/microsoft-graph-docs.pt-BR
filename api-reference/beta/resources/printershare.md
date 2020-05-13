---
title: tipo de recurso printerShare
description: Representa uma impressora que pretende ser detectável por usuários e por aplicativos de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 5acbcdc58b730404a39af1f3069b3433fac54ed3
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217344"
---
# <a name="printershare-resource-type"></a><span data-ttu-id="1b378-103">tipo de recurso printerShare</span><span class="sxs-lookup"><span data-stu-id="1b378-103">printerShare resource type</span></span>

<span data-ttu-id="1b378-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b378-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b378-105">Representa uma impressora que pretende ser detectável por usuários e por aplicativos de impressão.</span><span class="sxs-lookup"><span data-stu-id="1b378-105">Represents a printer that is intended to be discoverable by users and printing applications.</span></span>

## <a name="methods"></a><span data-ttu-id="1b378-106">Methods</span><span class="sxs-lookup"><span data-stu-id="1b378-106">Methods</span></span>

| <span data-ttu-id="1b378-107">Método</span><span class="sxs-lookup"><span data-stu-id="1b378-107">Method</span></span>       | <span data-ttu-id="1b378-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1b378-108">Return Type</span></span> | <span data-ttu-id="1b378-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b378-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1b378-110">Listar</span><span class="sxs-lookup"><span data-stu-id="1b378-110">List</span></span>](../api/print-list-shares.md) | <span data-ttu-id="1b378-111">coleção [printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="1b378-111">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="1b378-112">Obtenha uma lista de compartilhamentos de impressora no locatário.</span><span class="sxs-lookup"><span data-stu-id="1b378-112">Get a list of printer shares in the tenant.</span></span> |
| [<span data-ttu-id="1b378-113">Get</span><span class="sxs-lookup"><span data-stu-id="1b378-113">Get</span></span>](../api/printershare-get.md) | [<span data-ttu-id="1b378-114">printerShare</span><span class="sxs-lookup"><span data-stu-id="1b378-114">printerShare</span></span>](printershare.md) | <span data-ttu-id="1b378-115">Ler propriedades e relações de um objeto **printerShare** .</span><span class="sxs-lookup"><span data-stu-id="1b378-115">Read properties and relationships of a **printerShare** object.</span></span> |
| [<span data-ttu-id="1b378-116">Update</span><span class="sxs-lookup"><span data-stu-id="1b378-116">Update</span></span>](../api/printershare-update.md) | [<span data-ttu-id="1b378-117">printerShare</span><span class="sxs-lookup"><span data-stu-id="1b378-117">printerShare</span></span>](printershare.md) | <span data-ttu-id="1b378-118">Atualizar um objeto **printerShare** .</span><span class="sxs-lookup"><span data-stu-id="1b378-118">Update a **printerShare** object.</span></span> |
| [<span data-ttu-id="1b378-119">Delete</span><span class="sxs-lookup"><span data-stu-id="1b378-119">Delete</span></span>](../api/printershare-delete.md) | <span data-ttu-id="1b378-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1b378-120">None</span></span> | <span data-ttu-id="1b378-121">Descompartilhar uma impressora.</span><span class="sxs-lookup"><span data-stu-id="1b378-121">Unshare a printer.</span></span> |
| [<span data-ttu-id="1b378-122">Listar allowedUsers</span><span class="sxs-lookup"><span data-stu-id="1b378-122">List allowedUsers</span></span>](../api/printershare-list-allowedusers.md) | <span data-ttu-id="1b378-123">coleção [printUserIdentity](printuseridentity.md)</span><span class="sxs-lookup"><span data-stu-id="1b378-123">[printUserIdentity](printuseridentity.md) collection</span></span> | <span data-ttu-id="1b378-124">Recupere uma lista de usuários que receberam acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado.</span><span class="sxs-lookup"><span data-stu-id="1b378-124">Retrieve a list of users who have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="1b378-125">Adicionar allowedUser</span><span class="sxs-lookup"><span data-stu-id="1b378-125">Add allowedUser</span></span>](../api/printershare-post-allowedusers.md) | <span data-ttu-id="1b378-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1b378-126">None</span></span> | <span data-ttu-id="1b378-127">Conceda ao usuário especificado o acesso ao envio de trabalhos de impressão para o compartilhamento de impressora associado.</span><span class="sxs-lookup"><span data-stu-id="1b378-127">Grant the specified user access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="1b378-128">Remover allowedUser</span><span class="sxs-lookup"><span data-stu-id="1b378-128">Remove allowedUser</span></span>](../api/printershare-delete-alloweduser.md) | <span data-ttu-id="1b378-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1b378-129">None</span></span> | <span data-ttu-id="1b378-130">Revoga o acesso ao compartilhamento de impressora do usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="1b378-130">Revoke printer share access from the specified user.</span></span> |
| [<span data-ttu-id="1b378-131">Listar allowedGroups</span><span class="sxs-lookup"><span data-stu-id="1b378-131">List allowedGroups</span></span>](../api/printershare-list-allowedgroups.md) | <span data-ttu-id="1b378-132">coleção [Multiidentity](printidentity.md)</span><span class="sxs-lookup"><span data-stu-id="1b378-132">[printIdentity](printidentity.md) collection</span></span> | <span data-ttu-id="1b378-133">Recupere uma lista de grupos aos quais foi concedido acesso para enviar trabalhos de impressão ao compartilhamento de impressora associado.</span><span class="sxs-lookup"><span data-stu-id="1b378-133">Retrieve a list of groups that have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="1b378-134">Adicionar allowedGroup</span><span class="sxs-lookup"><span data-stu-id="1b378-134">Add allowedGroup</span></span>](../api/printershare-post-allowedgroups.md) | <span data-ttu-id="1b378-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1b378-135">None</span></span> | <span data-ttu-id="1b378-136">Conceda ao grupo especificado o acesso ao envio de trabalhos de impressão para o compartilhamento de impressora associado.</span><span class="sxs-lookup"><span data-stu-id="1b378-136">Grant the specified group access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="1b378-137">Remover allowedGroup</span><span class="sxs-lookup"><span data-stu-id="1b378-137">Remove allowedGroup</span></span>](../api/printershare-delete-allowedgroup.md) | <span data-ttu-id="1b378-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1b378-138">None</span></span> | <span data-ttu-id="1b378-139">Revoga o acesso ao compartilhamento de impressora do grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="1b378-139">Revoke printer share access from the specified group.</span></span> |

## <a name="properties"></a><span data-ttu-id="1b378-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b378-140">Properties</span></span>
| <span data-ttu-id="1b378-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b378-141">Property</span></span>     | <span data-ttu-id="1b378-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b378-142">Type</span></span>        | <span data-ttu-id="1b378-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b378-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1b378-144">id</span><span class="sxs-lookup"><span data-stu-id="1b378-144">id</span></span>|<span data-ttu-id="1b378-145">String</span><span class="sxs-lookup"><span data-stu-id="1b378-145">String</span></span>| <span data-ttu-id="1b378-146">O identificador do printerShare.</span><span class="sxs-lookup"><span data-stu-id="1b378-146">The printerShare's identifier.</span></span> <span data-ttu-id="1b378-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b378-147">Read-only.</span></span>|
|<span data-ttu-id="1b378-148">displayName</span><span class="sxs-lookup"><span data-stu-id="1b378-148">displayName</span></span>|<span data-ttu-id="1b378-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b378-149">String</span></span>|<span data-ttu-id="1b378-150">O nome do compartilhamento de impressora que os clientes de impressão devem exibir.</span><span class="sxs-lookup"><span data-stu-id="1b378-150">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="1b378-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b378-151">createdDateTime</span></span>|<span data-ttu-id="1b378-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b378-152">DateTimeOffset</span></span>|<span data-ttu-id="1b378-153">O DateTimeOffset quando o compartilhamento da impressora foi criado.</span><span class="sxs-lookup"><span data-stu-id="1b378-153">The DateTimeOffset when the printer share was created.</span></span> <span data-ttu-id="1b378-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b378-154">Read-only.</span></span>|
|<span data-ttu-id="1b378-155">fabricante</span><span class="sxs-lookup"><span data-stu-id="1b378-155">manufacturer</span></span>|<span data-ttu-id="1b378-156">String</span><span class="sxs-lookup"><span data-stu-id="1b378-156">String</span></span>|<span data-ttu-id="1b378-157">O fabricante relatado pela impressora associada a este compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="1b378-157">The manufacturer reported by the printer associated with this printer share.</span></span> <span data-ttu-id="1b378-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b378-158">Read-only.</span></span>|
|<span data-ttu-id="1b378-159">modelo</span><span class="sxs-lookup"><span data-stu-id="1b378-159">model</span></span>|<span data-ttu-id="1b378-160">String</span><span class="sxs-lookup"><span data-stu-id="1b378-160">String</span></span>|<span data-ttu-id="1b378-161">O nome do modelo relatado pela impressora associada a este compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="1b378-161">The model name reported by the printer associated with this printer share.</span></span> <span data-ttu-id="1b378-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b378-162">Read-only.</span></span>|
|<span data-ttu-id="1b378-163">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="1b378-163">isAcceptingJobs</span></span>|<span data-ttu-id="1b378-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b378-164">Boolean</span></span>|<span data-ttu-id="1b378-165">Se a impressora associada a este compartilhamento de impressora está atualmente aceitando novos trabalhos de impressão.</span><span class="sxs-lookup"><span data-stu-id="1b378-165">Whether the printer associated with this printer share is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="1b378-166">padrões</span><span class="sxs-lookup"><span data-stu-id="1b378-166">defaults</span></span>|[<span data-ttu-id="1b378-167">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="1b378-167">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="1b378-168">As configurações de impressão padrão da impressora associadas a este compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="1b378-168">The default print settings of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="1b378-169">capabilities</span><span class="sxs-lookup"><span data-stu-id="1b378-169">capabilities</span></span>|[<span data-ttu-id="1b378-170">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="1b378-170">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="1b378-171">Os recursos da impressora associada a este compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="1b378-171">The capabilities of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="1b378-172">location</span><span class="sxs-lookup"><span data-stu-id="1b378-172">location</span></span>|[<span data-ttu-id="1b378-173">printerLocation</span><span class="sxs-lookup"><span data-stu-id="1b378-173">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="1b378-174">O local físico e/ou organizacional da impressora associado a este compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="1b378-174">The physical and/or organizational location of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="1b378-175">status</span><span class="sxs-lookup"><span data-stu-id="1b378-175">status</span></span>|[<span data-ttu-id="1b378-176">printerStatus</span><span class="sxs-lookup"><span data-stu-id="1b378-176">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="1b378-177">O status de processamento, incluindo qualquer erro, da impressora associada a este compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="1b378-177">The processing status, including any errors, of the printer associated with this printer share.</span></span> <span data-ttu-id="1b378-178">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b378-178">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b378-179">Relações</span><span class="sxs-lookup"><span data-stu-id="1b378-179">Relationships</span></span>
| <span data-ttu-id="1b378-180">Relação</span><span class="sxs-lookup"><span data-stu-id="1b378-180">Relationship</span></span> | <span data-ttu-id="1b378-181">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b378-181">Type</span></span>        | <span data-ttu-id="1b378-182">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b378-182">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1b378-183">impressora</span><span class="sxs-lookup"><span data-stu-id="1b378-183">printer</span></span>|[<span data-ttu-id="1b378-184">impressora</span><span class="sxs-lookup"><span data-stu-id="1b378-184">printer</span></span>](printer.md)|<span data-ttu-id="1b378-185">A impressora à qual esse compartilhamento de impressora está relacionado.</span><span class="sxs-lookup"><span data-stu-id="1b378-185">The printer that this printer share is related to.</span></span> |
|<span data-ttu-id="1b378-186">allowedUsers</span><span class="sxs-lookup"><span data-stu-id="1b378-186">allowedUsers</span></span>|<span data-ttu-id="1b378-187">coleção [printUserIdentity](printuseridentity.md)</span><span class="sxs-lookup"><span data-stu-id="1b378-187">[printUserIdentity](printuseridentity.md) collection</span></span>|<span data-ttu-id="1b378-188">Os usuários que têm acesso à impressão usando a impressora.</span><span class="sxs-lookup"><span data-stu-id="1b378-188">The users who have access to print using the printer.</span></span>|
|<span data-ttu-id="1b378-189">allowedGroups</span><span class="sxs-lookup"><span data-stu-id="1b378-189">allowedGroups</span></span>|[<span data-ttu-id="1b378-190">multiidentity</span><span class="sxs-lookup"><span data-stu-id="1b378-190">printIdentity</span></span>](printidentity.md)|<span data-ttu-id="1b378-191">Os grupos cujos usuários têm acesso para imprimir usando a impressora.</span><span class="sxs-lookup"><span data-stu-id="1b378-191">The groups whose users have access to print using the printer.</span></span>|
|<span data-ttu-id="1b378-192">serviços</span><span class="sxs-lookup"><span data-stu-id="1b378-192">jobs</span></span>|<span data-ttu-id="1b378-193">coleção [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="1b378-193">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="1b378-194">A lista de trabalhos que estão na fila para impressão pela impressora associada a este compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="1b378-194">The list of jobs that are queued for printing by the printer associated with this printer share.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b378-195">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b378-195">JSON representation</span></span>

<span data-ttu-id="1b378-196">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1b378-196">The following is a JSON representation of the resource.</span></span>

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
