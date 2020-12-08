---
title: tipo de recurso authorizationPolicy
description: Representa uma política que pode controlar as configurações de autorização do Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5c71e4d01ba54c9043ff827b3749be63442d06ac
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581182"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="ea1d7-103">tipo de recurso authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="ea1d7-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="ea1d7-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ea1d7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea1d7-105">Representa uma política que pode controlar as configurações de autorização do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="ea1d7-106">É um singleton que herda do tipo de política base e sempre existe para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="ea1d7-107">Methods</span><span class="sxs-lookup"><span data-stu-id="ea1d7-107">Methods</span></span>

| <span data-ttu-id="ea1d7-108">Método</span><span class="sxs-lookup"><span data-stu-id="ea1d7-108">Method</span></span>       | <span data-ttu-id="ea1d7-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ea1d7-109">Return Type</span></span> | <span data-ttu-id="ea1d7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea1d7-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ea1d7-111">Obter authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="ea1d7-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="ea1d7-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="ea1d7-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="ea1d7-113">Leia o objeto authorizationPolicy.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="ea1d7-114">Atualizar authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="ea1d7-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="ea1d7-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea1d7-115">None</span></span> | <span data-ttu-id="ea1d7-116">Atualize o objeto authorizationPolicy.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ea1d7-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea1d7-117">Properties</span></span>  
| <span data-ttu-id="ea1d7-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea1d7-118">Property</span></span> | <span data-ttu-id="ea1d7-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea1d7-119">Type</span></span> | <span data-ttu-id="ea1d7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea1d7-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="ea1d7-121">id</span><span class="sxs-lookup"><span data-stu-id="ea1d7-121">id</span></span>|<span data-ttu-id="ea1d7-122">String</span><span class="sxs-lookup"><span data-stu-id="ea1d7-122">String</span></span>| <span data-ttu-id="ea1d7-123">ID da política de autorização.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-123">ID of the authorization policy.</span></span> <span data-ttu-id="ea1d7-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-124">Required.</span></span> <span data-ttu-id="ea1d7-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-125">Read-only.</span></span>| 
|<span data-ttu-id="ea1d7-126">displayName</span><span class="sxs-lookup"><span data-stu-id="ea1d7-126">displayName</span></span>|<span data-ttu-id="ea1d7-127">String</span><span class="sxs-lookup"><span data-stu-id="ea1d7-127">String</span></span>| <span data-ttu-id="ea1d7-128">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-128">Display name for this policy.</span></span> |  
|<span data-ttu-id="ea1d7-129">description</span><span class="sxs-lookup"><span data-stu-id="ea1d7-129">description</span></span>|<span data-ttu-id="ea1d7-130">String</span><span class="sxs-lookup"><span data-stu-id="ea1d7-130">String</span></span>| <span data-ttu-id="ea1d7-131">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-131">Description of this policy.</span></span>|  
|<span data-ttu-id="ea1d7-132">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="ea1d7-132">blockMsolPowerShell</span></span>|<span data-ttu-id="ea1d7-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea1d7-133">Boolean</span></span>| <span data-ttu-id="ea1d7-134">Para desabilitar o uso do MSOL PowerShell defina essa propriedade como true.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-134">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="ea1d7-135">A configuração como true também desabilitará o acesso baseado no usuário ao ponto de extremidade de serviço herdado usado pelo MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-135">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="ea1d7-136">Isso não afeta o Azure AD Connect ou o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-136">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="ea1d7-137">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="ea1d7-137">defaultUserRolePermissions</span></span>|[<span data-ttu-id="ea1d7-138">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="ea1d7-138">defaultUserRolePermissions</span></span>](defaultuserrolepermissions.md)| <span data-ttu-id="ea1d7-139">Especifica determinadas permissões personalizáveis para a função de usuário padrão.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-139">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="ea1d7-140">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="ea1d7-140">allowedToUseSSPR</span></span>|<span data-ttu-id="ea1d7-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea1d7-141">Boolean</span></span>| <span data-ttu-id="ea1d7-142">Indica se o Self-Serve recurso de redefinição de senha pode ser usado por usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-142">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="ea1d7-143">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="ea1d7-143">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="ea1d7-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea1d7-144">Boolean</span></span>| <span data-ttu-id="ea1d7-145">Indica se os usuários podem se inscrever para assinaturas baseadas em email.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-145">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="ea1d7-146">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="ea1d7-146">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="ea1d7-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea1d7-147">Boolean</span></span>| <span data-ttu-id="ea1d7-148">Indica se um usuário pode ingressar no locatário por validação de email.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-148">Indicates whether a user can join the tenant by email validation.</span></span> | 
|<span data-ttu-id="ea1d7-149">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="ea1d7-149">allowInvitesFrom</span></span>|<span data-ttu-id="ea1d7-150">String</span><span class="sxs-lookup"><span data-stu-id="ea1d7-150">String</span></span>|<span data-ttu-id="ea1d7-151">Indica quem pode convidar usuários externos para a organização.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-151">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="ea1d7-152">Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="ea1d7-152">Possible values are:</span></span><ul><li><span data-ttu-id="ea1d7-153">`none` – Impedir que todos, incluindo administradores, convidarem usuários externos.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-153">`none` - Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="ea1d7-154">Configuração padrão para o governo dos EUA.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-154">Default setting for US Government.</span></span></li><li><span data-ttu-id="ea1d7-155">`adminsAndGuestInviters` – Permitir que membros de administradores globais, administradores de usuários e funções do convidado de convidados convidarem usuários externos.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-155">`adminsAndGuestInviters` - Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span></li><li><span data-ttu-id="ea1d7-156">`adminsGuestInvitersAndAllMembers` – Permitir que as funções de administrador acima e todos os outros membros da função de usuário convidem usuários externos.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-156">`adminsGuestInvitersAndAllMembers` - Allow the above admin roles and all other User role members to invite external users.</span></span></li><li><span data-ttu-id="ea1d7-157">`everyone` – Permitir que todos na organização, incluindo usuários convidados, convidem usuários externos.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-157">`everyone` - Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="ea1d7-158">Configuração padrão para todos os ambientes de nuvem, exceto o governo dos EUA.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-158">Default setting for all cloud environments except US Government.</span></span></li></ul> |

## <a name="relationships"></a><span data-ttu-id="ea1d7-159">Relações</span><span class="sxs-lookup"><span data-stu-id="ea1d7-159">Relationships</span></span>

<span data-ttu-id="ea1d7-160">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea1d7-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea1d7-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea1d7-161">JSON representation</span></span>

<span data-ttu-id="ea1d7-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea1d7-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authorizationPolicy",
  "baseType": "",
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
