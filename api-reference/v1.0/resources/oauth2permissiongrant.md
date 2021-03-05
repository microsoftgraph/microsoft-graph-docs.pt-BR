---
title: Tipo de recurso oAuth2PermissionGrant
description: Representa as permissões delegadas (escopos OAuth 2.0) que foram concedidas a um aplicativo, geralmente como resultado do processo de consentimento do usuário ou administrador.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: d0c9e78d22a882998c0e17ba521cc76a611697af
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50432841"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="6e73f-103">Tipo de recurso oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="6e73f-103">oAuth2PermissionGrant resource type</span></span>

<span data-ttu-id="6e73f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e73f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6e73f-105">Representa as permissões delegadas que foram concedidas à entidade de serviço de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6e73f-105">Represents the delegated permissions that have been granted to an application's service principal.</span></span>

<span data-ttu-id="6e73f-106">As concessões de permissões delegadas podem ser criadas como resultado de um usuário consentir a solicitação de um aplicativo para acessar uma API ou criado diretamente.</span><span class="sxs-lookup"><span data-stu-id="6e73f-106">Delegated permissions grants can be created as a result of a user consenting the an application's request to access an API, or created directly.</span></span>

<span data-ttu-id="6e73f-107">As permissões delegadas às vezes são conhecidas como "escopos OAuth 2.0" ou "escopos".</span><span class="sxs-lookup"><span data-stu-id="6e73f-107">Delegated permissions are sometimes referred to as "OAuth 2.0 scopes" or "scopes".</span></span>

## <a name="methods"></a><span data-ttu-id="6e73f-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="6e73f-108">Methods</span></span>

