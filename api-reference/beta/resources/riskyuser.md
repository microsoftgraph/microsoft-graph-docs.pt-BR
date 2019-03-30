---
title: tipo de recurso riskyUsers
description: Representa usuários do Azure AD que estão em risco. O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina. Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3265ea40903ca2c5c10272f5df280bd3715af366
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/30/2019
ms.locfileid: "31003717"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="7f5a9-105">tipo de recurso riskyUsers</span><span class="sxs-lookup"><span data-stu-id="7f5a9-105">riskyUsers resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f5a9-106">Representa usuários do Azure AD que estão em risco.</span><span class="sxs-lookup"><span data-stu-id="7f5a9-106">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="7f5a9-107">O Azure AD avalia continuamente o risco do usuário com base em vários sinais e aprendizado de máquina.</span><span class="sxs-lookup"><span data-stu-id="7f5a9-107">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="7f5a9-108">Essa API fornece acesso programático a todos os usuários de risco em seu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7f5a9-108">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="7f5a9-109">Para obter mais informações sobre eventos de risco, consulte [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="7f5a9-109">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

><span data-ttu-id="7f5a9-110">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="7f5a9-110">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="7f5a9-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="7f5a9-111">Methods</span></span>

| <span data-ttu-id="7f5a9-112">Método</span><span class="sxs-lookup"><span data-stu-id="7f5a9-112">Method</span></span>   | <span data-ttu-id="7f5a9-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7f5a9-113">Return Type</span></span>|<span data-ttu-id="7f5a9-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f5a9-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7f5a9-115">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="7f5a9-115">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="7f5a9-116">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="7f5a9-116">riskyUsers</span></span>](riskyUser.md) |<span data-ttu-id="7f5a9-117">Listar usuários arriscados e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="7f5a9-117">List risky users and their properties.</span></span>|
|[<span data-ttu-id="7f5a9-118">Obter riskyUsers</span><span class="sxs-lookup"><span data-stu-id="7f5a9-118">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="7f5a9-119">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="7f5a9-119">riskyUsers</span></span>](riskyUser.md)|<span data-ttu-id="7f5a9-120">Obtenha um usuário arriscado específico e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="7f5a9-120">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="7f5a9-121">Confirmar riskyUsers comprometido</span><span class="sxs-lookup"><span data-stu-id="7f5a9-121">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="7f5a9-122">Confirmar um usuário arriscado como comprometido.</span><span class="sxs-lookup"><span data-stu-id="7f5a9-122">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="7f5a9-123">Ignorar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="7f5a9-123">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="7f5a9-124">DesCartar o risco de um usuário arriscado.</span><span class="sxs-lookup"><span data-stu-id="7f5a9-124">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="7f5a9-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f5a9-125">Properties</span></span>

| <span data-ttu-id="7f5a9-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f5a9-126">Property</span></span>   | <span data-ttu-id="7f5a9-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f5a9-127">Type</span></span>|<span data-ttu-id="7f5a9-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f5a9-128">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="7f5a9-129">ID exclusiva do usuário em risco</span><span class="sxs-lookup"><span data-stu-id="7f5a9-129">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="7f5a9-130">Indica se o usuário é excluído.</span><span class="sxs-lookup"><span data-stu-id="7f5a9-130">Indicates whether the user is deleted.</span></span> <span data-ttu-id="7f5a9-131">Os valores possíveis são `true`:,`false`</span><span class="sxs-lookup"><span data-stu-id="7f5a9-131">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="7f5a9-132">Indica se o usuário é um usuário convidado.</span><span class="sxs-lookup"><span data-stu-id="7f5a9-132">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="7f5a9-133">Os valores possíveis são: `true` e `false`.</span><span class="sxs-lookup"><span data-stu-id="7f5a9-133">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="7f5a9-134">True se a identidade do usuário está fora do locatário em consideração.</span><span class="sxs-lookup"><span data-stu-id="7f5a9-134">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="7f5a9-135">Este usuário pode ser um usuário B2B ou B2C com identidade no Azure AD, no MSA ou no provedor de identidade de terceiros.</span><span class="sxs-lookup"><span data-stu-id="7f5a9-135">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="7f5a9-136">False se a identidade do usuário está dentro do locatário em consideração</span><span class="sxs-lookup"><span data-stu-id="7f5a9-136">False if user’s identity lies inside the tenant in consideration</span></span>|
|`isProcessing`|`bool`|<span data-ttu-id="7f5a9-137">Indica wehther que o estado arriscado de um usuário está sendo processado pelo backend</span><span class="sxs-lookup"><span data-stu-id="7f5a9-137">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|`risk`|[<span data-ttu-id="7f5a9-138">risco</span><span class="sxs-lookup"><span data-stu-id="7f5a9-138">risk</span></span>](risk.md)|<span data-ttu-id="7f5a9-139">Estado de usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="7f5a9-139">Risky user state</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="7f5a9-140">A data e a hora em que o usuário arriscado foi atualizado pela última vez</span><span class="sxs-lookup"><span data-stu-id="7f5a9-140">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="7f5a9-141">Nome de exibição do usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="7f5a9-141">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="7f5a9-142">Nome UPN de usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="7f5a9-142">Risky user principal name</span></span>|


## <a name="json-representation"></a><span data-ttu-id="7f5a9-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f5a9-143">JSON representation</span></span>

<span data-ttu-id="7f5a9-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f5a9-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskyusers"
}-->

```json
{
 "id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isGuest": "boolean",
"isProcessing": "boolean",
"isDeleted": "boolean",
"risk": {"@odata.type": "microsoft.graph.risk"},
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
