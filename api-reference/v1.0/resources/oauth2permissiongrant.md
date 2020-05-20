---
title: tipo de recurso oAuth2PermissionGrant
description: Representa as permissões delegadas (escopos de OAuth 2,0) que foram concedidas a um aplicativo, com frequência como resultado de um usuário ou processo de consentimento de administrador.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: edf4ff7ed44e9b084ca2206b24fed0e18b5c581c
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290164"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="d5b5e-103">tipo de recurso oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="d5b5e-103">oAuth2PermissionGrant resource type</span></span>

<span data-ttu-id="d5b5e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5b5e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d5b5e-105">Representa as permissões delegadas que foram concedidas à entidade de serviço de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-105">Represents the delegated permissions that have been granted to an application's service principal.</span></span>

<span data-ttu-id="d5b5e-106">Conceder permissões delegadas podem ser criadas como resultado de um usuário que esteja consentindo a solicitação de um aplicativo para acessar uma API ou criado diretamente.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-106">Delegated permissions grants can be created as a result of a user consenting the an application's request to access an API, or created directly.</span></span>

<span data-ttu-id="d5b5e-107">As permissões delegadas às vezes são chamadas de "escopos de OAuth 2,0" ou "escopos".</span><span class="sxs-lookup"><span data-stu-id="d5b5e-107">Delegated permissions are sometimes referred to as "OAuth 2.0 scopes" or "scopes".</span></span>

## <a name="methods"></a><span data-ttu-id="d5b5e-108">Methods</span><span class="sxs-lookup"><span data-stu-id="d5b5e-108">Methods</span></span>

