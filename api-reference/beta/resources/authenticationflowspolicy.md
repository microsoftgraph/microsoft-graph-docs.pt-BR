---
title: Tipo de recurso authenticationFlowsPolicy
description: 'Representa a configuração da política da experiência de inscrição de autoatendimento no nível do locatário que permite aos usuários externos solicitar a inscrição para a aprovação. '
author: linkhp
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1113836041f4faa89a356811e38d2ef3ac70fef4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433156"
---
# <a name="authenticationflowspolicy-resource-type"></a><span data-ttu-id="3eb4a-103">Tipo de recurso authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="3eb4a-103">authenticationFlowsPolicy resource type</span></span>


<span data-ttu-id="3eb4a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3eb4a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3eb4a-105">Representa a [configuração da política da experiência de inscrição de autoatendimento](../resources/selfservicesignupauthenticationflowconfiguration.md) no nível do locatário que permite aos usuários externos solicitar a inscrição para a aprovação.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-105">Represents the [policy configuration of self-service sign-up experience](../resources/selfservicesignupauthenticationflowconfiguration.md) at a tenant level that lets external users request to sign up for approval.</span></span> <span data-ttu-id="3eb4a-106">Ela contém informações sobre a ID, o nome de exibição e a descrição e indica se a inscrição de autoatendimento está habilitada para a política.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-106">It contains information about the ID, display name, and description, and indicates whether self-service sign up is enabled for the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="3eb4a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3eb4a-107">Properties</span></span>
|<span data-ttu-id="3eb4a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3eb4a-108">Property</span></span>|<span data-ttu-id="3eb4a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3eb4a-109">Type</span></span>|<span data-ttu-id="3eb4a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3eb4a-110">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="3eb4a-111">id</span><span class="sxs-lookup"><span data-stu-id="3eb4a-111">id</span></span>|<span data-ttu-id="3eb4a-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3eb4a-112">String</span></span>| <span data-ttu-id="3eb4a-113">Propriedade herdada.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-113">Inherited property.</span></span> <span data-ttu-id="3eb4a-114">A ID da política de fluxos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-114">The ID of the authentication flows policy.</span></span> <span data-ttu-id="3eb4a-115">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-115">Optional.</span></span> <span data-ttu-id="3eb4a-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-116">Read-only.</span></span>
|<span data-ttu-id="3eb4a-117">displayName</span><span class="sxs-lookup"><span data-stu-id="3eb4a-117">displayName</span></span>|<span data-ttu-id="3eb4a-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3eb4a-118">String</span></span>| <span data-ttu-id="3eb4a-119">Propriedade herdada.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-119">Inherited property.</span></span> <span data-ttu-id="3eb4a-120">O nome de política legível.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-120">The human-readable name of the policy.</span></span> <span data-ttu-id="3eb4a-121">Essa propriedade não é uma chave.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-121">This property is not a key.</span></span> <span data-ttu-id="3eb4a-122">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-122">Optional.</span></span> <span data-ttu-id="3eb4a-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-123">Read-only.</span></span>|
|<span data-ttu-id="3eb4a-124">description</span><span class="sxs-lookup"><span data-stu-id="3eb4a-124">description</span></span>|<span data-ttu-id="3eb4a-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3eb4a-125">String</span></span>|<span data-ttu-id="3eb4a-126">Propriedade herdada.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-126">Inherited property.</span></span> <span data-ttu-id="3eb4a-127">Uma descrição da política.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-127">A description of the policy.</span></span> <span data-ttu-id="3eb4a-128">Essa propriedade não é uma chave.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-128">This property is not a key.</span></span> <span data-ttu-id="3eb4a-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-129">Optional.</span></span> <span data-ttu-id="3eb4a-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-130">Read-only.</span></span>|
|<span data-ttu-id="3eb4a-131">selfServiceSignUp</span><span class="sxs-lookup"><span data-stu-id="3eb4a-131">selfServiceSignUp</span></span>|[<span data-ttu-id="3eb4a-132">selfServiceSignUpAuthenticationFlowConfiguration</span><span class="sxs-lookup"><span data-stu-id="3eb4a-132">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md) |<span data-ttu-id="3eb4a-133">Contém configurações [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) que comunicam se a inscrição de autoatendimento está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-133">Contains [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) settings that convey whether self-service sign-up is enabled or disabled.</span></span> <span data-ttu-id="3eb4a-134">Essa propriedade não é uma chave.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-134">This property is not a key.</span></span> <span data-ttu-id="3eb4a-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-135">Optional.</span></span> <span data-ttu-id="3eb4a-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-136">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3eb4a-137">Relações</span><span class="sxs-lookup"><span data-stu-id="3eb4a-137">Relationships</span></span>
<span data-ttu-id="3eb4a-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3eb4a-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3eb4a-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3eb4a-139">JSON representation</span></span>
<span data-ttu-id="3eb4a-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3eb4a-140">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationFlowsPolicy",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "selfServiceSignUp": {
    "@odata.type": "#microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
  },
}
```


