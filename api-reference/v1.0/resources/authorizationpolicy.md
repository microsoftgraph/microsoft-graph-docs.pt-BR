---
title: Tipo de recurso authorizationPolicy
description: Representa uma política que pode controlar as configurações de autorização de Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b08284d99d88ffbfa38c950062986ba72da900d5
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231924"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="2d608-103">Tipo de recurso authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="2d608-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="2d608-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d608-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d608-105">Representa uma política que pode controlar as Azure Active Directory de autorização.</span><span class="sxs-lookup"><span data-stu-id="2d608-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="2d608-106">É um singleton que herda do tipo de política base e sempre existe para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2d608-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="2d608-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="2d608-107">Methods</span></span>

| <span data-ttu-id="2d608-108">Método</span><span class="sxs-lookup"><span data-stu-id="2d608-108">Method</span></span>       | <span data-ttu-id="2d608-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2d608-109">Return Type</span></span> | <span data-ttu-id="2d608-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d608-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2d608-111">Obter authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="2d608-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="2d608-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="2d608-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="2d608-113">Leia o objeto authorizationPolicy.</span><span class="sxs-lookup"><span data-stu-id="2d608-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="2d608-114">Atualizar authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="2d608-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="2d608-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2d608-115">None</span></span> | <span data-ttu-id="2d608-116">Atualize o objeto authorizationPolicy.</span><span class="sxs-lookup"><span data-stu-id="2d608-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2d608-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d608-117">Properties</span></span>  
| <span data-ttu-id="2d608-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d608-118">Property</span></span> | <span data-ttu-id="2d608-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d608-119">Type</span></span> | <span data-ttu-id="2d608-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d608-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="2d608-121">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="2d608-121">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="2d608-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="2d608-122">Boolean</span></span>| <span data-ttu-id="2d608-123">Indica se os usuários podem se inscrever para assinaturas baseadas em email.</span><span class="sxs-lookup"><span data-stu-id="2d608-123">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="2d608-124">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="2d608-124">allowedToUseSSPR</span></span>|<span data-ttu-id="2d608-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="2d608-125">Boolean</span></span>| <span data-ttu-id="2d608-126">Indica se o recurso Self-Serve redefinição de senha pode ser usado pelos usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="2d608-126">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="2d608-127">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="2d608-127">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="2d608-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="2d608-128">Boolean</span></span>| <span data-ttu-id="2d608-129">Indica se um usuário pode ingressar no locatário por validação de email.</span><span class="sxs-lookup"><span data-stu-id="2d608-129">Indicates whether a user can join the tenant by email validation.</span></span> | 
|<span data-ttu-id="2d608-130">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="2d608-130">allowInvitesFrom</span></span>|<span data-ttu-id="2d608-131">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="2d608-131">allowInvitesFrom</span></span>|<span data-ttu-id="2d608-132">Indica quem pode convidar usuários externos para a organização.</span><span class="sxs-lookup"><span data-stu-id="2d608-132">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="2d608-133">Os valores possíveis são: `none`, `adminsAndGuestInviters`, `adminsGuestInvitersAndAllMembers`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="2d608-133">Possible values are: `none`, `adminsAndGuestInviters`, `adminsGuestInvitersAndAllMembers`, `everyone`.</span></span>  <span data-ttu-id="2d608-134">`everyone` é a configuração padrão para todos os ambientes de nuvem, exceto o Governo dos EUA.</span><span class="sxs-lookup"><span data-stu-id="2d608-134">`everyone` is the default setting for all cloud environments except US Government.</span></span> <span data-ttu-id="2d608-135">Confira mais na [tabela abaixo](#allowinvitesfrom-values).</span><span class="sxs-lookup"><span data-stu-id="2d608-135">See more in the [table below](#allowinvitesfrom-values).</span></span> |
|<span data-ttu-id="2d608-136">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="2d608-136">blockMsolPowerShell</span></span>|<span data-ttu-id="2d608-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="2d608-137">Boolean</span></span>| <span data-ttu-id="2d608-138">Para desabilitar o uso do MSOL PowerShell, de definir essa propriedade como `true` .</span><span class="sxs-lookup"><span data-stu-id="2d608-138">To disable the use of MSOL PowerShell set this property to `true`.</span></span> <span data-ttu-id="2d608-139">Isso também desabilitará o acesso baseado no usuário ao ponto de extremidade de serviço herdado usado pelo MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2d608-139">This will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="2d608-140">Isso não afeta o Azure AD Conexão ou o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2d608-140">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="2d608-141">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="2d608-141">defaultUserRolePermissions</span></span>|[<span data-ttu-id="2d608-142">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="2d608-142">defaultUserRolePermissions</span></span>](defaultuserrolepermissions.md)| <span data-ttu-id="2d608-143">Especifica determinadas permissões personalizáveis para a função de usuário padrão.</span><span class="sxs-lookup"><span data-stu-id="2d608-143">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="2d608-144">descrição</span><span class="sxs-lookup"><span data-stu-id="2d608-144">description</span></span>|<span data-ttu-id="2d608-145">String</span><span class="sxs-lookup"><span data-stu-id="2d608-145">String</span></span>| <span data-ttu-id="2d608-146">Descrição dessa política.</span><span class="sxs-lookup"><span data-stu-id="2d608-146">Description of this policy.</span></span>|
|<span data-ttu-id="2d608-147">displayName</span><span class="sxs-lookup"><span data-stu-id="2d608-147">displayName</span></span>|<span data-ttu-id="2d608-148">String</span><span class="sxs-lookup"><span data-stu-id="2d608-148">String</span></span>| <span data-ttu-id="2d608-149">Nome de exibição para esta política.</span><span class="sxs-lookup"><span data-stu-id="2d608-149">Display name for this policy.</span></span> |    
|<span data-ttu-id="2d608-150">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="2d608-150">guestUserRoleId</span></span>|<span data-ttu-id="2d608-151">Guid</span><span class="sxs-lookup"><span data-stu-id="2d608-151">Guid</span></span>| <span data-ttu-id="2d608-152">Representa modelo de funçãoId para a função que deve ser concedida ao usuário convidado.</span><span class="sxs-lookup"><span data-stu-id="2d608-152">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="2d608-153">Atualmente, há suporte para as seguintes funções: User ( `a0b1b346-4d3e-4e8b-98f8-753987be4970` ), Guest User ( ) e `10dae51f-b6af-4016-8d66-8c2a99b929b3` Restricted Guest User ( `2af84b1e-32c8-42b7-82bc-daa82404023b` ).</span><span class="sxs-lookup"><span data-stu-id="2d608-153">Currently following roles are supported:  User (`a0b1b346-4d3e-4e8b-98f8-753987be4970`), Guest User (`10dae51f-b6af-4016-8d66-8c2a99b929b3`), and Restricted Guest User (`2af84b1e-32c8-42b7-82bc-daa82404023b`).</span></span> |
|<span data-ttu-id="2d608-154">id</span><span class="sxs-lookup"><span data-stu-id="2d608-154">id</span></span>|<span data-ttu-id="2d608-155">String</span><span class="sxs-lookup"><span data-stu-id="2d608-155">String</span></span>| <span data-ttu-id="2d608-156">ID da política de autorização.</span><span class="sxs-lookup"><span data-stu-id="2d608-156">ID of the authorization policy.</span></span> <span data-ttu-id="2d608-157">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d608-157">Required.</span></span> <span data-ttu-id="2d608-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2d608-158">Read-only.</span></span>| 

### <a name="allowinvitesfrom-values"></a><span data-ttu-id="2d608-159">valores allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="2d608-159">allowInvitesFrom values</span></span>

|<span data-ttu-id="2d608-160">Member</span><span class="sxs-lookup"><span data-stu-id="2d608-160">Member</span></span>|<span data-ttu-id="2d608-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d608-161">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2d608-162">nenhuma</span><span class="sxs-lookup"><span data-stu-id="2d608-162">none</span></span>|<span data-ttu-id="2d608-163">Impedir que todos, incluindo administradores, convidam usuários externos.</span><span class="sxs-lookup"><span data-stu-id="2d608-163">Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="2d608-164">Configuração padrão para o Governo dos EUA.</span><span class="sxs-lookup"><span data-stu-id="2d608-164">Default setting for US Government.</span></span>|
|<span data-ttu-id="2d608-165">adminsAndGuestInviters</span><span class="sxs-lookup"><span data-stu-id="2d608-165">adminsAndGuestInviters</span></span>|<span data-ttu-id="2d608-166">Permitir que os membros das funções Administradores Globais, Administradores de Usuários e Convidados convidem usuários externos.</span><span class="sxs-lookup"><span data-stu-id="2d608-166">Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span>|
|<span data-ttu-id="2d608-167">adminsGuestInvitersAndAllMembers</span><span class="sxs-lookup"><span data-stu-id="2d608-167">adminsGuestInvitersAndAllMembers</span></span>|<span data-ttu-id="2d608-168">Permitir que as funções de administrador acima e todos os outros membros da função de usuário convidem usuários externos.</span><span class="sxs-lookup"><span data-stu-id="2d608-168">Allow the above admin roles and all other User role members to invite external users.</span></span>|
|<span data-ttu-id="2d608-169">everyone</span><span class="sxs-lookup"><span data-stu-id="2d608-169">everyone</span></span>|<span data-ttu-id="2d608-170">Permitir que todos na organização, incluindo usuários convidados, convidem usuários externos.</span><span class="sxs-lookup"><span data-stu-id="2d608-170">Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="2d608-171">A configuração padrão para todos os ambientes de nuvem, exceto o Governo dos EUA.</span><span class="sxs-lookup"><span data-stu-id="2d608-171">The default setting for all cloud environments except US Government.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d608-172">Relações</span><span class="sxs-lookup"><span data-stu-id="2d608-172">Relationships</span></span>

<span data-ttu-id="2d608-173">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2d608-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d608-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d608-174">JSON representation</span></span>

<span data-ttu-id="2d608-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d608-175">The following is a JSON representation of the resource.</span></span>

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
  "allowInvitesFrom": "String",
  "guestUserRoleId": "Guid"
}
```
