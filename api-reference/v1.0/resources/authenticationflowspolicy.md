---
title: Tipo de recurso authenticationFlowsPolicy
description: 'Representa a configuração da política da experiência de inscrição de autoatendimento no nível do locatário que permite aos usuários externos solicitar a inscrição para a aprovação. '
author: linkhp
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 369ad06f9d653054c6b165b0ebc2daa3e8d402c6
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231253"
---
# <a name="authenticationflowspolicy-resource-type"></a><span data-ttu-id="70120-103">Tipo de recurso authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="70120-103">authenticationFlowsPolicy resource type</span></span>

<span data-ttu-id="70120-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70120-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70120-105">Representa a [configuração da política da experiência de inscrição de autoatendimento](../resources/selfservicesignupauthenticationflowconfiguration.md) no nível do locatário que permite aos usuários externos solicitar a inscrição para a aprovação.</span><span class="sxs-lookup"><span data-stu-id="70120-105">Represents the [policy configuration of self-service sign-up experience](../resources/selfservicesignupauthenticationflowconfiguration.md) at a tenant level that lets external users request to sign up for approval.</span></span> <span data-ttu-id="70120-106">Ela contém informações sobre a ID, o nome de exibição e a descrição e indica se a inscrição de autoatendimento está habilitada para a política.</span><span class="sxs-lookup"><span data-stu-id="70120-106">It contains information, such as the identifier, display name, and description, and indicates whether self-service sign-up is enabled for the policy.</span></span>

## <a name="methods"></a><span data-ttu-id="70120-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="70120-107">Methods</span></span>

| <span data-ttu-id="70120-108">Método</span><span class="sxs-lookup"><span data-stu-id="70120-108">Method</span></span>       | <span data-ttu-id="70120-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="70120-109">Return Type</span></span>  |<span data-ttu-id="70120-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="70120-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="70120-111">Obter política de fluxos de autenticação</span><span class="sxs-lookup"><span data-stu-id="70120-111">Get authentication flows policy</span></span>](../api/authenticationflowspolicy-get.md)|<span data-ttu-id="70120-112">authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="70120-112">authenticationFlowsPolicy</span></span>|<span data-ttu-id="70120-113">Obter a configuração da política de fluxos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="70120-113">Get the authentication flows policy configuration.</span></span>|
|[<span data-ttu-id="70120-114">Atualizar a política de fluxos de autenticação</span><span class="sxs-lookup"><span data-stu-id="70120-114">Update authentication flows policy</span></span>](../api/authenticationflowspolicy-update.md)|<span data-ttu-id="70120-115">authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="70120-115">authenticationFlowsPolicy</span></span>|<span data-ttu-id="70120-116">Atualizar a configuração de política de fluxos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="70120-116">Update the authentication flows policy configuration.</span></span>|

## <a name="properties"></a><span data-ttu-id="70120-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70120-117">Properties</span></span>

|<span data-ttu-id="70120-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70120-118">Property</span></span>|<span data-ttu-id="70120-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="70120-119">Type</span></span>|<span data-ttu-id="70120-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="70120-120">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="70120-121">id</span><span class="sxs-lookup"><span data-stu-id="70120-121">id</span></span>|<span data-ttu-id="70120-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="70120-122">String</span></span>| <span data-ttu-id="70120-123">Propriedade herdada.</span><span class="sxs-lookup"><span data-stu-id="70120-123">Inherited property.</span></span> <span data-ttu-id="70120-124">A ID da política de fluxos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="70120-124">The identifier of the authentication flows policy.</span></span> <span data-ttu-id="70120-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="70120-125">Optional.</span></span> <span data-ttu-id="70120-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70120-126">Read-only.</span></span>
|<span data-ttu-id="70120-127">displayName</span><span class="sxs-lookup"><span data-stu-id="70120-127">displayName</span></span>|<span data-ttu-id="70120-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="70120-128">String</span></span>| <span data-ttu-id="70120-129">Propriedade herdada.</span><span class="sxs-lookup"><span data-stu-id="70120-129">Inherited property.</span></span> <span data-ttu-id="70120-130">O nome de política legível.</span><span class="sxs-lookup"><span data-stu-id="70120-130">The human-readable name of the policy.</span></span> <span data-ttu-id="70120-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="70120-131">Optional.</span></span> <span data-ttu-id="70120-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70120-132">Read-only.</span></span>|
|<span data-ttu-id="70120-133">description</span><span class="sxs-lookup"><span data-stu-id="70120-133">description</span></span>|<span data-ttu-id="70120-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="70120-134">String</span></span>|<span data-ttu-id="70120-135">Propriedade herdada.</span><span class="sxs-lookup"><span data-stu-id="70120-135">Inherited property.</span></span> <span data-ttu-id="70120-136">Uma descrição da política.</span><span class="sxs-lookup"><span data-stu-id="70120-136">A description of the policy.</span></span> <span data-ttu-id="70120-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="70120-137">Optional.</span></span> <span data-ttu-id="70120-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70120-138">Read-only.</span></span>|
|<span data-ttu-id="70120-139">selfServiceSignUp</span><span class="sxs-lookup"><span data-stu-id="70120-139">selfServiceSignUp</span></span>|[<span data-ttu-id="70120-140">selfServiceSignUpAuthenticationFlowConfiguration</span><span class="sxs-lookup"><span data-stu-id="70120-140">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md) |<span data-ttu-id="70120-141">Contém configurações [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) que comunicam se a inscrição de autoatendimento está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="70120-141">Contains [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) settings that convey whether self-service sign-up is enabled or disabled.</span></span> <span data-ttu-id="70120-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="70120-142">Optional.</span></span> <span data-ttu-id="70120-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70120-143">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="70120-144">Relações</span><span class="sxs-lookup"><span data-stu-id="70120-144">Relationships</span></span>

<span data-ttu-id="70120-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="70120-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="70120-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70120-146">JSON representation</span></span>

<span data-ttu-id="70120-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="70120-147">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationFlowsPolicy",
  "openType": false
}
-->

``` json
{
   "id":"String (identifier)",
   "displayName":"String",
   "description":"String",
   "selfServiceSignUp":{
      "@odata.type":"#microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
   }
}
```
