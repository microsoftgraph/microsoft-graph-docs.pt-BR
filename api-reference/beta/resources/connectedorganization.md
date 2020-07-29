---
title: tipo de recurso connectedOrganization
description: No Azure AD pretitulation Management, uma organização conectada é uma referência a um diretório ou domínio de outra organização cujos usuários podem solicitar acesso.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cb82ac88f1f81bf7d2f3238657818d0782ed6b60
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509973"
---
# <a name="connectedorganization-resource-type"></a><span data-ttu-id="ae243-103">tipo de recurso connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="ae243-103">connectedOrganization resource type</span></span>

<span data-ttu-id="ae243-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae243-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae243-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma organização conectada é uma referência a um diretório ou domínio de outra organização cujos usuários podem solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="ae243-105">In [Azure AD entitlement management](entitlementmanagement-root.md), a connected organization is a reference to a directory or domain of another organization whose users can request access.</span></span>

## <a name="methods"></a><span data-ttu-id="ae243-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ae243-106">Methods</span></span>

|<span data-ttu-id="ae243-107">Método</span><span class="sxs-lookup"><span data-stu-id="ae243-107">Method</span></span>|<span data-ttu-id="ae243-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ae243-108">Return type</span></span>|<span data-ttu-id="ae243-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae243-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ae243-110">Listar connectedOrganizations</span><span class="sxs-lookup"><span data-stu-id="ae243-110">List connectedOrganizations</span></span>](../api/connectedorganization-list.md) | <span data-ttu-id="ae243-111">coleção [connectedOrganization](connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="ae243-111">[connectedOrganization](connectedorganization.md) collection</span></span> | <span data-ttu-id="ae243-112">Recupere uma lista de objetos connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="ae243-112">Retrieve a list of connectedOrganization objects.</span></span> |
|[<span data-ttu-id="ae243-113">Criar connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="ae243-113">Create connectedOrganization</span></span>](../api/connectedorganization-post.md) | [<span data-ttu-id="ae243-114">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="ae243-114">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="ae243-115">Criar um novo objeto connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="ae243-115">Create a new connectedOrganization object.</span></span> |
|[<span data-ttu-id="ae243-116">Obter connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="ae243-116">Get connectedOrganization</span></span>](../api/connectedorganization-get.md) | [<span data-ttu-id="ae243-117">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="ae243-117">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="ae243-118">Ler propriedades e relações de um objeto connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="ae243-118">Read properties and relationships of a connectedOrganization object.</span></span> |
|[<span data-ttu-id="ae243-119">Atualizar connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="ae243-119">Update connectedOrganization</span></span>](../api/connectedorganization-update.md) | | <span data-ttu-id="ae243-120">Atualizar um connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="ae243-120">Update a connectedOrganization.</span></span> |
|[<span data-ttu-id="ae243-121">Excluir connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="ae243-121">Delete connectedOrganization</span></span>](../api/connectedorganization-delete.md) |<span data-ttu-id="ae243-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ae243-122">None</span></span> | <span data-ttu-id="ae243-123">Excluir um connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="ae243-123">Delete a connectedOrganization.</span></span> |

## <a name="properties"></a><span data-ttu-id="ae243-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae243-124">Properties</span></span>

|<span data-ttu-id="ae243-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae243-125">Property</span></span>|<span data-ttu-id="ae243-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae243-126">Type</span></span>|<span data-ttu-id="ae243-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae243-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae243-128">createdBy</span><span class="sxs-lookup"><span data-stu-id="ae243-128">createdBy</span></span>|<span data-ttu-id="ae243-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae243-129">String</span></span>|<span data-ttu-id="ae243-130">UPN do usuário que criou este recurso.</span><span class="sxs-lookup"><span data-stu-id="ae243-130">UPN of the user who created this resource.</span></span> <span data-ttu-id="ae243-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae243-131">Read-only.</span></span>|
|<span data-ttu-id="ae243-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae243-132">createdDateTime</span></span>|<span data-ttu-id="ae243-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae243-133">DateTimeOffset</span></span>|<span data-ttu-id="ae243-134">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ae243-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ae243-135">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ae243-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="ae243-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae243-136">Read-only.</span></span>|
|<span data-ttu-id="ae243-137">description</span><span class="sxs-lookup"><span data-stu-id="ae243-137">description</span></span>|<span data-ttu-id="ae243-138">String</span><span class="sxs-lookup"><span data-stu-id="ae243-138">String</span></span>|<span data-ttu-id="ae243-139">A descrição da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="ae243-139">The description of the connected organization.</span></span>|
|<span data-ttu-id="ae243-140">displayName</span><span class="sxs-lookup"><span data-stu-id="ae243-140">displayName</span></span>|<span data-ttu-id="ae243-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae243-141">String</span></span>|<span data-ttu-id="ae243-142">O nome de exibição da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="ae243-142">The display name of the connected organization.</span></span>|
|<span data-ttu-id="ae243-143">id</span><span class="sxs-lookup"><span data-stu-id="ae243-143">id</span></span>|<span data-ttu-id="ae243-144">String</span><span class="sxs-lookup"><span data-stu-id="ae243-144">String</span></span>| <span data-ttu-id="ae243-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae243-145">Read-only.</span></span>|
|<span data-ttu-id="ae243-146">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="ae243-146">modifiedBy</span></span>|<span data-ttu-id="ae243-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae243-147">String</span></span>|<span data-ttu-id="ae243-148">UPN do usuário que modificou este recurso pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ae243-148">UPN of the user who last modified this resource.</span></span> <span data-ttu-id="ae243-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae243-149">Read-only.</span></span>|
|<span data-ttu-id="ae243-150">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae243-150">modifiedDateTime</span></span>|<span data-ttu-id="ae243-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae243-151">DateTimeOffset</span></span>|<span data-ttu-id="ae243-152">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ae243-152">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ae243-153">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ae243-153">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="ae243-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae243-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae243-155">Relações</span><span class="sxs-lookup"><span data-stu-id="ae243-155">Relationships</span></span>

|<span data-ttu-id="ae243-156">Relação</span><span class="sxs-lookup"><span data-stu-id="ae243-156">Relationship</span></span>|<span data-ttu-id="ae243-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae243-157">Type</span></span>|<span data-ttu-id="ae243-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae243-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae243-159">identitySources</span><span class="sxs-lookup"><span data-stu-id="ae243-159">identitySources</span></span>|<span data-ttu-id="ae243-160">coleção [identityry](identitySource.md)</span><span class="sxs-lookup"><span data-stu-id="ae243-160">[identitySource](identitySource.md) collection</span></span>| <span data-ttu-id="ae243-161">As fontes de identidade nesta organização conectada, uma de [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) ou [externalDomainFederation](externaldomainfederation.md).</span><span class="sxs-lookup"><span data-stu-id="ae243-161">The identity sources in this connected organization, one of [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) or [externalDomainFederation](externaldomainfederation.md).</span></span> <span data-ttu-id="ae243-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae243-162">Read-only.</span></span> <span data-ttu-id="ae243-163">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ae243-163">Nullable.</span></span>|
|<span data-ttu-id="ae243-164">internalSponsors</span><span class="sxs-lookup"><span data-stu-id="ae243-164">internalSponsors</span></span>| <span data-ttu-id="ae243-165">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="ae243-165">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="ae243-166">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ae243-166">Nullable.</span></span>|
|<span data-ttu-id="ae243-167">externalSponsors</span><span class="sxs-lookup"><span data-stu-id="ae243-167">externalSponsors</span></span>| <span data-ttu-id="ae243-168">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="ae243-168">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="ae243-169">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ae243-169">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae243-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae243-170">JSON representation</span></span>

<span data-ttu-id="ae243-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ae243-171">The following is a JSON representation of the resource.</span></span>

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
