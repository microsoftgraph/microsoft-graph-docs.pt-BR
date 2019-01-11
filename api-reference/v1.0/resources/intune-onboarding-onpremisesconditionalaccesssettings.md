---
title: Tipo de recurso onPremisesConditionalAccessSettings
description: Entidade singleton que representa as Configurações de acesso condicional do Exchange OnPremises para um locatário.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 88d513cc59b9570b355e67fa417a9856519cf551
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875989"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="f868d-103">Tipo de recurso onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="f868d-103">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="f868d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f868d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f868d-105">Entidade singleton que representa as Configurações de acesso condicional do Exchange OnPremises para um locatário.</span><span class="sxs-lookup"><span data-stu-id="f868d-105">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="f868d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f868d-106">Methods</span></span>
|<span data-ttu-id="f868d-107">Método</span><span class="sxs-lookup"><span data-stu-id="f868d-107">Method</span></span>|<span data-ttu-id="f868d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f868d-108">Return Type</span></span>|<span data-ttu-id="f868d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f868d-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f868d-110">Obter onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="f868d-110">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[<span data-ttu-id="f868d-111">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="f868d-111">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="f868d-112">Ler propriedades e relações de objetos de [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="f868d-112">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="f868d-113">Atualizar onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="f868d-113">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="f868d-114">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="f868d-114">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="f868d-115">Atualizar as propriedades de um objeto de [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="f868d-115">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f868d-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f868d-116">Properties</span></span>
|<span data-ttu-id="f868d-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f868d-117">Property</span></span>|<span data-ttu-id="f868d-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="f868d-118">Type</span></span>|<span data-ttu-id="f868d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f868d-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f868d-120">id</span><span class="sxs-lookup"><span data-stu-id="f868d-120">id</span></span>|<span data-ttu-id="f868d-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f868d-121">String</span></span>|<span data-ttu-id="f868d-122">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f868d-122">Not yet documented</span></span>|
|<span data-ttu-id="f868d-123">enabled</span><span class="sxs-lookup"><span data-stu-id="f868d-123">enabled</span></span>|<span data-ttu-id="f868d-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="f868d-124">Boolean</span></span>|<span data-ttu-id="f868d-125">Indica se o acesso condicional local está habilitado para esta organização</span><span class="sxs-lookup"><span data-stu-id="f868d-125">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="f868d-126">includedGroups</span><span class="sxs-lookup"><span data-stu-id="f868d-126">includedGroups</span></span>|<span data-ttu-id="f868d-127">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="f868d-127">Guid collection</span></span>|<span data-ttu-id="f868d-128">Grupos de usuários que serão direcionados pelo acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="f868d-128">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="f868d-129">Todos os usuários nesses grupos deverão ter dispositivos móveis gerenciados e compatíveis com o acesso a email.</span><span class="sxs-lookup"><span data-stu-id="f868d-129">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="f868d-130">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="f868d-130">excludedGroups</span></span>|<span data-ttu-id="f868d-131">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="f868d-131">Guid collection</span></span>|<span data-ttu-id="f868d-132">Grupos de usuários que estarão isentos ao acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="f868d-132">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="f868d-133">Todos os usuários desses grupos ficarão isentos da política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="f868d-133">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="f868d-134">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="f868d-134">overrideDefaultRule</span></span>|<span data-ttu-id="f868d-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="f868d-135">Boolean</span></span>|<span data-ttu-id="f868d-136">Substitui as regras de acesso padrão ao permitir a um dispositivo que seja concedida a garantia de acesso.</span><span class="sxs-lookup"><span data-stu-id="f868d-136">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f868d-137">Relações</span><span class="sxs-lookup"><span data-stu-id="f868d-137">Relationships</span></span>
<span data-ttu-id="f868d-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f868d-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f868d-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f868d-139">JSON Representation</span></span>
<span data-ttu-id="f868d-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f868d-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "Guid"
  ],
  "excludedGroups": [
    "Guid"
  ],
  "overrideDefaultRule": true
}
```