| <span data-ttu-id="d5b5e-109">Método</span><span class="sxs-lookup"><span data-stu-id="d5b5e-109">Method</span></span> | <span data-ttu-id="d5b5e-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d5b5e-110">Return Type</span></span> | <span data-ttu-id="d5b5e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5b5e-111">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="d5b5e-112">Listar oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="d5b5e-112">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="d5b5e-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span><span class="sxs-lookup"><span data-stu-id="d5b5e-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="d5b5e-114">Recupere uma lista de subsídios de permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-114">Retrieve a list of delegated permission grants.</span></span> |
| [<span data-ttu-id="d5b5e-115">Obter oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="d5b5e-115">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="d5b5e-116">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="d5b5e-116">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)  | <span data-ttu-id="d5b5e-117">Leia uma única concessão de permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-117">Read a single delegated permission grant.</span></span>|
| [<span data-ttu-id="d5b5e-118">Criar oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="d5b5e-118">Create oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-post.md) | [<span data-ttu-id="d5b5e-119">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="d5b5e-119">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) | <span data-ttu-id="d5b5e-120">Criar uma concessão de permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-120">Create a delegated permission grant.</span></span> |
| [<span data-ttu-id="d5b5e-121">Atualizar oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="d5b5e-121">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | <span data-ttu-id="d5b5e-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5b5e-122">None</span></span> | <span data-ttu-id="d5b5e-123">Atualize o objeto oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-123">Update oAuth2PermissionGrant object.</span></span> |
| [<span data-ttu-id="d5b5e-124">Excluir oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="d5b5e-124">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="d5b5e-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5b5e-125">None</span></span>  | <span data-ttu-id="d5b5e-126">Excluir uma concessão de permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-126">Delete a delegated permission grant.</span></span> |

## <a name="properties"></a><span data-ttu-id="d5b5e-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5b5e-127">Properties</span></span>

| <span data-ttu-id="d5b5e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5b5e-128">Property</span></span> | <span data-ttu-id="d5b5e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5b5e-129">Type</span></span> | <span data-ttu-id="d5b5e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5b5e-130">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="d5b5e-131">id</span><span class="sxs-lookup"><span data-stu-id="d5b5e-131">id</span></span> | <span data-ttu-id="d5b5e-132">String</span><span class="sxs-lookup"><span data-stu-id="d5b5e-132">String</span></span> | <span data-ttu-id="d5b5e-133">Identificador exclusivo para o **oAuth2PermissionGrant**.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-133">Unique identifier for the **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="d5b5e-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-134">Read-only.</span></span>|
| <span data-ttu-id="d5b5e-135">clientId</span><span class="sxs-lookup"><span data-stu-id="d5b5e-135">clientId</span></span> | <span data-ttu-id="d5b5e-136">String</span><span class="sxs-lookup"><span data-stu-id="d5b5e-136">String</span></span> | <span data-ttu-id="d5b5e-137">A **ID** da entidade de [serviço](serviceprincipal.md) do cliente para o aplicativo que é autorizado a atuar em nome de um usuário conectado ao acessar uma API.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-137">The **id** of the client [service principal](serviceprincipal.md) for the application which is authorized to act on behalf of a signed-in user when accessing an API.</span></span> <span data-ttu-id="d5b5e-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-138">Required.</span></span> <span data-ttu-id="d5b5e-139">Suporta `$filter` ( `eq` somente).</span><span class="sxs-lookup"><span data-stu-id="d5b5e-139">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="d5b5e-140">consentType</span><span class="sxs-lookup"><span data-stu-id="d5b5e-140">consentType</span></span> | <span data-ttu-id="d5b5e-141">String</span><span class="sxs-lookup"><span data-stu-id="d5b5e-141">String</span></span> | <span data-ttu-id="d5b5e-142">Indica se a autorização é concedida para que o aplicativo cliente represente todos os usuários ou apenas um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-142">Indicates if authorization is granted for the client application to impersonate all users or only a specific user.</span></span> <span data-ttu-id="d5b5e-143">A *entidade de segurança* indica autorização para representar todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-143">*AllPrincipals* indicates authorization to impersonate all users.</span></span> <span data-ttu-id="d5b5e-144">*Principal* indica autorização para representar um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-144">*Principal* indicates authorization to impersonate a specific user.</span></span> <span data-ttu-id="d5b5e-145">O consentimento em nome de todos os usuários pode ser concedido por um administrador.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-145">Consent on behalf of all users can be granted by an administrator.</span></span> <span data-ttu-id="d5b5e-146">Os usuários que não são administradores podem ser autorizados a consentir em nome de alguns casos, para algumas permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-146">Non-admin users may be authorized to consent on behalf of themselves in some cases, for some delegated permissions.</span></span> <span data-ttu-id="d5b5e-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-147">Required.</span></span> <span data-ttu-id="d5b5e-148">Suporta `$filter` ( `eq` somente).</span><span class="sxs-lookup"><span data-stu-id="d5b5e-148">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="d5b5e-149">principalId</span><span class="sxs-lookup"><span data-stu-id="d5b5e-149">principalId</span></span> | <span data-ttu-id="d5b5e-150">String</span><span class="sxs-lookup"><span data-stu-id="d5b5e-150">String</span></span> | <span data-ttu-id="d5b5e-151">A **ID** do [usuário](user.md) em nome do qual o cliente está autorizado a acessar o recurso, quando **resenttype** é o *principal*.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-151">The **id** of the [user](user.md) on behalf of whom the client is authorized to access the resource, when **consentType** is *Principal*.</span></span> <span data-ttu-id="d5b5e-152">Se **consenttype** for *servicePrincipalName* , esse valor será NULL.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-152">If **consentType** is *AllPrincipals* this value is null.</span></span> <span data-ttu-id="d5b5e-153">Obrigatório quando **resenttype** é *principal*.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-153">Required when **consentType** is *Principal*.</span></span> |
| <span data-ttu-id="d5b5e-154">resourceId</span><span class="sxs-lookup"><span data-stu-id="d5b5e-154">resourceId</span></span> | <span data-ttu-id="d5b5e-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5b5e-155">String</span></span> | <span data-ttu-id="d5b5e-156">A **ID** da entidade de [serviço](serviceprincipal.md) de recurso para a qual o acesso é autorizado.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-156">The **id** of the resource [service principal](serviceprincipal.md) to which access is authorized.</span></span> <span data-ttu-id="d5b5e-157">Isso identifica a API que o cliente está autorizado a tentar chamar em nome de um usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-157">This identifies the API which the client is authorized to attempt to call on behalf of a signed-in user.</span></span> |
| <span data-ttu-id="d5b5e-158">escopo</span><span class="sxs-lookup"><span data-stu-id="d5b5e-158">scope</span></span> | <span data-ttu-id="d5b5e-159">String</span><span class="sxs-lookup"><span data-stu-id="d5b5e-159">String</span></span> | <span data-ttu-id="d5b5e-160">Uma lista separada por espaços dos valores de declaração para permissões delegadas que devem ser incluídas em tokens de acesso para o aplicativo de recurso (a API).</span><span class="sxs-lookup"><span data-stu-id="d5b5e-160">A space-separated list of the claim values for delegated permissions which should be included in access tokens for the resource application (the API).</span></span> <span data-ttu-id="d5b5e-161">Por exemplo, `openid User.Read GroupMember.Read.All`.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-161">For example, `openid User.Read GroupMember.Read.All`.</span></span> <span data-ttu-id="d5b5e-162">Cada valor de declaração deve corresponder ao campo de **valor** de uma das permissões delegadas definidas pela API, listadas na propriedade **publishedPermissionScopes** da entidade de [serviço](serviceprincipal.md)de recurso.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-162">Each claim value should match the **value** field of one of the delegated permissions defined by the API, listed in the **publishedPermissionScopes** property of the resource [service principal](serviceprincipal.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="d5b5e-163">Relações</span><span class="sxs-lookup"><span data-stu-id="d5b5e-163">Relationships</span></span>

<span data-ttu-id="d5b5e-164">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5b5e-164">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5b5e-165">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5b5e-165">JSON representation</span></span>

<span data-ttu-id="d5b5e-166">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5b5e-166">The following is a JSON representation of the resource.</span></span>

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
