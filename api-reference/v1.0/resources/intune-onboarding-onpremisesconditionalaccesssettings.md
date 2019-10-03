---
title: Tipo de recurso onPremisesConditionalAccessSettings
description: Entidade singleton que representa as Configurações de acesso condicional do Exchange OnPremises para um locatário.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fa2c7030f7e9e1328c3b6dbc3f43e93bb10192e8
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367851"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="63234-103">Tipo de recurso onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="63234-103">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="63234-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63234-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63234-105">Entidade singleton que representa as Configurações de acesso condicional do Exchange OnPremises para um locatário.</span><span class="sxs-lookup"><span data-stu-id="63234-105">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="63234-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="63234-106">Methods</span></span>
|<span data-ttu-id="63234-107">Método</span><span class="sxs-lookup"><span data-stu-id="63234-107">Method</span></span>|<span data-ttu-id="63234-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="63234-108">Return Type</span></span>|<span data-ttu-id="63234-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="63234-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="63234-110">Obter onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="63234-110">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[<span data-ttu-id="63234-111">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="63234-111">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="63234-112">Ler propriedades e relações de objetos de [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="63234-112">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="63234-113">Atualizar onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="63234-113">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="63234-114">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="63234-114">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="63234-115">Atualizar as propriedades de um objeto de [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="63234-115">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="63234-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="63234-116">Properties</span></span>
|<span data-ttu-id="63234-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63234-117">Property</span></span>|<span data-ttu-id="63234-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="63234-118">Type</span></span>|<span data-ttu-id="63234-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="63234-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63234-120">id</span><span class="sxs-lookup"><span data-stu-id="63234-120">id</span></span>|<span data-ttu-id="63234-121">String</span><span class="sxs-lookup"><span data-stu-id="63234-121">String</span></span>|<span data-ttu-id="63234-122">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="63234-122">Not yet documented</span></span>|
|<span data-ttu-id="63234-123">enabled</span><span class="sxs-lookup"><span data-stu-id="63234-123">enabled</span></span>|<span data-ttu-id="63234-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="63234-124">Boolean</span></span>|<span data-ttu-id="63234-125">Indica se o acesso condicional local está habilitado para esta organização</span><span class="sxs-lookup"><span data-stu-id="63234-125">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="63234-126">includedGroups</span><span class="sxs-lookup"><span data-stu-id="63234-126">includedGroups</span></span>|<span data-ttu-id="63234-127">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="63234-127">Guid collection</span></span>|<span data-ttu-id="63234-128">Grupos de usuários que serão direcionados pelo acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="63234-128">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="63234-129">Todos os usuários nesses grupos deverão ter dispositivos móveis gerenciados e compatíveis com o acesso a email.</span><span class="sxs-lookup"><span data-stu-id="63234-129">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="63234-130">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="63234-130">excludedGroups</span></span>|<span data-ttu-id="63234-131">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="63234-131">Guid collection</span></span>|<span data-ttu-id="63234-132">Grupos de usuários que estarão isentos ao acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="63234-132">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="63234-133">Todos os usuários desses grupos ficarão isentos da política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="63234-133">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="63234-134">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="63234-134">overrideDefaultRule</span></span>|<span data-ttu-id="63234-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="63234-135">Boolean</span></span>|<span data-ttu-id="63234-136">Substitui as regras de acesso padrão ao permitir a um dispositivo que seja concedida a garantia de acesso.</span><span class="sxs-lookup"><span data-stu-id="63234-136">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63234-137">Relações</span><span class="sxs-lookup"><span data-stu-id="63234-137">Relationships</span></span>
<span data-ttu-id="63234-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="63234-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63234-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="63234-139">JSON Representation</span></span>
<span data-ttu-id="63234-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="63234-140">Here is a JSON representation of the resource.</span></span>
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




