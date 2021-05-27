---
title: tipo de recurso authenticationMethodsRegistrationCampaign
description: Representa as configurações usadas para executar campanhas para pressionar os usuários a configurar métodos de autenticação direcionada.
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: be989bc86e5e708a89cd33c700e57edce42d9e50
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682863"
---
# <a name="authenticationmethodsregistrationcampaign-resource-type"></a><span data-ttu-id="b7877-103">tipo de recurso authenticationMethodsRegistrationCampaign</span><span class="sxs-lookup"><span data-stu-id="b7877-103">authenticationMethodsRegistrationCampaign resource type</span></span>

<span data-ttu-id="b7877-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7877-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7877-105">Representa as configurações usadas para executar campanhas para pressionar os usuários a configurar métodos de autenticação direcionada.</span><span class="sxs-lookup"><span data-stu-id="b7877-105">Represents the settings used to run campaigns to push users to set up targeted authentication methods.</span></span> <span data-ttu-id="b7877-106">Os usuários são solicitados a configurar o método de autenticação após concluirem com êxito um desafio de MFA.</span><span class="sxs-lookup"><span data-stu-id="b7877-106">Users are prompted to set up the authentication method after they successfully complete a MFA challenge.</span></span> <span data-ttu-id="b7877-107">Disponível apenas para o aplicativo Microsoft Authenticator para MFA.</span><span class="sxs-lookup"><span data-stu-id="b7877-107">Only available for the Microsoft Authenticator app for MFA.</span></span>

## <a name="properties"></a><span data-ttu-id="b7877-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b7877-108">Properties</span></span>
|<span data-ttu-id="b7877-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7877-109">Property</span></span>|<span data-ttu-id="b7877-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7877-110">Type</span></span>|<span data-ttu-id="b7877-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7877-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7877-112">excludeTargets</span><span class="sxs-lookup"><span data-stu-id="b7877-112">excludeTargets</span></span>|<span data-ttu-id="b7877-113">[Coleção excludeTarget](../resources/excludetarget.md)</span><span class="sxs-lookup"><span data-stu-id="b7877-113">[excludeTarget](../resources/excludetarget.md) collection</span></span>|<span data-ttu-id="b7877-114">Usuários e grupos de usuários excluídos de serem solicitados a configurar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="b7877-114">Users and groups of users that are excluded from being prompted to set up the authentication method.</span></span>|
|<span data-ttu-id="b7877-115">includeTargets</span><span class="sxs-lookup"><span data-stu-id="b7877-115">includeTargets</span></span>|<span data-ttu-id="b7877-116">[coleção authenticationMethodsRegistrationCampaignIncludeTarget](../resources/authenticationmethodsregistrationcampaignincludetarget.md)</span><span class="sxs-lookup"><span data-stu-id="b7877-116">[authenticationMethodsRegistrationCampaignIncludeTarget](../resources/authenticationmethodsregistrationcampaignincludetarget.md) collection</span></span>|<span data-ttu-id="b7877-117">Usuários e grupos de usuários solicitados a configurar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="b7877-117">Users and groups of users that are prompted to set up the authentication method.</span></span>|
|<span data-ttu-id="b7877-118">snoozeDurationInDays</span><span class="sxs-lookup"><span data-stu-id="b7877-118">snoozeDurationInDays</span></span>|<span data-ttu-id="b7877-119">Int32</span><span class="sxs-lookup"><span data-stu-id="b7877-119">Int32</span></span>|<span data-ttu-id="b7877-120">Especifica o número de dias em que o usuário vê um prompt novamente se ele selecionar "Não agora" e esnome o prompt.</span><span class="sxs-lookup"><span data-stu-id="b7877-120">Specifies the number of days that the user sees a prompt again if they select "Not now" and snoozes the prompt.</span></span> <span data-ttu-id="b7877-121">Mínimo de 0 dias.</span><span class="sxs-lookup"><span data-stu-id="b7877-121">Minimum 0 days.</span></span> <span data-ttu-id="b7877-122">Máximo: 14 dias.</span><span class="sxs-lookup"><span data-stu-id="b7877-122">Maximum: 14 days.</span></span> <span data-ttu-id="b7877-123">Se o valor for "0" – o usuário será solicitado durante cada tentativa de MFA.</span><span class="sxs-lookup"><span data-stu-id="b7877-123">If the value is “0” – The user is prompted during every MFA attempt.</span></span>|
|<span data-ttu-id="b7877-124">state</span><span class="sxs-lookup"><span data-stu-id="b7877-124">state</span></span>|<span data-ttu-id="b7877-125">advancedConfigState</span><span class="sxs-lookup"><span data-stu-id="b7877-125">advancedConfigState</span></span>|<span data-ttu-id="b7877-126">Habilitar ou desabilitar o recurso.</span><span class="sxs-lookup"><span data-stu-id="b7877-126">Enable or disable the feature.</span></span> <span data-ttu-id="b7877-127">Os valores possíveis são: `default`, `enabled`, `disabled`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b7877-127">Possible values are: `default`, `enabled`, `disabled`, `unknownFutureValue`.</span></span> <span data-ttu-id="b7877-128">O valor é usado quando a configuração não foi definida explicitamente e usa o comportamento padrão do `default` Azure AD para a configuração.</span><span class="sxs-lookup"><span data-stu-id="b7877-128">The `default` value is used when the configuration hasn't been explicitly set and uses the default behavior of Azure AD for the setting.</span></span> <span data-ttu-id="b7877-129">O valor padrão é `disabled`.</span><span class="sxs-lookup"><span data-stu-id="b7877-129">The default value is `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7877-130">Relações</span><span class="sxs-lookup"><span data-stu-id="b7877-130">Relationships</span></span>
<span data-ttu-id="b7877-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b7877-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7877-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b7877-132">JSON representation</span></span>
<span data-ttu-id="b7877-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b7877-133">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaign"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsRegistrationCampaign",
  "excludeTargets": [
    {
      "@odata.type": "microsoft.graph.excludeTarget"
    }
  ],
  "includeTargets": [
    {
      "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaignIncludeTarget"
    }
  ],
  "snoozeDurationInDays": "Integer",
  "state": "String"
}
```
