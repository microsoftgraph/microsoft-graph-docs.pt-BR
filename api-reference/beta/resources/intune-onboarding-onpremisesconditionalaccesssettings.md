---
title: Tipo de recurso onPremisesConditionalAccessSettings
description: Entidade singleton que representa as Configurações de acesso condicional do Exchange OnPremises para um locatário.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c2a696696a25382778ef043d6dcae1320ed75a58
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358010"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="0971a-103">Tipo de recurso onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="0971a-103">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="0971a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0971a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0971a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0971a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0971a-106">Entidade singleton que representa as Configurações de acesso condicional do Exchange OnPremises para um locatário.</span><span class="sxs-lookup"><span data-stu-id="0971a-106">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="0971a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="0971a-107">Methods</span></span>
|<span data-ttu-id="0971a-108">Método</span><span class="sxs-lookup"><span data-stu-id="0971a-108">Method</span></span>|<span data-ttu-id="0971a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0971a-109">Return Type</span></span>|<span data-ttu-id="0971a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0971a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0971a-111">Obter onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="0971a-111">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[<span data-ttu-id="0971a-112">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="0971a-112">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="0971a-113">Ler propriedades e relações de objetos de [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="0971a-113">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="0971a-114">Atualizar onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="0971a-114">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="0971a-115">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="0971a-115">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="0971a-116">Atualizar as propriedades de um objeto de [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="0971a-116">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0971a-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0971a-117">Properties</span></span>
|<span data-ttu-id="0971a-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0971a-118">Property</span></span>|<span data-ttu-id="0971a-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="0971a-119">Type</span></span>|<span data-ttu-id="0971a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0971a-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0971a-121">id</span><span class="sxs-lookup"><span data-stu-id="0971a-121">id</span></span>|<span data-ttu-id="0971a-122">String</span><span class="sxs-lookup"><span data-stu-id="0971a-122">String</span></span>|<span data-ttu-id="0971a-123">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0971a-123">Not yet documented</span></span>|
|<span data-ttu-id="0971a-124">enabled</span><span class="sxs-lookup"><span data-stu-id="0971a-124">enabled</span></span>|<span data-ttu-id="0971a-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="0971a-125">Boolean</span></span>|<span data-ttu-id="0971a-126">Indica se o acesso condicional local está habilitado para esta organização</span><span class="sxs-lookup"><span data-stu-id="0971a-126">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="0971a-127">includedGroups</span><span class="sxs-lookup"><span data-stu-id="0971a-127">includedGroups</span></span>|<span data-ttu-id="0971a-128">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="0971a-128">Guid collection</span></span>|<span data-ttu-id="0971a-129">Grupos de usuários que serão direcionados pelo acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="0971a-129">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="0971a-130">Todos os usuários nesses grupos deverão ter dispositivos móveis gerenciados e compatíveis com o acesso a email.</span><span class="sxs-lookup"><span data-stu-id="0971a-130">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="0971a-131">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="0971a-131">excludedGroups</span></span>|<span data-ttu-id="0971a-132">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="0971a-132">Guid collection</span></span>|<span data-ttu-id="0971a-133">Grupos de usuários que estarão isentos ao acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="0971a-133">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="0971a-134">Todos os usuários desses grupos ficarão isentos da política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="0971a-134">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="0971a-135">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="0971a-135">overrideDefaultRule</span></span>|<span data-ttu-id="0971a-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="0971a-136">Boolean</span></span>|<span data-ttu-id="0971a-137">Substitui as regras de acesso padrão ao permitir a um dispositivo que seja concedida a garantia de acesso.</span><span class="sxs-lookup"><span data-stu-id="0971a-137">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0971a-138">Relações</span><span class="sxs-lookup"><span data-stu-id="0971a-138">Relationships</span></span>
<span data-ttu-id="0971a-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0971a-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0971a-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0971a-140">JSON Representation</span></span>
<span data-ttu-id="0971a-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0971a-141">Here is a JSON representation of the resource.</span></span>
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



