---
title: tipo de recurso connectedOrganization
description: No Azure AD pretitulation Management, uma organização conectada é uma referência a um diretório ou domínio de outra organização cujos usuários podem solicitar acesso.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5356a48aae90f22fdd54a54ed5fe7132598b9d42
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757290"
---
# <a name="connectedorganization-resource-type"></a><span data-ttu-id="cc2ae-103">tipo de recurso connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="cc2ae-103">connectedOrganization resource type</span></span>

<span data-ttu-id="cc2ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc2ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc2ae-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma organização conectada é uma referência a um diretório ou domínio de outra organização cujos usuários podem solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-105">In [Azure AD entitlement management](entitlementmanagement-root.md), a connected organization is a reference to a directory or domain of another organization whose users can request access.</span></span>

## <a name="methods"></a><span data-ttu-id="cc2ae-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="cc2ae-106">Methods</span></span>

|<span data-ttu-id="cc2ae-107">Método</span><span class="sxs-lookup"><span data-stu-id="cc2ae-107">Method</span></span>|<span data-ttu-id="cc2ae-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cc2ae-108">Return type</span></span>|<span data-ttu-id="cc2ae-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc2ae-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cc2ae-110">Listar connectedOrganizations</span><span class="sxs-lookup"><span data-stu-id="cc2ae-110">List connectedOrganizations</span></span>](../api/connectedorganization-list.md) | <span data-ttu-id="cc2ae-111">coleção [connectedOrganization](connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="cc2ae-111">[connectedOrganization](connectedorganization.md) collection</span></span> | <span data-ttu-id="cc2ae-112">Recupere uma lista de objetos connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-112">Retrieve a list of connectedOrganization objects.</span></span> |
|[<span data-ttu-id="cc2ae-113">Criar connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="cc2ae-113">Create connectedOrganization</span></span>](../api/connectedorganization-post.md) | [<span data-ttu-id="cc2ae-114">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="cc2ae-114">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="cc2ae-115">Criar um novo objeto connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-115">Create a new connectedOrganization object.</span></span> |
|[<span data-ttu-id="cc2ae-116">Obter connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="cc2ae-116">Get connectedOrganization</span></span>](../api/connectedorganization-get.md) | [<span data-ttu-id="cc2ae-117">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="cc2ae-117">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="cc2ae-118">Ler propriedades e relações de um objeto connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-118">Read properties and relationships of a connectedOrganization object.</span></span> |
|[<span data-ttu-id="cc2ae-119">Atualizar connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="cc2ae-119">Update connectedOrganization</span></span>](../api/connectedorganization-update.md) | | <span data-ttu-id="cc2ae-120">Atualizar um connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-120">Update a connectedOrganization.</span></span> |
|[<span data-ttu-id="cc2ae-121">Excluir connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="cc2ae-121">Delete connectedOrganization</span></span>](../api/connectedorganization-delete.md) |<span data-ttu-id="cc2ae-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cc2ae-122">None</span></span> | <span data-ttu-id="cc2ae-123">Excluir um connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-123">Delete a connectedOrganization.</span></span> |
|[<span data-ttu-id="cc2ae-124">Listar internalSponsors</span><span class="sxs-lookup"><span data-stu-id="cc2ae-124">List internalSponsors</span></span>](../api/connectedorganization-list-internalsponsors.md) | <span data-ttu-id="cc2ae-125">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="cc2ae-125">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="cc2ae-126">Recupere uma lista de patrocinadores internos de um connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-126">Retrieve a list of a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="cc2ae-127">Listar externalSponsors</span><span class="sxs-lookup"><span data-stu-id="cc2ae-127">List externalSponsors</span></span>](../api/connectedorganization-list-externalsponsors.md) | <span data-ttu-id="cc2ae-128">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="cc2ae-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="cc2ae-129">Recupere uma lista de patrocinadores externos de um connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-129">Retrieve a list of a connectedOrganization's external sponsors.</span></span> |
|[<span data-ttu-id="cc2ae-130">Adicionar internalSponsors</span><span class="sxs-lookup"><span data-stu-id="cc2ae-130">Add internalSponsors</span></span>](../api/connectedorganization-post-internalsponsors.md) | <span data-ttu-id="cc2ae-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cc2ae-131">None</span></span> | <span data-ttu-id="cc2ae-132">Adicionar um usuário ou grupo aos patrocinadores internos de um connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-132">Add a user or group to a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="cc2ae-133">Adicionar externalSponsors</span><span class="sxs-lookup"><span data-stu-id="cc2ae-133">Add externalSponsors</span></span>](../api/connectedorganization-post-externalsponsors.md) | <span data-ttu-id="cc2ae-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cc2ae-134">None</span></span> | <span data-ttu-id="cc2ae-135">Adicionar um usuário ou grupo aos patrocinadores externos de um connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-135">Add a user or group to a connectedOrganization's external sponsors.</span></span> |
|[<span data-ttu-id="cc2ae-136">Remover internalSponsors</span><span class="sxs-lookup"><span data-stu-id="cc2ae-136">Remove internalSponsors</span></span>](../api/connectedorganization-delete-internalsponsors.md) | <span data-ttu-id="cc2ae-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cc2ae-137">None</span></span> | <span data-ttu-id="cc2ae-138">Remover um usuário ou grupo dos patrocinadores internos de um connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-138">Remove a user or group from a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="cc2ae-139">Remover externalSponsors</span><span class="sxs-lookup"><span data-stu-id="cc2ae-139">Remove externalSponsors</span></span>](../api/connectedorganization-delete-externalsponsors.md) | <span data-ttu-id="cc2ae-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cc2ae-140">None</span></span> | <span data-ttu-id="cc2ae-141">Remover um usuário ou grupo dos patrocinadores externos de um connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-141">Remove a user or group from a connectedOrganization's external sponsors.</span></span> |

## <a name="properties"></a><span data-ttu-id="cc2ae-142">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cc2ae-142">Properties</span></span>

|<span data-ttu-id="cc2ae-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc2ae-143">Property</span></span>|<span data-ttu-id="cc2ae-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc2ae-144">Type</span></span>|<span data-ttu-id="cc2ae-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc2ae-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc2ae-146">createdBy</span><span class="sxs-lookup"><span data-stu-id="cc2ae-146">createdBy</span></span>|<span data-ttu-id="cc2ae-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc2ae-147">String</span></span>|<span data-ttu-id="cc2ae-148">UPN do usuário que criou este recurso.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-148">UPN of the user who created this resource.</span></span> <span data-ttu-id="cc2ae-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-149">Read-only.</span></span>|
|<span data-ttu-id="cc2ae-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc2ae-150">createdDateTime</span></span>|<span data-ttu-id="cc2ae-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc2ae-151">DateTimeOffset</span></span>|<span data-ttu-id="cc2ae-152">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-152">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cc2ae-153">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-153">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="cc2ae-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-154">Read-only.</span></span>|
|<span data-ttu-id="cc2ae-155">description</span><span class="sxs-lookup"><span data-stu-id="cc2ae-155">description</span></span>|<span data-ttu-id="cc2ae-156">String</span><span class="sxs-lookup"><span data-stu-id="cc2ae-156">String</span></span>|<span data-ttu-id="cc2ae-157">A descrição da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-157">The description of the connected organization.</span></span>|
|<span data-ttu-id="cc2ae-158">displayName</span><span class="sxs-lookup"><span data-stu-id="cc2ae-158">displayName</span></span>|<span data-ttu-id="cc2ae-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc2ae-159">String</span></span>|<span data-ttu-id="cc2ae-160">O nome de exibição da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-160">The display name of the connected organization.</span></span>|
|<span data-ttu-id="cc2ae-161">id</span><span class="sxs-lookup"><span data-stu-id="cc2ae-161">id</span></span>|<span data-ttu-id="cc2ae-162">String</span><span class="sxs-lookup"><span data-stu-id="cc2ae-162">String</span></span>| <span data-ttu-id="cc2ae-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-163">Read-only.</span></span>|
|<span data-ttu-id="cc2ae-164">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="cc2ae-164">modifiedBy</span></span>|<span data-ttu-id="cc2ae-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc2ae-165">String</span></span>|<span data-ttu-id="cc2ae-166">UPN do usuário que modificou este recurso pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-166">UPN of the user who last modified this resource.</span></span> <span data-ttu-id="cc2ae-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-167">Read-only.</span></span>|
|<span data-ttu-id="cc2ae-168">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc2ae-168">modifiedDateTime</span></span>|<span data-ttu-id="cc2ae-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc2ae-169">DateTimeOffset</span></span>|<span data-ttu-id="cc2ae-170">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-170">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cc2ae-171">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-171">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="cc2ae-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-172">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc2ae-173">Relações</span><span class="sxs-lookup"><span data-stu-id="cc2ae-173">Relationships</span></span>

|<span data-ttu-id="cc2ae-174">Relação</span><span class="sxs-lookup"><span data-stu-id="cc2ae-174">Relationship</span></span>|<span data-ttu-id="cc2ae-175">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc2ae-175">Type</span></span>|<span data-ttu-id="cc2ae-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc2ae-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc2ae-177">identitySources</span><span class="sxs-lookup"><span data-stu-id="cc2ae-177">identitySources</span></span>|<span data-ttu-id="cc2ae-178">coleção [identityry](identitySource.md)</span><span class="sxs-lookup"><span data-stu-id="cc2ae-178">[identitySource](identitySource.md) collection</span></span>| <span data-ttu-id="cc2ae-179">As fontes de identidade nesta organização conectada, uma de [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) ou [externalDomainFederation](externaldomainfederation.md).</span><span class="sxs-lookup"><span data-stu-id="cc2ae-179">The identity sources in this connected organization, one of [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) or [externalDomainFederation](externaldomainfederation.md).</span></span> <span data-ttu-id="cc2ae-180">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-180">Read-only.</span></span> <span data-ttu-id="cc2ae-181">Anulável.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-181">Nullable.</span></span>|
|<span data-ttu-id="cc2ae-182">internalSponsors</span><span class="sxs-lookup"><span data-stu-id="cc2ae-182">internalSponsors</span></span>| <span data-ttu-id="cc2ae-183">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="cc2ae-183">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="cc2ae-184">Anulável.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-184">Nullable.</span></span>|
|<span data-ttu-id="cc2ae-185">externalSponsors</span><span class="sxs-lookup"><span data-stu-id="cc2ae-185">externalSponsors</span></span>| <span data-ttu-id="cc2ae-186">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="cc2ae-186">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="cc2ae-187">Anulável.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-187">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc2ae-188">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc2ae-188">JSON representation</span></span>

<span data-ttu-id="cc2ae-189">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cc2ae-189">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.connectedOrganization",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "identitySources": [
    {
      "@odata.type": "microsoft.graph.azureActiveDirectoryTenant",
      "tenantId": "String (identifier)",
      "displayName": "String"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectedOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
