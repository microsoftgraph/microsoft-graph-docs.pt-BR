---
title: Tipo de recurso authorizationPolicy
description: Representa uma política que pode controlar as configurações de autorização do Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 85af4636f52e49717e864f2ccb9d710fea313eb2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962515"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="a71ab-103">Tipo de recurso authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="a71ab-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="a71ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a71ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a71ab-105">Representa uma política que pode controlar as configurações de autorização do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a71ab-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="a71ab-106">É um singleton que herda do tipo de política base e sempre existe para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a71ab-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="a71ab-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a71ab-107">Methods</span></span>

| <span data-ttu-id="a71ab-108">Método</span><span class="sxs-lookup"><span data-stu-id="a71ab-108">Method</span></span>       | <span data-ttu-id="a71ab-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a71ab-109">Return Type</span></span> | <span data-ttu-id="a71ab-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a71ab-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a71ab-111">Obter authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="a71ab-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="a71ab-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="a71ab-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="a71ab-113">Leia o objeto authorizationPolicy.</span><span class="sxs-lookup"><span data-stu-id="a71ab-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="a71ab-114">Atualizar authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="a71ab-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="a71ab-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a71ab-115">None</span></span> | <span data-ttu-id="a71ab-116">Atualize o objeto authorizationPolicy.</span><span class="sxs-lookup"><span data-stu-id="a71ab-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a71ab-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a71ab-117">Properties</span></span>  
| <span data-ttu-id="a71ab-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a71ab-118">Property</span></span> | <span data-ttu-id="a71ab-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a71ab-119">Type</span></span> | <span data-ttu-id="a71ab-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a71ab-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="a71ab-121">id</span><span class="sxs-lookup"><span data-stu-id="a71ab-121">id</span></span>|<span data-ttu-id="a71ab-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a71ab-122">String</span></span>| <span data-ttu-id="a71ab-123">ID da política de autorização.</span><span class="sxs-lookup"><span data-stu-id="a71ab-123">ID of the authorization policy.</span></span> <span data-ttu-id="a71ab-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a71ab-124">Required.</span></span> <span data-ttu-id="a71ab-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a71ab-125">Read-only.</span></span>| 
|<span data-ttu-id="a71ab-126">displayName</span><span class="sxs-lookup"><span data-stu-id="a71ab-126">displayName</span></span>|<span data-ttu-id="a71ab-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a71ab-127">String</span></span>| <span data-ttu-id="a71ab-128">Nome de exibição para esta política.</span><span class="sxs-lookup"><span data-stu-id="a71ab-128">Display name for this policy.</span></span> |  
|<span data-ttu-id="a71ab-129">description</span><span class="sxs-lookup"><span data-stu-id="a71ab-129">description</span></span>|<span data-ttu-id="a71ab-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a71ab-130">String</span></span>| <span data-ttu-id="a71ab-131">Descrição dessa política.</span><span class="sxs-lookup"><span data-stu-id="a71ab-131">Description of this policy.</span></span>|  
|<span data-ttu-id="a71ab-132">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="a71ab-132">blockMsolPowerShell</span></span>|<span data-ttu-id="a71ab-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="a71ab-133">Boolean</span></span>| <span data-ttu-id="a71ab-134">Para desabilitar o uso do MSOL PowerShell, de definir essa propriedade como true.</span><span class="sxs-lookup"><span data-stu-id="a71ab-134">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="a71ab-135">A configuração como true também desabilitará o acesso baseado no usuário ao ponto de extremidade de serviço herdado usado pelo MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a71ab-135">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="a71ab-136">Isso não afeta o Azure AD Connect ou o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a71ab-136">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="a71ab-137">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="a71ab-137">defaultUserRolePermissions</span></span>|[<span data-ttu-id="a71ab-138">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="a71ab-138">defaultUserRolePermissions</span></span>](defaultuserrolepermissions.md)| <span data-ttu-id="a71ab-139">Especifica determinadas permissões personalizáveis para a função de usuário padrão.</span><span class="sxs-lookup"><span data-stu-id="a71ab-139">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="a71ab-140">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="a71ab-140">allowedToUseSSPR</span></span>|<span data-ttu-id="a71ab-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="a71ab-141">Boolean</span></span>| <span data-ttu-id="a71ab-142">Indica se o recurso Self-Serve redefinição de senha pode ser usado pelos usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="a71ab-142">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="a71ab-143">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="a71ab-143">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="a71ab-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="a71ab-144">Boolean</span></span>| <span data-ttu-id="a71ab-145">Indica se os usuários podem se inscrever para assinaturas baseadas em email.</span><span class="sxs-lookup"><span data-stu-id="a71ab-145">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="a71ab-146">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="a71ab-146">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="a71ab-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="a71ab-147">Boolean</span></span>| <span data-ttu-id="a71ab-148">Indica se um usuário pode ingressar no locatário por validação de email.</span><span class="sxs-lookup"><span data-stu-id="a71ab-148">Indicates whether a user can join the tenant by email validation.</span></span> | 
|<span data-ttu-id="a71ab-149">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="a71ab-149">allowInvitesFrom</span></span>|<span data-ttu-id="a71ab-150">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="a71ab-150">allowInvitesFrom</span></span>|<span data-ttu-id="a71ab-151">Indica quem pode convidar usuários externos para a organização.</span><span class="sxs-lookup"><span data-stu-id="a71ab-151">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="a71ab-152">Os valores possíveis são: `none`, `adminsAndGuestInviters`, `adminsGuestInvitersAndAllMembers`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="a71ab-152">Possible values are: `none`, `adminsAndGuestInviters`, `adminsGuestInvitersAndAllMembers`, `everyone`.</span></span>  <span data-ttu-id="a71ab-153">`everyone` é a configuração padrão para todos os ambientes de nuvem, exceto o Governo dos EUA.</span><span class="sxs-lookup"><span data-stu-id="a71ab-153">`everyone` is the default setting for all cloud environments except US Government.</span></span> <span data-ttu-id="a71ab-154">Veja mais na [tabela abaixo](#allowinvitesfrom-values).</span><span class="sxs-lookup"><span data-stu-id="a71ab-154">See more in the [table below](#allowinvitesfrom-values).</span></span> |

### <a name="allowinvitesfrom-values"></a><span data-ttu-id="a71ab-155">valores allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="a71ab-155">allowInvitesFrom values</span></span>

|<span data-ttu-id="a71ab-156">Member</span><span class="sxs-lookup"><span data-stu-id="a71ab-156">Member</span></span>|<span data-ttu-id="a71ab-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="a71ab-157">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a71ab-158">nenhum</span><span class="sxs-lookup"><span data-stu-id="a71ab-158">none</span></span>|<span data-ttu-id="a71ab-159">Impedir que todos, incluindo administradores, convidam usuários externos.</span><span class="sxs-lookup"><span data-stu-id="a71ab-159">Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="a71ab-160">Configuração padrão para o Governo dos EUA.</span><span class="sxs-lookup"><span data-stu-id="a71ab-160">Default setting for US Government.</span></span>|
|<span data-ttu-id="a71ab-161">adminsAndGuestInviters</span><span class="sxs-lookup"><span data-stu-id="a71ab-161">adminsAndGuestInviters</span></span>|<span data-ttu-id="a71ab-162">Permitir que os membros das funções Administradores Globais, Administradores de Usuários e Convidados convidem usuários externos.</span><span class="sxs-lookup"><span data-stu-id="a71ab-162">Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span>|
|<span data-ttu-id="a71ab-163">adminsGuestInvitersAndAllMembers</span><span class="sxs-lookup"><span data-stu-id="a71ab-163">adminsGuestInvitersAndAllMembers</span></span>|<span data-ttu-id="a71ab-164">Permitir que as funções de administrador acima e todos os outros membros da função de usuário convidem usuários externos.</span><span class="sxs-lookup"><span data-stu-id="a71ab-164">Allow the above admin roles and all other User role members to invite external users.</span></span>|
|<span data-ttu-id="a71ab-165">everyone</span><span class="sxs-lookup"><span data-stu-id="a71ab-165">everyone</span></span>|<span data-ttu-id="a71ab-166">Permitir que todos na organização, incluindo usuários convidados, convidem usuários externos.</span><span class="sxs-lookup"><span data-stu-id="a71ab-166">Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="a71ab-167">A configuração padrão para todos os ambientes de nuvem, exceto o Governo dos EUA.</span><span class="sxs-lookup"><span data-stu-id="a71ab-167">The default setting for all cloud environments except US Government.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a71ab-168">Relações</span><span class="sxs-lookup"><span data-stu-id="a71ab-168">Relationships</span></span>

<span data-ttu-id="a71ab-169">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a71ab-169">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a71ab-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a71ab-170">JSON representation</span></span>

<span data-ttu-id="a71ab-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a71ab-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authorizationPolicy",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "blockMsolPowerShell": true,
  "defaultUserRolePermissions": {"@odata.type": "microsoft.graph.defaultUserRolePermissions"},
  "allowedToUseSSPR": true,
  "allowedToSignUpEmailBasedSubscriptions": true,
  "allowEmailVerifiedUsersToJoinOrganization": true,
  "allowInvitesFrom": "String"
}
```
