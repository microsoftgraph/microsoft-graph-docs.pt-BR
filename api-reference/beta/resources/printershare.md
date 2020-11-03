---
title: tipo de recurso printerShare
description: Representa uma impressora que pretende ser detectável por usuários e por aplicativos de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 4fc729a41105340cc4066ee238c8d1ace3490765
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848223"
---
# <a name="printershare-resource-type"></a><span data-ttu-id="b53e7-103">tipo de recurso printerShare</span><span class="sxs-lookup"><span data-stu-id="b53e7-103">printerShare resource type</span></span>

<span data-ttu-id="b53e7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b53e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b53e7-105">Representa uma impressora que pretende ser detectável por usuários e por aplicativos de impressão.</span><span class="sxs-lookup"><span data-stu-id="b53e7-105">Represents a printer that is intended to be discoverable by users and printing applications.</span></span>

## <a name="methods"></a><span data-ttu-id="b53e7-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b53e7-106">Methods</span></span>

| <span data-ttu-id="b53e7-107">Método</span><span class="sxs-lookup"><span data-stu-id="b53e7-107">Method</span></span>       | <span data-ttu-id="b53e7-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b53e7-108">Return Type</span></span> | <span data-ttu-id="b53e7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b53e7-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b53e7-110">List</span><span class="sxs-lookup"><span data-stu-id="b53e7-110">List</span></span>](../api/print-list-shares.md) | <span data-ttu-id="b53e7-111">coleção [printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="b53e7-111">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="b53e7-112">Obtenha uma lista de compartilhamentos de impressora no locatário.</span><span class="sxs-lookup"><span data-stu-id="b53e7-112">Get a list of printer shares in the tenant.</span></span> |
| [<span data-ttu-id="b53e7-113">Get</span><span class="sxs-lookup"><span data-stu-id="b53e7-113">Get</span></span>](../api/printershare-get.md) | [<span data-ttu-id="b53e7-114">printerShare</span><span class="sxs-lookup"><span data-stu-id="b53e7-114">printerShare</span></span>](printershare.md) | <span data-ttu-id="b53e7-115">Ler propriedades e relações de um objeto **printerShare** .</span><span class="sxs-lookup"><span data-stu-id="b53e7-115">Read properties and relationships of a **printerShare** object.</span></span> |
| [<span data-ttu-id="b53e7-116">Update</span><span class="sxs-lookup"><span data-stu-id="b53e7-116">Update</span></span>](../api/printershare-update.md) | [<span data-ttu-id="b53e7-117">printerShare</span><span class="sxs-lookup"><span data-stu-id="b53e7-117">printerShare</span></span>](printershare.md) | <span data-ttu-id="b53e7-118">Atualizar um objeto **printerShare** .</span><span class="sxs-lookup"><span data-stu-id="b53e7-118">Update a **printerShare** object.</span></span> |
| [<span data-ttu-id="b53e7-119">Delete</span><span class="sxs-lookup"><span data-stu-id="b53e7-119">Delete</span></span>](../api/printershare-delete.md) | <span data-ttu-id="b53e7-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b53e7-120">None</span></span> | <span data-ttu-id="b53e7-121">Descompartilhar uma impressora.</span><span class="sxs-lookup"><span data-stu-id="b53e7-121">Unshare a printer.</span></span> |
| [<span data-ttu-id="b53e7-122">Listar trabalhos</span><span class="sxs-lookup"><span data-stu-id="b53e7-122">List jobs</span></span>](../api/printershare-list-jobs.md) | <span data-ttu-id="b53e7-123">coleção [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="b53e7-123">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="b53e7-124">Obtenha uma lista de trabalhos de impressão que são enfileirados para processamento pelo printerShare.</span><span class="sxs-lookup"><span data-stu-id="b53e7-124">Get a list of print jobs that are queued for processing by the printerShare.</span></span> |
| [<span data-ttu-id="b53e7-125">Criar trabalho</span><span class="sxs-lookup"><span data-stu-id="b53e7-125">Create job</span></span>](../api/printershare-post-jobs.md) | [<span data-ttu-id="b53e7-126">Impressão</span><span class="sxs-lookup"><span data-stu-id="b53e7-126">printJob</span></span>](printjob.md) | <span data-ttu-id="b53e7-127">Criar um novo trabalho de impressão para o printerShare.</span><span class="sxs-lookup"><span data-stu-id="b53e7-127">Create a new print job for the printerShare.</span></span> <span data-ttu-id="b53e7-128">Para começar a imprimir o trabalho, use [Iniciar](../api/printjob-start.md).</span><span class="sxs-lookup"><span data-stu-id="b53e7-128">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="b53e7-129">Listar allowedUsers</span><span class="sxs-lookup"><span data-stu-id="b53e7-129">List allowedUsers</span></span>](../api/printershare-list-allowedusers.md) | <span data-ttu-id="b53e7-130">coleção [printUserIdentity](printuseridentity.md)</span><span class="sxs-lookup"><span data-stu-id="b53e7-130">[printUserIdentity](printuseridentity.md) collection</span></span> | <span data-ttu-id="b53e7-131">Recupere uma lista de usuários que receberam acesso para enviar trabalhos de impressão para o compartilhamento de impressora associado.</span><span class="sxs-lookup"><span data-stu-id="b53e7-131">Retrieve a list of users who have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="b53e7-132">Adicionar allowedUser</span><span class="sxs-lookup"><span data-stu-id="b53e7-132">Add allowedUser</span></span>](../api/printershare-post-allowedusers.md) | <span data-ttu-id="b53e7-133">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b53e7-133">None</span></span> | <span data-ttu-id="b53e7-134">Conceda ao usuário especificado o acesso ao envio de trabalhos de impressão para o compartilhamento de impressora associado.</span><span class="sxs-lookup"><span data-stu-id="b53e7-134">Grant the specified user access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="b53e7-135">Remover allowedUser</span><span class="sxs-lookup"><span data-stu-id="b53e7-135">Remove allowedUser</span></span>](../api/printershare-delete-alloweduser.md) | <span data-ttu-id="b53e7-136">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b53e7-136">None</span></span> | <span data-ttu-id="b53e7-137">Revoga o acesso ao compartilhamento de impressora do usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="b53e7-137">Revoke printer share access from the specified user.</span></span> |
| [<span data-ttu-id="b53e7-138">Listar allowedGroups</span><span class="sxs-lookup"><span data-stu-id="b53e7-138">List allowedGroups</span></span>](../api/printershare-list-allowedgroups.md) | <span data-ttu-id="b53e7-139">coleção [Multiidentity](printidentity.md)</span><span class="sxs-lookup"><span data-stu-id="b53e7-139">[printIdentity](printidentity.md) collection</span></span> | <span data-ttu-id="b53e7-140">Recupere uma lista de grupos aos quais foi concedido acesso para enviar trabalhos de impressão ao compartilhamento de impressora associado.</span><span class="sxs-lookup"><span data-stu-id="b53e7-140">Retrieve a list of groups that have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="b53e7-141">Adicionar allowedGroup</span><span class="sxs-lookup"><span data-stu-id="b53e7-141">Add allowedGroup</span></span>](../api/printershare-post-allowedgroups.md) | <span data-ttu-id="b53e7-142">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b53e7-142">None</span></span> | <span data-ttu-id="b53e7-143">Conceda ao grupo especificado o acesso ao envio de trabalhos de impressão para o compartilhamento de impressora associado.</span><span class="sxs-lookup"><span data-stu-id="b53e7-143">Grant the specified group access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="b53e7-144">Remover allowedGroup</span><span class="sxs-lookup"><span data-stu-id="b53e7-144">Remove allowedGroup</span></span>](../api/printershare-delete-allowedgroup.md) | <span data-ttu-id="b53e7-145">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b53e7-145">None</span></span> | <span data-ttu-id="b53e7-146">Revoga o acesso ao compartilhamento de impressora do grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="b53e7-146">Revoke printer share access from the specified group.</span></span> |

