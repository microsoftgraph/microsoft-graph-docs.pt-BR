---
title: tipo de recurso authenticationFlowsPolicy
description: 'Representa a configuração de política da experiência de inscrição de autoatendimento em um nível de locatário que permite aos usuários externos solicitar a inscrição para aprovação. '
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 263b92c081545fc3ce337d25b4813d85fe034940
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556382"
---
# <a name="authenticationflowspolicy-resource-type"></a><span data-ttu-id="6db24-103">tipo de recurso authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="6db24-103">authenticationFlowsPolicy resource type</span></span>


<span data-ttu-id="6db24-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6db24-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6db24-105">Representa a [configuração de política da experiência de inscrição de autoatendimento](../resources/selfservicesignupauthenticationflowconfiguration.md) em um nível de locatário que permite aos usuários externos solicitar a inscrição para aprovação.</span><span class="sxs-lookup"><span data-stu-id="6db24-105">Represents the [policy configuration of self-service sign-up experience](../resources/selfservicesignupauthenticationflowconfiguration.md) at a tenant level that lets external users request to sign up for approval.</span></span> <span data-ttu-id="6db24-106">Ele contém informações sobre a ID, o nome para exibição e a descrição e indica se a inscrição de autoatendimento está habilitada para a política.</span><span class="sxs-lookup"><span data-stu-id="6db24-106">It contains information about the ID, display name, and description, and indicates whether self-service sign up is enabled for the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="6db24-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6db24-107">Properties</span></span>
|<span data-ttu-id="6db24-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6db24-108">Property</span></span>|<span data-ttu-id="6db24-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6db24-109">Type</span></span>|<span data-ttu-id="6db24-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6db24-110">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="6db24-111">id</span><span class="sxs-lookup"><span data-stu-id="6db24-111">id</span></span>|<span data-ttu-id="6db24-112">String</span><span class="sxs-lookup"><span data-stu-id="6db24-112">String</span></span>| <span data-ttu-id="6db24-113">Propriedade Inherited.</span><span class="sxs-lookup"><span data-stu-id="6db24-113">Inherited property.</span></span> <span data-ttu-id="6db24-114">A ID da política de fluxos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="6db24-114">The ID of the authentication flows policy.</span></span> <span data-ttu-id="6db24-115">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6db24-115">Optional.</span></span> <span data-ttu-id="6db24-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6db24-116">Read-only.</span></span>
|<span data-ttu-id="6db24-117">displayName</span><span class="sxs-lookup"><span data-stu-id="6db24-117">displayName</span></span>|<span data-ttu-id="6db24-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6db24-118">String</span></span>| <span data-ttu-id="6db24-119">Propriedade Inherited.</span><span class="sxs-lookup"><span data-stu-id="6db24-119">Inherited property.</span></span> <span data-ttu-id="6db24-120">O nome legível da política.</span><span class="sxs-lookup"><span data-stu-id="6db24-120">The human-readable name of the policy.</span></span> <span data-ttu-id="6db24-121">Esta propriedade não é uma chave.</span><span class="sxs-lookup"><span data-stu-id="6db24-121">This property is not a key.</span></span> <span data-ttu-id="6db24-122">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6db24-122">Optional.</span></span> <span data-ttu-id="6db24-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6db24-123">Read-only.</span></span>|
|<span data-ttu-id="6db24-124">description</span><span class="sxs-lookup"><span data-stu-id="6db24-124">description</span></span>|<span data-ttu-id="6db24-125">String</span><span class="sxs-lookup"><span data-stu-id="6db24-125">String</span></span>|<span data-ttu-id="6db24-126">Propriedade Inherited.</span><span class="sxs-lookup"><span data-stu-id="6db24-126">Inherited property.</span></span> <span data-ttu-id="6db24-127">Uma descrição da política.</span><span class="sxs-lookup"><span data-stu-id="6db24-127">A description of the policy.</span></span> <span data-ttu-id="6db24-128">Esta propriedade não é uma chave.</span><span class="sxs-lookup"><span data-stu-id="6db24-128">This property is not a key.</span></span> <span data-ttu-id="6db24-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6db24-129">Optional.</span></span> <span data-ttu-id="6db24-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6db24-130">Read-only.</span></span>|
|<span data-ttu-id="6db24-131">selfServiceSignUp</span><span class="sxs-lookup"><span data-stu-id="6db24-131">selfServiceSignUp</span></span>|[<span data-ttu-id="6db24-132">selfServiceSignUpAuthenticationFlowConfiguration</span><span class="sxs-lookup"><span data-stu-id="6db24-132">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md) |<span data-ttu-id="6db24-133">Contém configurações do [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) que transmitem se a inscrição de autoatendimento está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="6db24-133">Contains [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) settings that convey whether self-service sign-up is enabled or disabled.</span></span> <span data-ttu-id="6db24-134">Esta propriedade não é uma chave.</span><span class="sxs-lookup"><span data-stu-id="6db24-134">This property is not a key.</span></span> <span data-ttu-id="6db24-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6db24-135">Optional.</span></span> <span data-ttu-id="6db24-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6db24-136">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6db24-137">Relações</span><span class="sxs-lookup"><span data-stu-id="6db24-137">Relationships</span></span>
<span data-ttu-id="6db24-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6db24-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6db24-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6db24-139">JSON representation</span></span>
<span data-ttu-id="6db24-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6db24-140">The following is a JSON representation of the resource.</span></span>
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