| <span data-ttu-id="6e73f-109">Método</span><span class="sxs-lookup"><span data-stu-id="6e73f-109">Method</span></span> | <span data-ttu-id="6e73f-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6e73f-110">Return Type</span></span> | <span data-ttu-id="6e73f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e73f-111">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="6e73f-112">Listar oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="6e73f-112">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="6e73f-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span><span class="sxs-lookup"><span data-stu-id="6e73f-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="6e73f-114">Recupere uma lista de concessões de permissão delegadas.</span><span class="sxs-lookup"><span data-stu-id="6e73f-114">Retrieve a list of delegated permission grants.</span></span> |
| [<span data-ttu-id="6e73f-115">Obter oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="6e73f-115">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="6e73f-116">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="6e73f-116">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)  | <span data-ttu-id="6e73f-117">Leia uma única concessão de permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="6e73f-117">Read a single delegated permission grant.</span></span>|
| [<span data-ttu-id="6e73f-118">Criar oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="6e73f-118">Create oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-post.md) | [<span data-ttu-id="6e73f-119">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="6e73f-119">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) | <span data-ttu-id="6e73f-120">Crie uma concessão de permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="6e73f-120">Create a delegated permission grant.</span></span> |
| [<span data-ttu-id="6e73f-121">Atualizar oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="6e73f-121">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | <span data-ttu-id="6e73f-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e73f-122">None</span></span> | <span data-ttu-id="6e73f-123">Atualizar o objeto oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="6e73f-123">Update oAuth2PermissionGrant object.</span></span> |
| [<span data-ttu-id="6e73f-124">Excluir oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="6e73f-124">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="6e73f-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e73f-125">None</span></span>  | <span data-ttu-id="6e73f-126">Exclua uma concessão de permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="6e73f-126">Delete a delegated permission grant.</span></span> |
|[<span data-ttu-id="6e73f-127">Obter delta</span><span class="sxs-lookup"><span data-stu-id="6e73f-127">Get delta</span></span>](../api/oauth2permissiongrant-delta.md)|[<span data-ttu-id="6e73f-128">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="6e73f-128">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)|<span data-ttu-id="6e73f-129">Obter objetos **oauth2permissiongrant** recém-criados, atualizados ou excluídos sem executar uma leitura completa de toda a coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="6e73f-129">Get newly created, updated, or deleted **oauth2permissiongrant** objects without performing a full read of the entire resource collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="6e73f-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e73f-130">Properties</span></span>

| <span data-ttu-id="6e73f-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e73f-131">Property</span></span> | <span data-ttu-id="6e73f-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e73f-132">Type</span></span> | <span data-ttu-id="6e73f-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e73f-133">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="6e73f-134">id</span><span class="sxs-lookup"><span data-stu-id="6e73f-134">id</span></span> | <span data-ttu-id="6e73f-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e73f-135">String</span></span> | <span data-ttu-id="6e73f-136">Identificador exclusivo do **oAuth2PermissionGrant**.</span><span class="sxs-lookup"><span data-stu-id="6e73f-136">Unique identifier for the **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="6e73f-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6e73f-137">Read-only.</span></span>|
| <span data-ttu-id="6e73f-138">clientId</span><span class="sxs-lookup"><span data-stu-id="6e73f-138">clientId</span></span> | <span data-ttu-id="6e73f-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e73f-139">String</span></span> | <span data-ttu-id="6e73f-140">A **id** da [](serviceprincipal.md) entidade de serviço do cliente para o aplicativo que está autorizado a agir em nome de um usuário interno ao acessar uma API.</span><span class="sxs-lookup"><span data-stu-id="6e73f-140">The **id** of the client [service principal](serviceprincipal.md) for the application which is authorized to act on behalf of a signed-in user when accessing an API.</span></span> <span data-ttu-id="6e73f-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e73f-141">Required.</span></span> <span data-ttu-id="6e73f-142">Suporte para `$filter` (`eq` somente).</span><span class="sxs-lookup"><span data-stu-id="6e73f-142">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="6e73f-143">consentType</span><span class="sxs-lookup"><span data-stu-id="6e73f-143">consentType</span></span> | <span data-ttu-id="6e73f-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e73f-144">String</span></span> | <span data-ttu-id="6e73f-145">Indica se a autorização é concedida para que o aplicativo cliente represente todos os usuários ou apenas um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="6e73f-145">Indicates if authorization is granted for the client application to impersonate all users or only a specific user.</span></span> <span data-ttu-id="6e73f-146">*AllPrincipals* indica autorização para representar todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="6e73f-146">*AllPrincipals* indicates authorization to impersonate all users.</span></span> <span data-ttu-id="6e73f-147">*A* entidade indica autorização para representar um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="6e73f-147">*Principal* indicates authorization to impersonate a specific user.</span></span> <span data-ttu-id="6e73f-148">O consentimento em nome de todos os usuários pode ser concedido por um administrador.</span><span class="sxs-lookup"><span data-stu-id="6e73f-148">Consent on behalf of all users can be granted by an administrator.</span></span> <span data-ttu-id="6e73f-149">Os usuários que não são administradores podem ser autorizados a consentir em nome de si mesmos em alguns casos, para algumas permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="6e73f-149">Non-admin users may be authorized to consent on behalf of themselves in some cases, for some delegated permissions.</span></span> <span data-ttu-id="6e73f-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e73f-150">Required.</span></span> <span data-ttu-id="6e73f-151">Suporte para `$filter` (`eq` somente).</span><span class="sxs-lookup"><span data-stu-id="6e73f-151">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="6e73f-152">principalId</span><span class="sxs-lookup"><span data-stu-id="6e73f-152">principalId</span></span> | <span data-ttu-id="6e73f-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e73f-153">String</span></span> | <span data-ttu-id="6e73f-154">A **id** do [usuário em](user.md) nome do qual o cliente está autorizado a acessar o recurso, quando **consentType** for *Principal*.</span><span class="sxs-lookup"><span data-stu-id="6e73f-154">The **id** of the [user](user.md) on behalf of whom the client is authorized to access the resource, when **consentType** is *Principal*.</span></span> <span data-ttu-id="6e73f-155">Se **consentType** for *AllPrincipals,* esse valor será nulo.</span><span class="sxs-lookup"><span data-stu-id="6e73f-155">If **consentType** is *AllPrincipals* this value is null.</span></span> <span data-ttu-id="6e73f-156">Obrigatório quando **consentType** for *Principal*.</span><span class="sxs-lookup"><span data-stu-id="6e73f-156">Required when **consentType** is *Principal*.</span></span> |
| <span data-ttu-id="6e73f-157">resourceId</span><span class="sxs-lookup"><span data-stu-id="6e73f-157">resourceId</span></span> | <span data-ttu-id="6e73f-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e73f-158">String</span></span> | <span data-ttu-id="6e73f-159">A **id da** entidade de [serviço de recursos](serviceprincipal.md) à qual o acesso está autorizado.</span><span class="sxs-lookup"><span data-stu-id="6e73f-159">The **id** of the resource [service principal](serviceprincipal.md) to which access is authorized.</span></span> <span data-ttu-id="6e73f-160">Isso identifica a API que o cliente está autorizado a tentar chamar em nome de um usuário in-locar.</span><span class="sxs-lookup"><span data-stu-id="6e73f-160">This identifies the API which the client is authorized to attempt to call on behalf of a signed-in user.</span></span> |
| <span data-ttu-id="6e73f-161">escopo</span><span class="sxs-lookup"><span data-stu-id="6e73f-161">scope</span></span> | <span data-ttu-id="6e73f-162">String</span><span class="sxs-lookup"><span data-stu-id="6e73f-162">String</span></span> | <span data-ttu-id="6e73f-163">Uma lista separada por espaço dos valores de declaração para permissões delegadas que devem ser incluídos em tokens de acesso para o aplicativo de recurso (a API).</span><span class="sxs-lookup"><span data-stu-id="6e73f-163">A space-separated list of the claim values for delegated permissions which should be included in access tokens for the resource application (the API).</span></span> <span data-ttu-id="6e73f-164">Por exemplo, `openid User.Read GroupMember.Read.All`.</span><span class="sxs-lookup"><span data-stu-id="6e73f-164">For example, `openid User.Read GroupMember.Read.All`.</span></span> <span data-ttu-id="6e73f-165">Cada valor de  declaração deve corresponder ao campo de valor de uma das permissões delegadas definidas pela API, listadas na propriedade **publishedPermissionScopes** da entidade de [serviço de recursos](serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="6e73f-165">Each claim value should match the **value** field of one of the delegated permissions defined by the API, listed in the **publishedPermissionScopes** property of the resource [service principal](serviceprincipal.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="6e73f-166">Relações</span><span class="sxs-lookup"><span data-stu-id="6e73f-166">Relationships</span></span>

<span data-ttu-id="6e73f-167">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e73f-167">None.</span></span>

<span data-ttu-id="6e73f-168">Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/oauth2permissiongrant-delta.md).</span><span class="sxs-lookup"><span data-stu-id="6e73f-168">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/oauth2permissiongrant-delta.md) function.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e73f-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e73f-169">JSON representation</span></span>

<span data-ttu-id="6e73f-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e73f-170">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
}-->

```json
{
  "clientId": "string",
  "consentType": "string",
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

