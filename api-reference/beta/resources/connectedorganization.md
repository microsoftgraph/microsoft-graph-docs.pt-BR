---
title: tipo de recurso connectedOrganization
description: No Azure AD pretitulation Management, uma organização conectada é uma referência a um diretório ou domínio de outra organização cujos usuários podem solicitar acesso.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 95cce32d4336c34a61d6845b74e6e428d1774d21
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027206"
---
# <a name="connectedorganization-resource-type"></a><span data-ttu-id="2e6ac-103">tipo de recurso connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="2e6ac-103">connectedOrganization resource type</span></span>

<span data-ttu-id="2e6ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e6ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e6ac-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma organização conectada é uma referência a um diretório ou domínio de outra organização cujos usuários podem solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-105">In [Azure AD entitlement management](entitlementmanagement-root.md), a connected organization is a reference to a directory or domain of another organization whose users can request access.</span></span>

## <a name="methods"></a><span data-ttu-id="2e6ac-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="2e6ac-106">Methods</span></span>

|<span data-ttu-id="2e6ac-107">Método</span><span class="sxs-lookup"><span data-stu-id="2e6ac-107">Method</span></span>|<span data-ttu-id="2e6ac-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2e6ac-108">Return type</span></span>|<span data-ttu-id="2e6ac-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e6ac-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2e6ac-110">Listar connectedOrganizations</span><span class="sxs-lookup"><span data-stu-id="2e6ac-110">List connectedOrganizations</span></span>](../api/connectedorganization-list.md) | <span data-ttu-id="2e6ac-111">coleção [connectedOrganization](connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="2e6ac-111">[connectedOrganization](connectedorganization.md) collection</span></span> | <span data-ttu-id="2e6ac-112">Recupere uma lista de objetos connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-112">Retrieve a list of connectedOrganization objects.</span></span> |
|[<span data-ttu-id="2e6ac-113">Criar connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="2e6ac-113">Create connectedOrganization</span></span>](../api/connectedorganization-post.md) | [<span data-ttu-id="2e6ac-114">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="2e6ac-114">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="2e6ac-115">Criar um novo objeto connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-115">Create a new connectedOrganization object.</span></span> |
|[<span data-ttu-id="2e6ac-116">Obter connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="2e6ac-116">Get connectedOrganization</span></span>](../api/connectedorganization-get.md) | [<span data-ttu-id="2e6ac-117">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="2e6ac-117">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="2e6ac-118">Ler propriedades e relações de um objeto connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-118">Read properties and relationships of a connectedOrganization object.</span></span> |
|[<span data-ttu-id="2e6ac-119">Atualizar connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="2e6ac-119">Update connectedOrganization</span></span>](../api/connectedorganization-update.md) | | <span data-ttu-id="2e6ac-120">Atualizar um connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-120">Update a connectedOrganization.</span></span> |
|[<span data-ttu-id="2e6ac-121">Excluir connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="2e6ac-121">Delete connectedOrganization</span></span>](../api/connectedorganization-delete.md) |<span data-ttu-id="2e6ac-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2e6ac-122">None</span></span> | <span data-ttu-id="2e6ac-123">Excluir um connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-123">Delete a connectedOrganization.</span></span> |
|[<span data-ttu-id="2e6ac-124">Listar internalSponsors</span><span class="sxs-lookup"><span data-stu-id="2e6ac-124">List internalSponsors</span></span>](../api/connectedorganization-list-internalsponsors.md) | <span data-ttu-id="2e6ac-125">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="2e6ac-125">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="2e6ac-126">Recupere uma lista de patrocinadores internos de um connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-126">Retrieve a list of a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="2e6ac-127">Listar externalSponsors</span><span class="sxs-lookup"><span data-stu-id="2e6ac-127">List externalSponsors</span></span>](../api/connectedorganization-list-externalsponsors.md) | <span data-ttu-id="2e6ac-128">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="2e6ac-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="2e6ac-129">Recupere uma lista de patrocinadores externos de um connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-129">Retrieve a list of a connectedOrganization's external sponsors.</span></span> |
|[<span data-ttu-id="2e6ac-130">Adicionar internalSponsors</span><span class="sxs-lookup"><span data-stu-id="2e6ac-130">Add internalSponsors</span></span>](../api/connectedorganization-post-internalsponsors.md) | <span data-ttu-id="2e6ac-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2e6ac-131">None</span></span> | <span data-ttu-id="2e6ac-132">Adicionar um usuário ou grupo aos patrocinadores internos de um connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-132">Add a user or group to a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="2e6ac-133">Adicionar externalSponsors</span><span class="sxs-lookup"><span data-stu-id="2e6ac-133">Add externalSponsors</span></span>](../api/connectedorganization-post-externalsponsors.md) | <span data-ttu-id="2e6ac-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2e6ac-134">None</span></span> | <span data-ttu-id="2e6ac-135">Adicionar um usuário ou grupo aos patrocinadores externos de um connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-135">Add a user or group to a connectedOrganization's external sponsors.</span></span> |
|[<span data-ttu-id="2e6ac-136">Remover internalSponsors</span><span class="sxs-lookup"><span data-stu-id="2e6ac-136">Remove internalSponsors</span></span>](../api/connectedorganization-delete-internalsponsors.md) | <span data-ttu-id="2e6ac-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2e6ac-137">None</span></span> | <span data-ttu-id="2e6ac-138">Remover um usuário ou grupo dos patrocinadores internos de um connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-138">Remove a user or group from a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="2e6ac-139">Remover externalSponsors</span><span class="sxs-lookup"><span data-stu-id="2e6ac-139">Remove externalSponsors</span></span>](../api/connectedorganization-delete-externalsponsors.md) | <span data-ttu-id="2e6ac-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2e6ac-140">None</span></span> | <span data-ttu-id="2e6ac-141">Remover um usuário ou grupo dos patrocinadores externos de um connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-141">Remove a user or group from a connectedOrganization's external sponsors.</span></span> |

## <a name="properties"></a><span data-ttu-id="2e6ac-142">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2e6ac-142">Properties</span></span>

|<span data-ttu-id="2e6ac-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e6ac-143">Property</span></span>|<span data-ttu-id="2e6ac-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e6ac-144">Type</span></span>|<span data-ttu-id="2e6ac-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e6ac-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e6ac-146">createdBy</span><span class="sxs-lookup"><span data-stu-id="2e6ac-146">createdBy</span></span>|<span data-ttu-id="2e6ac-147">String</span><span class="sxs-lookup"><span data-stu-id="2e6ac-147">String</span></span>|<span data-ttu-id="2e6ac-148">UPN do usuário que criou este recurso.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-148">UPN of the user who created this resource.</span></span> <span data-ttu-id="2e6ac-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-149">Read-only.</span></span>|
|<span data-ttu-id="2e6ac-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2e6ac-150">createdDateTime</span></span>|<span data-ttu-id="2e6ac-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e6ac-151">DateTimeOffset</span></span>|<span data-ttu-id="2e6ac-152">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-152">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2e6ac-153">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-153">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="2e6ac-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-154">Read-only.</span></span>|
|<span data-ttu-id="2e6ac-155">description</span><span class="sxs-lookup"><span data-stu-id="2e6ac-155">description</span></span>|<span data-ttu-id="2e6ac-156">String</span><span class="sxs-lookup"><span data-stu-id="2e6ac-156">String</span></span>|<span data-ttu-id="2e6ac-157">A descrição da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-157">The description of the connected organization.</span></span>|
|<span data-ttu-id="2e6ac-158">displayName</span><span class="sxs-lookup"><span data-stu-id="2e6ac-158">displayName</span></span>|<span data-ttu-id="2e6ac-159">String</span><span class="sxs-lookup"><span data-stu-id="2e6ac-159">String</span></span>|<span data-ttu-id="2e6ac-160">O nome de exibição da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-160">The display name of the connected organization.</span></span>|
|<span data-ttu-id="2e6ac-161">id</span><span class="sxs-lookup"><span data-stu-id="2e6ac-161">id</span></span>|<span data-ttu-id="2e6ac-162">String</span><span class="sxs-lookup"><span data-stu-id="2e6ac-162">String</span></span>| <span data-ttu-id="2e6ac-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-163">Read-only.</span></span>|
|<span data-ttu-id="2e6ac-164">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="2e6ac-164">modifiedBy</span></span>|<span data-ttu-id="2e6ac-165">String</span><span class="sxs-lookup"><span data-stu-id="2e6ac-165">String</span></span>|<span data-ttu-id="2e6ac-166">UPN do usuário que modificou este recurso pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-166">UPN of the user who last modified this resource.</span></span> <span data-ttu-id="2e6ac-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-167">Read-only.</span></span>|
|<span data-ttu-id="2e6ac-168">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e6ac-168">modifiedDateTime</span></span>|<span data-ttu-id="2e6ac-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e6ac-169">DateTimeOffset</span></span>|<span data-ttu-id="2e6ac-170">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-170">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2e6ac-171">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-171">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="2e6ac-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-172">Read-only.</span></span>|
|<span data-ttu-id="2e6ac-173">state</span><span class="sxs-lookup"><span data-stu-id="2e6ac-173">state</span></span>|<span data-ttu-id="2e6ac-174">connectedOrganizationState</span><span class="sxs-lookup"><span data-stu-id="2e6ac-174">connectedOrganizationState</span></span>|<span data-ttu-id="2e6ac-175">O estado de uma organização conectada define se as políticas de atribuição com tipo de escopo solicitante `AllConfiguredConnectedOrganizationSubjects` são aplicáveis ou não.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-175">The state of a connected organization defines whether assignment policies with requestor scope type `AllConfiguredConnectedOrganizationSubjects` are applicable or not.</span></span> <span data-ttu-id="2e6ac-176">Os valores possíveis são: `configured`, `proposed`.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-176">Possible values are: `configured`, `proposed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e6ac-177">Relações</span><span class="sxs-lookup"><span data-stu-id="2e6ac-177">Relationships</span></span>

|<span data-ttu-id="2e6ac-178">Relação</span><span class="sxs-lookup"><span data-stu-id="2e6ac-178">Relationship</span></span>|<span data-ttu-id="2e6ac-179">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e6ac-179">Type</span></span>|<span data-ttu-id="2e6ac-180">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e6ac-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e6ac-181">identitySources</span><span class="sxs-lookup"><span data-stu-id="2e6ac-181">identitySources</span></span>|<span data-ttu-id="2e6ac-182">coleção [identityry](identitySource.md)</span><span class="sxs-lookup"><span data-stu-id="2e6ac-182">[identitySource](identitySource.md) collection</span></span>| <span data-ttu-id="2e6ac-183">As fontes de identidade nesta organização conectada, uma de [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) ou [externalDomainFederation](externaldomainfederation.md).</span><span class="sxs-lookup"><span data-stu-id="2e6ac-183">The identity sources in this connected organization, one of [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) or [externalDomainFederation](externaldomainfederation.md).</span></span> <span data-ttu-id="2e6ac-184">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-184">Read-only.</span></span> <span data-ttu-id="2e6ac-185">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-185">Nullable.</span></span>|
|<span data-ttu-id="2e6ac-186">internalSponsors</span><span class="sxs-lookup"><span data-stu-id="2e6ac-186">internalSponsors</span></span>| <span data-ttu-id="2e6ac-187">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="2e6ac-187">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="2e6ac-188">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-188">Nullable.</span></span>|
|<span data-ttu-id="2e6ac-189">externalSponsors</span><span class="sxs-lookup"><span data-stu-id="2e6ac-189">externalSponsors</span></span>| <span data-ttu-id="2e6ac-190">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="2e6ac-190">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="2e6ac-191">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-191">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e6ac-192">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2e6ac-192">JSON representation</span></span>

<span data-ttu-id="2e6ac-193">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2e6ac-193">The following is a JSON representation of the resource.</span></span>

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
  ],
  "state": "String"
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


