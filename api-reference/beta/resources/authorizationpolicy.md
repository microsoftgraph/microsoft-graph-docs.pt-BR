---
title: tipo de recurso authorizationPolicy
description: Representa uma política que pode controlar as configurações de autorização do Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c20f4dad0263e9d4c931e43da99870ed022f1e58
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492198"
---
# <a name="authorizationpolicy-resource-type"></a><span data-ttu-id="7edad-103">tipo de recurso authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="7edad-103">authorizationPolicy resource type</span></span>

<span data-ttu-id="7edad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7edad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7edad-105">Representa uma política que pode controlar as configurações de autorização do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7edad-105">Represents a policy that can control Azure Active Directory authorization settings.</span></span> <span data-ttu-id="7edad-106">É um singleton que herda do tipo de política base e sempre existe para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7edad-106">It's a singleton that inherits from base policy type, and always exists for the tenant.</span></span> 

## <a name="methods"></a><span data-ttu-id="7edad-107">Methods</span><span class="sxs-lookup"><span data-stu-id="7edad-107">Methods</span></span>

| <span data-ttu-id="7edad-108">Método</span><span class="sxs-lookup"><span data-stu-id="7edad-108">Method</span></span>       | <span data-ttu-id="7edad-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7edad-109">Return Type</span></span> | <span data-ttu-id="7edad-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7edad-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7edad-111">Obter authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="7edad-111">Get authorizationPolicy</span></span>](../api/authorizationpolicy-get.md) | [<span data-ttu-id="7edad-112">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="7edad-112">authorizationPolicy</span></span>](authorizationpolicy.md) | <span data-ttu-id="7edad-113">Leia o objeto authorizationPolicy.</span><span class="sxs-lookup"><span data-stu-id="7edad-113">Read the authorizationPolicy object.</span></span> |
| [<span data-ttu-id="7edad-114">Atualizar authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="7edad-114">Update authorizationPolicy</span></span>](../api/authorizationpolicy-update.md) | <span data-ttu-id="7edad-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7edad-115">None</span></span> | <span data-ttu-id="7edad-116">Atualize o objeto authorizationPolicy.</span><span class="sxs-lookup"><span data-stu-id="7edad-116">Update the authorizationPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7edad-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7edad-117">Properties</span></span>  
| <span data-ttu-id="7edad-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7edad-118">Property</span></span> | <span data-ttu-id="7edad-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="7edad-119">Type</span></span> | <span data-ttu-id="7edad-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7edad-120">Description</span></span> | 
|-|-|-|
|<span data-ttu-id="7edad-121">id</span><span class="sxs-lookup"><span data-stu-id="7edad-121">id</span></span>|<span data-ttu-id="7edad-122">String</span><span class="sxs-lookup"><span data-stu-id="7edad-122">String</span></span>| <span data-ttu-id="7edad-123">ID da política de autorização.</span><span class="sxs-lookup"><span data-stu-id="7edad-123">ID of the authorization policy.</span></span> <span data-ttu-id="7edad-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7edad-124">Required.</span></span> <span data-ttu-id="7edad-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7edad-125">Read-only.</span></span>| 
|<span data-ttu-id="7edad-126">displayName</span><span class="sxs-lookup"><span data-stu-id="7edad-126">displayName</span></span>|<span data-ttu-id="7edad-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7edad-127">String</span></span>| <span data-ttu-id="7edad-128">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="7edad-128">Display name for this policy.</span></span> |  
|<span data-ttu-id="7edad-129">description</span><span class="sxs-lookup"><span data-stu-id="7edad-129">description</span></span>|<span data-ttu-id="7edad-130">String</span><span class="sxs-lookup"><span data-stu-id="7edad-130">String</span></span>| <span data-ttu-id="7edad-131">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="7edad-131">Description of this policy.</span></span>|  
|<span data-ttu-id="7edad-132">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="7edad-132">guestUserRoleId</span></span>|<span data-ttu-id="7edad-133">Guid</span><span class="sxs-lookup"><span data-stu-id="7edad-133">Guid</span></span>| <span data-ttu-id="7edad-134">Representa o modelo de função para a função que deve ser concedida ao usuário convidado.</span><span class="sxs-lookup"><span data-stu-id="7edad-134">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="7edad-135">Consulte [list unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) para encontrar a lista de modelos de função disponíveis.</span><span class="sxs-lookup"><span data-stu-id="7edad-135">Refer to [List unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) to find the list of available role templates.</span></span> <span data-ttu-id="7edad-136">As funções a seguir são suportadas: usuário (a0b1b346-4d3e-4e8b-98f8-753987be4970), usuário convidado (10dae51f-b6af-4016-8d66-8c2a99b929b3) e usuário convidado restrito (2af84b1e-32c8-42b7-82bc-daa82404023b).</span><span class="sxs-lookup"><span data-stu-id="7edad-136">Currently following roles are supported: User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).</span></span> | 
|<span data-ttu-id="7edad-137">enabledPreviewFeatures</span><span class="sxs-lookup"><span data-stu-id="7edad-137">enabledPreviewFeatures</span></span>|<span data-ttu-id="7edad-138">Coleção (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="7edad-138">Collection(string)</span></span>| <span data-ttu-id="7edad-139">Lista de recursos habilitados para visualização privada no locatário.</span><span class="sxs-lookup"><span data-stu-id="7edad-139">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="7edad-140">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="7edad-140">blockMsolPowerShell</span></span>|<span data-ttu-id="7edad-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="7edad-141">Boolean</span></span>| <span data-ttu-id="7edad-142">Para desabilitar o uso do MSOL PowerShell defina essa propriedade como true.</span><span class="sxs-lookup"><span data-stu-id="7edad-142">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="7edad-143">A configuração como true também desabilitará o acesso baseado no usuário ao ponto de extremidade de serviço herdado usado pelo MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7edad-143">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="7edad-144">Isso não afeta o Azure AD Connect ou o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7edad-144">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 


## <a name="relationships"></a><span data-ttu-id="7edad-145">Relações</span><span class="sxs-lookup"><span data-stu-id="7edad-145">Relationships</span></span>
<span data-ttu-id="7edad-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7edad-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7edad-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7edad-147">JSON representation</span></span>

<span data-ttu-id="7edad-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7edad-148">The following is a JSON representation of the resource.</span></span>

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
  "enabledPreviewFeatures": "[String]",
  "guestUserRoleId": "Guid",
  "blockMsolPowerShell": true 
}
```