## <a name="properties"></a><span data-ttu-id="b53e7-147">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b53e7-147">Properties</span></span>
| <span data-ttu-id="b53e7-148">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b53e7-148">Property</span></span>     | <span data-ttu-id="b53e7-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="b53e7-149">Type</span></span>        | <span data-ttu-id="b53e7-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="b53e7-150">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b53e7-151">id</span><span class="sxs-lookup"><span data-stu-id="b53e7-151">id</span></span>|<span data-ttu-id="b53e7-152">String</span><span class="sxs-lookup"><span data-stu-id="b53e7-152">String</span></span>| <span data-ttu-id="b53e7-153">O identificador do printerShare.</span><span class="sxs-lookup"><span data-stu-id="b53e7-153">The printerShare's identifier.</span></span> <span data-ttu-id="b53e7-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b53e7-154">Read-only.</span></span>|
|<span data-ttu-id="b53e7-155">displayName</span><span class="sxs-lookup"><span data-stu-id="b53e7-155">displayName</span></span>|<span data-ttu-id="b53e7-156">String</span><span class="sxs-lookup"><span data-stu-id="b53e7-156">String</span></span>|<span data-ttu-id="b53e7-157">O nome do compartilhamento de impressora que os clientes de impressão devem exibir.</span><span class="sxs-lookup"><span data-stu-id="b53e7-157">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="b53e7-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b53e7-158">createdDateTime</span></span>|<span data-ttu-id="b53e7-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b53e7-159">DateTimeOffset</span></span>|<span data-ttu-id="b53e7-160">O DateTimeOffset quando o compartilhamento da impressora foi criado.</span><span class="sxs-lookup"><span data-stu-id="b53e7-160">The DateTimeOffset when the printer share was created.</span></span> <span data-ttu-id="b53e7-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b53e7-161">Read-only.</span></span>|
|<span data-ttu-id="b53e7-162">fabricante</span><span class="sxs-lookup"><span data-stu-id="b53e7-162">manufacturer</span></span>|<span data-ttu-id="b53e7-163">String</span><span class="sxs-lookup"><span data-stu-id="b53e7-163">String</span></span>|<span data-ttu-id="b53e7-164">O fabricante relatado pela impressora associada a este compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="b53e7-164">The manufacturer reported by the printer associated with this printer share.</span></span> <span data-ttu-id="b53e7-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b53e7-165">Read-only.</span></span>|
|<span data-ttu-id="b53e7-166">modelo</span><span class="sxs-lookup"><span data-stu-id="b53e7-166">model</span></span>|<span data-ttu-id="b53e7-167">String</span><span class="sxs-lookup"><span data-stu-id="b53e7-167">String</span></span>|<span data-ttu-id="b53e7-168">O nome do modelo relatado pela impressora associada a este compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="b53e7-168">The model name reported by the printer associated with this printer share.</span></span> <span data-ttu-id="b53e7-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b53e7-169">Read-only.</span></span>|
|<span data-ttu-id="b53e7-170">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="b53e7-170">isAcceptingJobs</span></span>|<span data-ttu-id="b53e7-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="b53e7-171">Boolean</span></span>|<span data-ttu-id="b53e7-172">Se a impressora associada a este compartilhamento de impressora está atualmente aceitando novos trabalhos de impressão.</span><span class="sxs-lookup"><span data-stu-id="b53e7-172">Whether the printer associated with this printer share is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="b53e7-173">defaults</span><span class="sxs-lookup"><span data-stu-id="b53e7-173">defaults</span></span>|[<span data-ttu-id="b53e7-174">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="b53e7-174">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="b53e7-175">As configurações de impressão padrão da impressora associadas a este compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="b53e7-175">The default print settings of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="b53e7-176">capabilities</span><span class="sxs-lookup"><span data-stu-id="b53e7-176">capabilities</span></span>|[<span data-ttu-id="b53e7-177">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="b53e7-177">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="b53e7-178">Os recursos da impressora associada a este compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="b53e7-178">The capabilities of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="b53e7-179">location</span><span class="sxs-lookup"><span data-stu-id="b53e7-179">location</span></span>|[<span data-ttu-id="b53e7-180">printerLocation</span><span class="sxs-lookup"><span data-stu-id="b53e7-180">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="b53e7-181">O local físico e/ou organizacional da impressora associado a este compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="b53e7-181">The physical and/or organizational location of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="b53e7-182">status</span><span class="sxs-lookup"><span data-stu-id="b53e7-182">status</span></span>|[<span data-ttu-id="b53e7-183">printerStatus</span><span class="sxs-lookup"><span data-stu-id="b53e7-183">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="b53e7-184">O status de processamento, incluindo qualquer erro, da impressora associada a este compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="b53e7-184">The processing status, including any errors, of the printer associated with this printer share.</span></span> <span data-ttu-id="b53e7-185">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b53e7-185">Read-only.</span></span>|
|<span data-ttu-id="b53e7-186">allowAllUsers</span><span class="sxs-lookup"><span data-stu-id="b53e7-186">allowAllUsers</span></span>|<span data-ttu-id="b53e7-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="b53e7-187">Boolean</span></span>|<span data-ttu-id="b53e7-188">Se true, todos os usuários e grupos terão acesso a esse compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="b53e7-188">If true, all users and groups will be granted access to this printer share.</span></span> <span data-ttu-id="b53e7-189">Isso substitui as listas de permissões definidas pelas propriedades de navegação **allowedUsers** e **allowedGroups** .</span><span class="sxs-lookup"><span data-stu-id="b53e7-189">This supersedes the allow lists defined by the **allowedUsers** and **allowedGroups** navigation properties.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b53e7-190">Relações</span><span class="sxs-lookup"><span data-stu-id="b53e7-190">Relationships</span></span>
| <span data-ttu-id="b53e7-191">Relação</span><span class="sxs-lookup"><span data-stu-id="b53e7-191">Relationship</span></span> | <span data-ttu-id="b53e7-192">Tipo</span><span class="sxs-lookup"><span data-stu-id="b53e7-192">Type</span></span>        | <span data-ttu-id="b53e7-193">Descrição</span><span class="sxs-lookup"><span data-stu-id="b53e7-193">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b53e7-194">impressora</span><span class="sxs-lookup"><span data-stu-id="b53e7-194">printer</span></span>|[<span data-ttu-id="b53e7-195">impressora</span><span class="sxs-lookup"><span data-stu-id="b53e7-195">printer</span></span>](printer.md)|<span data-ttu-id="b53e7-196">A impressora à qual esse compartilhamento de impressora está relacionado.</span><span class="sxs-lookup"><span data-stu-id="b53e7-196">The printer that this printer share is related to.</span></span> |
|<span data-ttu-id="b53e7-197">allowedUsers</span><span class="sxs-lookup"><span data-stu-id="b53e7-197">allowedUsers</span></span>|<span data-ttu-id="b53e7-198">coleção [printUserIdentity](printuseridentity.md)</span><span class="sxs-lookup"><span data-stu-id="b53e7-198">[printUserIdentity](printuseridentity.md) collection</span></span>|<span data-ttu-id="b53e7-199">Os usuários que têm acesso à impressão usando a impressora.</span><span class="sxs-lookup"><span data-stu-id="b53e7-199">The users who have access to print using the printer.</span></span>|
|<span data-ttu-id="b53e7-200">allowedGroups</span><span class="sxs-lookup"><span data-stu-id="b53e7-200">allowedGroups</span></span>|[<span data-ttu-id="b53e7-201">multiidentity</span><span class="sxs-lookup"><span data-stu-id="b53e7-201">printIdentity</span></span>](printidentity.md)|<span data-ttu-id="b53e7-202">Os grupos cujos usuários têm acesso para imprimir usando a impressora.</span><span class="sxs-lookup"><span data-stu-id="b53e7-202">The groups whose users have access to print using the printer.</span></span>|
|<span data-ttu-id="b53e7-203">jobs</span><span class="sxs-lookup"><span data-stu-id="b53e7-203">jobs</span></span>|<span data-ttu-id="b53e7-204">coleção [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="b53e7-204">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="b53e7-205">A lista de trabalhos que estão na fila para impressão pela impressora associada a este compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="b53e7-205">The list of jobs that are queued for printing by the printer associated with this printer share.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b53e7-206">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b53e7-206">JSON representation</span></span>

<span data-ttu-id="b53e7-207">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b53e7-207">The following is a JSON representation of the resource.</span></span>

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
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "createdDateTime": "String (timestamp)",
  "isAcceptingJobs": true,
  "allowAllUsers": false,
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "status": {"@odata.type": "microsoft.graph.printerStatus"},
  "defaults": {"@odata.type": "microsoft.graph.printerDefaults"},
  "capabilities": {"@odata.type": "microsoft.graph.printerCapabilities"}
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


