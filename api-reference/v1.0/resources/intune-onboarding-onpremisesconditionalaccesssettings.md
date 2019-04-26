---
title: Tipo de recurso onPremisesConditionalAccessSettings
description: Entidade singleton que representa as Configurações de acesso condicional do Exchange OnPremises para um locatário.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f307b137a39323e5e3c6b644602b1c0df3ab5512
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563746"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="e8da3-103">Tipo de recurso onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="e8da3-103">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="e8da3-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8da3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8da3-105">Entidade singleton que representa as Configurações de acesso condicional do Exchange OnPremises para um locatário.</span><span class="sxs-lookup"><span data-stu-id="e8da3-105">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="e8da3-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="e8da3-106">Methods</span></span>
|<span data-ttu-id="e8da3-107">Método</span><span class="sxs-lookup"><span data-stu-id="e8da3-107">Method</span></span>|<span data-ttu-id="e8da3-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e8da3-108">Return Type</span></span>|<span data-ttu-id="e8da3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8da3-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e8da3-110">Obter onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="e8da3-110">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[<span data-ttu-id="e8da3-111">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="e8da3-111">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="e8da3-112">Ler propriedades e relações de objetos de [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="e8da3-112">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="e8da3-113">Atualizar onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="e8da3-113">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="e8da3-114">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="e8da3-114">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="e8da3-115">Atualizar as propriedades de um objeto de [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="e8da3-115">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e8da3-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8da3-116">Properties</span></span>
|<span data-ttu-id="e8da3-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8da3-117">Property</span></span>|<span data-ttu-id="e8da3-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8da3-118">Type</span></span>|<span data-ttu-id="e8da3-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8da3-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8da3-120">id</span><span class="sxs-lookup"><span data-stu-id="e8da3-120">id</span></span>|<span data-ttu-id="e8da3-121">String</span><span class="sxs-lookup"><span data-stu-id="e8da3-121">String</span></span>|<span data-ttu-id="e8da3-122">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e8da3-122">Not yet documented</span></span>|
|<span data-ttu-id="e8da3-123">enabled</span><span class="sxs-lookup"><span data-stu-id="e8da3-123">enabled</span></span>|<span data-ttu-id="e8da3-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8da3-124">Boolean</span></span>|<span data-ttu-id="e8da3-125">Indica se o acesso condicional local está habilitado para esta organização</span><span class="sxs-lookup"><span data-stu-id="e8da3-125">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="e8da3-126">includedGroups</span><span class="sxs-lookup"><span data-stu-id="e8da3-126">includedGroups</span></span>|<span data-ttu-id="e8da3-127">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="e8da3-127">Guid collection</span></span>|<span data-ttu-id="e8da3-128">Grupos de usuários que serão direcionados pelo acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="e8da3-128">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="e8da3-129">Todos os usuários nesses grupos deverão ter dispositivos móveis gerenciados e compatíveis com o acesso a email.</span><span class="sxs-lookup"><span data-stu-id="e8da3-129">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="e8da3-130">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="e8da3-130">excludedGroups</span></span>|<span data-ttu-id="e8da3-131">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="e8da3-131">Guid collection</span></span>|<span data-ttu-id="e8da3-132">Grupos de usuários que estarão isentos ao acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="e8da3-132">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="e8da3-133">Todos os usuários desses grupos ficarão isentos da política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="e8da3-133">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="e8da3-134">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="e8da3-134">overrideDefaultRule</span></span>|<span data-ttu-id="e8da3-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="e8da3-135">Boolean</span></span>|<span data-ttu-id="e8da3-136">Substitui as regras de acesso padrão ao permitir a um dispositivo que seja concedida a garantia de acesso.</span><span class="sxs-lookup"><span data-stu-id="e8da3-136">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8da3-137">Relações</span><span class="sxs-lookup"><span data-stu-id="e8da3-137">Relationships</span></span>
<span data-ttu-id="e8da3-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e8da3-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8da3-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8da3-139">JSON Representation</span></span>
<span data-ttu-id="e8da3-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e8da3-140">Here is a JSON representation of the resource.</span></span>
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



