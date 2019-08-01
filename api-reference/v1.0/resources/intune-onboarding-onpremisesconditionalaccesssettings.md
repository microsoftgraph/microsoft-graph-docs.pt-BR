---
title: Tipo de recurso onPremisesConditionalAccessSettings
description: Entidade singleton que representa as Configurações de acesso condicional do Exchange OnPremises para um locatário.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f4152cd37907b8623b616845b2d82272a9ad83bd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037356"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="ea266-103">Tipo de recurso onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="ea266-103">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="ea266-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ea266-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea266-105">Entidade singleton que representa as Configurações de acesso condicional do Exchange OnPremises para um locatário.</span><span class="sxs-lookup"><span data-stu-id="ea266-105">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="ea266-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ea266-106">Methods</span></span>
|<span data-ttu-id="ea266-107">Método</span><span class="sxs-lookup"><span data-stu-id="ea266-107">Method</span></span>|<span data-ttu-id="ea266-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ea266-108">Return Type</span></span>|<span data-ttu-id="ea266-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea266-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ea266-110">Obter onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="ea266-110">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[<span data-ttu-id="ea266-111">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="ea266-111">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="ea266-112">Ler propriedades e relações de objetos de [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="ea266-112">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="ea266-113">Atualizar onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="ea266-113">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="ea266-114">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="ea266-114">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="ea266-115">Atualizar as propriedades de um objeto de [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="ea266-115">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ea266-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea266-116">Properties</span></span>
|<span data-ttu-id="ea266-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea266-117">Property</span></span>|<span data-ttu-id="ea266-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea266-118">Type</span></span>|<span data-ttu-id="ea266-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea266-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea266-120">id</span><span class="sxs-lookup"><span data-stu-id="ea266-120">id</span></span>|<span data-ttu-id="ea266-121">String</span><span class="sxs-lookup"><span data-stu-id="ea266-121">String</span></span>|<span data-ttu-id="ea266-122">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ea266-122">Not yet documented</span></span>|
|<span data-ttu-id="ea266-123">enabled</span><span class="sxs-lookup"><span data-stu-id="ea266-123">enabled</span></span>|<span data-ttu-id="ea266-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea266-124">Boolean</span></span>|<span data-ttu-id="ea266-125">Indica se o acesso condicional local está habilitado para esta organização</span><span class="sxs-lookup"><span data-stu-id="ea266-125">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="ea266-126">includedGroups</span><span class="sxs-lookup"><span data-stu-id="ea266-126">includedGroups</span></span>|<span data-ttu-id="ea266-127">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="ea266-127">Guid collection</span></span>|<span data-ttu-id="ea266-128">Grupos de usuários que serão direcionados pelo acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="ea266-128">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="ea266-129">Todos os usuários nesses grupos deverão ter dispositivos móveis gerenciados e compatíveis com o acesso a email.</span><span class="sxs-lookup"><span data-stu-id="ea266-129">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="ea266-130">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="ea266-130">excludedGroups</span></span>|<span data-ttu-id="ea266-131">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="ea266-131">Guid collection</span></span>|<span data-ttu-id="ea266-132">Grupos de usuários que estarão isentos ao acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="ea266-132">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="ea266-133">Todos os usuários desses grupos ficarão isentos da política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="ea266-133">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="ea266-134">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="ea266-134">overrideDefaultRule</span></span>|<span data-ttu-id="ea266-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="ea266-135">Boolean</span></span>|<span data-ttu-id="ea266-136">Substitui as regras de acesso padrão ao permitir a um dispositivo que seja concedida a garantia de acesso.</span><span class="sxs-lookup"><span data-stu-id="ea266-136">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea266-137">Relações</span><span class="sxs-lookup"><span data-stu-id="ea266-137">Relationships</span></span>
<span data-ttu-id="ea266-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea266-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea266-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea266-139">JSON Representation</span></span>
<span data-ttu-id="ea266-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea266-140">Here is a JSON representation of the resource.</span></span>
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



