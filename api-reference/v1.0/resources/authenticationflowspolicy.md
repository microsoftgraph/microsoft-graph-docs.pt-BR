---
title: Tipo de recurso authenticationFlowsPolicy
description: 'Representa a configuração da política da experiência de inscrição de autoatendimento no nível do locatário que permite aos usuários externos solicitar a inscrição para a aprovação. '
author: linkhp
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ea0ca54c4be4e80043ac9560d2b8dd3744584aa9
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882764"
---
# <a name="authenticationflowspolicy-resource-type"></a><span data-ttu-id="99d02-103">Tipo de recurso authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="99d02-103">authenticationFlowsPolicy resource type</span></span>

<span data-ttu-id="99d02-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99d02-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="99d02-105">Representa a [configuração da política da experiência de inscrição de autoatendimento](../resources/selfservicesignupauthenticationflowconfiguration.md) no nível do locatário que permite aos usuários externos solicitar a inscrição para a aprovação.</span><span class="sxs-lookup"><span data-stu-id="99d02-105">Represents the [policy configuration of self-service sign-up experience](../resources/selfservicesignupauthenticationflowconfiguration.md) at a tenant level that lets external users request to sign up for approval.</span></span> <span data-ttu-id="99d02-106">Ela contém informações sobre a ID, o nome de exibição e a descrição e indica se a inscrição de autoatendimento está habilitada para a política.</span><span class="sxs-lookup"><span data-stu-id="99d02-106">It contains information, such as the identifier, display name, and description, and indicates whether self-service sign-up is enabled for the policy.</span></span>

## <a name="methods"></a><span data-ttu-id="99d02-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="99d02-107">Methods</span></span>

| <span data-ttu-id="99d02-108">Método</span><span class="sxs-lookup"><span data-stu-id="99d02-108">Method</span></span>       | <span data-ttu-id="99d02-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="99d02-109">Return Type</span></span>  |<span data-ttu-id="99d02-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="99d02-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="99d02-111">Obter política de fluxos de autenticação</span><span class="sxs-lookup"><span data-stu-id="99d02-111">Get authentication flows policy</span></span>](../api/authenticationflowspolicy-get.md)|<span data-ttu-id="99d02-112">authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="99d02-112">authenticationFlowsPolicy</span></span>|<span data-ttu-id="99d02-113">Obter a configuração da política de fluxos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="99d02-113">Get the authentication flows policy configuration.</span></span>|
|[<span data-ttu-id="99d02-114">Atualizar a política de fluxos de autenticação</span><span class="sxs-lookup"><span data-stu-id="99d02-114">Update authentication flows policy</span></span>](../api/authenticationflowspolicy-update.md)|<span data-ttu-id="99d02-115">authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="99d02-115">authenticationFlowsPolicy</span></span>|<span data-ttu-id="99d02-116">Atualizar a configuração de política de fluxos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="99d02-116">Update the authentication flows policy configuration.</span></span>|

## <a name="properties"></a><span data-ttu-id="99d02-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99d02-117">Properties</span></span>

|<span data-ttu-id="99d02-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99d02-118">Property</span></span>|<span data-ttu-id="99d02-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="99d02-119">Type</span></span>|<span data-ttu-id="99d02-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="99d02-120">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="99d02-121">id</span><span class="sxs-lookup"><span data-stu-id="99d02-121">id</span></span>|<span data-ttu-id="99d02-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99d02-122">String</span></span>| <span data-ttu-id="99d02-123">Propriedade herdada.</span><span class="sxs-lookup"><span data-stu-id="99d02-123">Inherited property.</span></span> <span data-ttu-id="99d02-124">A ID da política de fluxos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="99d02-124">The identifier of the authentication flows policy.</span></span> <span data-ttu-id="99d02-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="99d02-125">Optional.</span></span> <span data-ttu-id="99d02-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="99d02-126">Read-only.</span></span>
|<span data-ttu-id="99d02-127">displayName</span><span class="sxs-lookup"><span data-stu-id="99d02-127">displayName</span></span>|<span data-ttu-id="99d02-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99d02-128">String</span></span>| <span data-ttu-id="99d02-129">Propriedade herdada.</span><span class="sxs-lookup"><span data-stu-id="99d02-129">Inherited property.</span></span> <span data-ttu-id="99d02-130">O nome de política legível.</span><span class="sxs-lookup"><span data-stu-id="99d02-130">The human-readable name of the policy.</span></span> <span data-ttu-id="99d02-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="99d02-131">Optional.</span></span> <span data-ttu-id="99d02-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="99d02-132">Read-only.</span></span>|
|<span data-ttu-id="99d02-133">description</span><span class="sxs-lookup"><span data-stu-id="99d02-133">description</span></span>|<span data-ttu-id="99d02-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99d02-134">String</span></span>|<span data-ttu-id="99d02-135">Propriedade herdada.</span><span class="sxs-lookup"><span data-stu-id="99d02-135">Inherited property.</span></span> <span data-ttu-id="99d02-136">Uma descrição da política.</span><span class="sxs-lookup"><span data-stu-id="99d02-136">A description of the policy.</span></span> <span data-ttu-id="99d02-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="99d02-137">Optional.</span></span> <span data-ttu-id="99d02-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="99d02-138">Read-only.</span></span>|
|<span data-ttu-id="99d02-139">selfServiceSignUp</span><span class="sxs-lookup"><span data-stu-id="99d02-139">selfServiceSignUp</span></span>|[<span data-ttu-id="99d02-140">selfServiceSignUpAuthenticationFlowConfiguration</span><span class="sxs-lookup"><span data-stu-id="99d02-140">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md) |<span data-ttu-id="99d02-141">Contém configurações [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) que comunicam se a inscrição de autoatendimento está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="99d02-141">Contains [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) settings that convey whether self-service sign-up is enabled or disabled.</span></span> <span data-ttu-id="99d02-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="99d02-142">Optional.</span></span> <span data-ttu-id="99d02-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="99d02-143">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="99d02-144">Relações</span><span class="sxs-lookup"><span data-stu-id="99d02-144">Relationships</span></span>

<span data-ttu-id="99d02-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99d02-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="99d02-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99d02-146">JSON representation</span></span>

<span data-ttu-id="99d02-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99d02-147">The following is a JSON representation of the resource.</span></span>
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
