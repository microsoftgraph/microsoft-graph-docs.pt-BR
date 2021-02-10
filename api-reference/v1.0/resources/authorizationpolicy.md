---
title: Tipo de recurso authorizationPolicy
description: Representa uma política que pode controlar as configurações de autorização do Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 12fe4ad670d2bb5056d05fde533d4b690068f7a5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154212"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="66040-103">Tipo de recurso authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="66040-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="66040-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66040-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="66040-105">Representa uma política que pode controlar as configurações de autorização do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="66040-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="66040-106">É um singleton que herda do tipo de política base e sempre existe para o locatário.</span><span class="sxs-lookup"><span data-stu-id="66040-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="66040-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="66040-107">Methods</span></span>

| <span data-ttu-id="66040-108">Método</span><span class="sxs-lookup"><span data-stu-id="66040-108">Method</span></span>       | <span data-ttu-id="66040-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="66040-109">Return Type</span></span> | <span data-ttu-id="66040-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="66040-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="66040-111">Obter authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="66040-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="66040-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="66040-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="66040-113">Leia o objeto authorizationPolicy.</span><span class="sxs-lookup"><span data-stu-id="66040-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="66040-114">Atualizar authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="66040-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="66040-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="66040-115">None</span></span> | <span data-ttu-id="66040-116">Atualize o objeto authorizationPolicy.</span><span class="sxs-lookup"><span data-stu-id="66040-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="66040-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66040-117">Properties</span></span>  
| <span data-ttu-id="66040-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66040-118">Property</span></span> | <span data-ttu-id="66040-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="66040-119">Type</span></span> | <span data-ttu-id="66040-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="66040-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="66040-121">id</span><span class="sxs-lookup"><span data-stu-id="66040-121">id</span></span>|<span data-ttu-id="66040-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66040-122">String</span></span>| <span data-ttu-id="66040-123">ID da política de autorização.</span><span class="sxs-lookup"><span data-stu-id="66040-123">ID of the authorization policy.</span></span> <span data-ttu-id="66040-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66040-124">Required.</span></span> <span data-ttu-id="66040-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66040-125">Read-only.</span></span>| 
|<span data-ttu-id="66040-126">displayName</span><span class="sxs-lookup"><span data-stu-id="66040-126">displayName</span></span>|<span data-ttu-id="66040-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66040-127">String</span></span>| <span data-ttu-id="66040-128">Nome para exibição desta política.</span><span class="sxs-lookup"><span data-stu-id="66040-128">Display name for this policy.</span></span> |  
|<span data-ttu-id="66040-129">description</span><span class="sxs-lookup"><span data-stu-id="66040-129">description</span></span>|<span data-ttu-id="66040-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66040-130">String</span></span>| <span data-ttu-id="66040-131">Descrição desta política.</span><span class="sxs-lookup"><span data-stu-id="66040-131">Description of this policy.</span></span>|  
|<span data-ttu-id="66040-132">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="66040-132">blockMsolPowerShell</span></span>|<span data-ttu-id="66040-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="66040-133">Boolean</span></span>| <span data-ttu-id="66040-134">Para desabilitar o uso do MSOL PowerShell, de definida essa propriedade como true.</span><span class="sxs-lookup"><span data-stu-id="66040-134">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="66040-135">A configuração como true também desabilitará o acesso baseado no usuário ao ponto de extremidade de serviço herdado usado pelo MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="66040-135">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="66040-136">Isso não afeta o Azure AD Connect ou o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="66040-136">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="66040-137">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="66040-137">defaultUserRolePermissions</span></span>|[<span data-ttu-id="66040-138">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="66040-138">defaultUserRolePermissions</span></span>](defaultuserrolepermissions.md)| <span data-ttu-id="66040-139">Especifica determinadas permissões personalizáveis para a função de usuário padrão.</span><span class="sxs-lookup"><span data-stu-id="66040-139">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="66040-140">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="66040-140">allowedToUseSSPR</span></span>|<span data-ttu-id="66040-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="66040-141">Boolean</span></span>| <span data-ttu-id="66040-142">Indica se o Self-Serve redefinição de senha pode ser usado pelos usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="66040-142">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="66040-143">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="66040-143">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="66040-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="66040-144">Boolean</span></span>| <span data-ttu-id="66040-145">Indica se os usuários podem se inscrever para assinaturas baseadas em email.</span><span class="sxs-lookup"><span data-stu-id="66040-145">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="66040-146">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="66040-146">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="66040-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="66040-147">Boolean</span></span>| <span data-ttu-id="66040-148">Indica se um usuário pode ingressar no locatário por meio de validação de email.</span><span class="sxs-lookup"><span data-stu-id="66040-148">Indicates whether a user can join the tenant by email validation.</span></span> | 
|<span data-ttu-id="66040-149">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="66040-149">allowInvitesFrom</span></span>|<span data-ttu-id="66040-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66040-150">String</span></span>|<span data-ttu-id="66040-151">Indica quem pode convidar usuários externos para a organização.</span><span class="sxs-lookup"><span data-stu-id="66040-151">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="66040-152">Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="66040-152">Possible values are:</span></span><ul><li><span data-ttu-id="66040-153">`none` - Impedir que todos, incluindo administradores, convidando usuários externos.</span><span class="sxs-lookup"><span data-stu-id="66040-153">`none` - Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="66040-154">Configuração padrão para o Governo dos Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="66040-154">Default setting for US Government.</span></span></li><li><span data-ttu-id="66040-155">`adminsAndGuestInviters` - Permitir que os membros das funções Administradores Globais, Administradores de Usuários e Convidados convidem usuários externos.</span><span class="sxs-lookup"><span data-stu-id="66040-155">`adminsAndGuestInviters` - Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span></li><li><span data-ttu-id="66040-156">`adminsGuestInvitersAndAllMembers` - Permitir que as funções de administrador acima e todos os outros membros da função de usuário convidem usuários externos.</span><span class="sxs-lookup"><span data-stu-id="66040-156">`adminsGuestInvitersAndAllMembers` - Allow the above admin roles and all other User role members to invite external users.</span></span></li><li><span data-ttu-id="66040-157">`everyone` - Permitir que todos na organização, incluindo usuários convidados, convidem usuários externos.</span><span class="sxs-lookup"><span data-stu-id="66040-157">`everyone` - Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="66040-158">Configuração padrão para todos os ambientes de nuvem, exceto o Governo dos Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="66040-158">Default setting for all cloud environments except US Government.</span></span></li></ul> |

## <a name="relationships"></a><span data-ttu-id="66040-159">Relações</span><span class="sxs-lookup"><span data-stu-id="66040-159">Relationships</span></span>

<span data-ttu-id="66040-160">Nenhum</span><span class="sxs-lookup"><span data-stu-id="66040-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="66040-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66040-161">JSON representation</span></span>

<span data-ttu-id="66040-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66040-162">The following is a JSON representation of the resource.</span></span>

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
