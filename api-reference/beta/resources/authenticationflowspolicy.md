---
title: Tipo de recurso authenticationFlowsPolicy
description: 'Representa a configuração da política da experiência de inscrição de autoatendimento no nível do locatário que permite aos usuários externos solicitar a inscrição para a aprovação. '
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a676014ba6d31ffea08331342504629796f49ec8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034128"
---
# <a name="authenticationflowspolicy-resource-type"></a><span data-ttu-id="bd9bb-103">Tipo de recurso authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="bd9bb-103">authenticationFlowsPolicy resource type</span></span>


<span data-ttu-id="bd9bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd9bb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bd9bb-105">Representa a [configuração da política da experiência de inscrição de autoatendimento](../resources/selfservicesignupauthenticationflowconfiguration.md) no nível do locatário que permite aos usuários externos solicitar a inscrição para a aprovação.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-105">Represents the [policy configuration of self-service sign-up experience](../resources/selfservicesignupauthenticationflowconfiguration.md) at a tenant level that lets external users request to sign up for approval.</span></span> <span data-ttu-id="bd9bb-106">Ela contém informações sobre a ID, o nome de exibição e a descrição e indica se a inscrição de autoatendimento está habilitada para a política.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-106">It contains information about the ID, display name, and description, and indicates whether self-service sign up is enabled for the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="bd9bb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bd9bb-107">Properties</span></span>
|<span data-ttu-id="bd9bb-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd9bb-108">Property</span></span>|<span data-ttu-id="bd9bb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd9bb-109">Type</span></span>|<span data-ttu-id="bd9bb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd9bb-110">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="bd9bb-111">id</span><span class="sxs-lookup"><span data-stu-id="bd9bb-111">id</span></span>|<span data-ttu-id="bd9bb-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd9bb-112">String</span></span>| <span data-ttu-id="bd9bb-113">Propriedade herdada.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-113">Inherited property.</span></span> <span data-ttu-id="bd9bb-114">A ID da política de fluxos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-114">The ID of the authentication flows policy.</span></span> <span data-ttu-id="bd9bb-115">Opcional.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-115">Optional.</span></span> <span data-ttu-id="bd9bb-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-116">Read-only.</span></span>
|<span data-ttu-id="bd9bb-117">displayName</span><span class="sxs-lookup"><span data-stu-id="bd9bb-117">displayName</span></span>|<span data-ttu-id="bd9bb-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd9bb-118">String</span></span>| <span data-ttu-id="bd9bb-119">Propriedade herdada.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-119">Inherited property.</span></span> <span data-ttu-id="bd9bb-120">O nome de política legível.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-120">The human-readable name of the policy.</span></span> <span data-ttu-id="bd9bb-121">Essa propriedade não é uma chave.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-121">This property is not a key.</span></span> <span data-ttu-id="bd9bb-122">Opcional.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-122">Optional.</span></span> <span data-ttu-id="bd9bb-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-123">Read-only.</span></span>|
|<span data-ttu-id="bd9bb-124">description</span><span class="sxs-lookup"><span data-stu-id="bd9bb-124">description</span></span>|<span data-ttu-id="bd9bb-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd9bb-125">String</span></span>|<span data-ttu-id="bd9bb-126">Propriedade herdada.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-126">Inherited property.</span></span> <span data-ttu-id="bd9bb-127">Uma descrição da política.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-127">A description of the policy.</span></span> <span data-ttu-id="bd9bb-128">Essa propriedade não é uma chave.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-128">This property is not a key.</span></span> <span data-ttu-id="bd9bb-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-129">Optional.</span></span> <span data-ttu-id="bd9bb-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-130">Read-only.</span></span>|
|<span data-ttu-id="bd9bb-131">selfServiceSignUp</span><span class="sxs-lookup"><span data-stu-id="bd9bb-131">selfServiceSignUp</span></span>|[<span data-ttu-id="bd9bb-132">selfServiceSignUpAuthenticationFlowConfiguration</span><span class="sxs-lookup"><span data-stu-id="bd9bb-132">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md) |<span data-ttu-id="bd9bb-133">Contém configurações [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) que comunicam se a inscrição de autoatendimento está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-133">Contains [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) settings that convey whether self-service sign-up is enabled or disabled.</span></span> <span data-ttu-id="bd9bb-134">Essa propriedade não é uma chave.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-134">This property is not a key.</span></span> <span data-ttu-id="bd9bb-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-135">Optional.</span></span> <span data-ttu-id="bd9bb-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-136">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bd9bb-137">Relações</span><span class="sxs-lookup"><span data-stu-id="bd9bb-137">Relationships</span></span>
<span data-ttu-id="bd9bb-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bd9bb-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd9bb-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bd9bb-139">JSON representation</span></span>
<span data-ttu-id="bd9bb-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bd9bb-140">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationFlowsPolicy",
  "baseType": "",
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


