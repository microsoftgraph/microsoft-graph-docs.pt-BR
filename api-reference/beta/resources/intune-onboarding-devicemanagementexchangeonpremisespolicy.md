---
title: tipo de recurso deviceManagementExchangeOnPremisesPolicy
description: Entidade singleton que representa a política local do Exchange configurada para um locatário.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3c3125ac19728a1f09f74a1245b1e11cc796b702
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998055"
---
# <a name="devicemanagementexchangeonpremisespolicy-resource-type"></a><span data-ttu-id="ab977-103">tipo de recurso deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="ab977-103">deviceManagementExchangeOnPremisesPolicy resource type</span></span>

> <span data-ttu-id="ab977-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ab977-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab977-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ab977-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab977-106">Entidade singleton que representa a política local do Exchange configurada para um locatário.</span><span class="sxs-lookup"><span data-stu-id="ab977-106">Singleton entity which represents the Exchange OnPremises policy configured for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="ab977-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ab977-107">Methods</span></span>
|<span data-ttu-id="ab977-108">Método</span><span class="sxs-lookup"><span data-stu-id="ab977-108">Method</span></span>|<span data-ttu-id="ab977-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ab977-109">Return Type</span></span>|<span data-ttu-id="ab977-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab977-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ab977-111">Obter deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="ab977-111">Get deviceManagementExchangeOnPremisesPolicy</span></span>](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-get.md)|[<span data-ttu-id="ab977-112">deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="ab977-112">deviceManagementExchangeOnPremisesPolicy</span></span>](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|<span data-ttu-id="ab977-113">Leia as propriedades e as relações do objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ab977-113">Read properties and relationships of the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>|
|[<span data-ttu-id="ab977-114">Atualizar deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="ab977-114">Update deviceManagementExchangeOnPremisesPolicy</span></span>](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-update.md)|[<span data-ttu-id="ab977-115">deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="ab977-115">deviceManagementExchangeOnPremisesPolicy</span></span>](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|<span data-ttu-id="ab977-116">Atualiza as propriedades de um objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ab977-116">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ab977-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab977-117">Properties</span></span>
|<span data-ttu-id="ab977-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab977-118">Property</span></span>|<span data-ttu-id="ab977-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab977-119">Type</span></span>|<span data-ttu-id="ab977-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab977-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab977-121">id</span><span class="sxs-lookup"><span data-stu-id="ab977-121">id</span></span>|<span data-ttu-id="ab977-122">String</span><span class="sxs-lookup"><span data-stu-id="ab977-122">String</span></span>|<span data-ttu-id="ab977-123">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ab977-123">Not yet documented</span></span>|
|<span data-ttu-id="ab977-124">notificationContent</span><span class="sxs-lookup"><span data-stu-id="ab977-124">notificationContent</span></span>|<span data-ttu-id="ab977-125">Binária</span><span class="sxs-lookup"><span data-stu-id="ab977-125">Binary</span></span>|<span data-ttu-id="ab977-126">Texto de notificação que será enviado aos usuários colocados em quarentena por esta política.</span><span class="sxs-lookup"><span data-stu-id="ab977-126">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="ab977-127">Este é um HTML de matriz de bytes codificado por UTF8.</span><span class="sxs-lookup"><span data-stu-id="ab977-127">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="ab977-128">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="ab977-128">defaultAccessLevel</span></span>|[<span data-ttu-id="ab977-129">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="ab977-129">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="ab977-130">Estado de acesso padrão no Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab977-130">Default access state in Exchange.</span></span> <span data-ttu-id="ab977-131">Essa regra se aplica globalmente a toda a organização do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab977-131">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="ab977-132">Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="ab977-132">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="ab977-133">accessRules</span><span class="sxs-lookup"><span data-stu-id="ab977-133">accessRules</span></span>|<span data-ttu-id="ab977-134">coleção [deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)</span><span class="sxs-lookup"><span data-stu-id="ab977-134">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="ab977-135">A lista de regras de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab977-135">The list of device access rules in Exchange.</span></span> <span data-ttu-id="ab977-136">As regras de acesso são aplicadas globalmente em toda a organização do Exchange</span><span class="sxs-lookup"><span data-stu-id="ab977-136">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="ab977-137">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="ab977-137">knownDeviceClasses</span></span>|<span data-ttu-id="ab977-138">coleção [deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)</span><span class="sxs-lookup"><span data-stu-id="ab977-138">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="ab977-139">A lista de classes de dispositivo conhecidas para o Exchange</span><span class="sxs-lookup"><span data-stu-id="ab977-139">The list of device classes known to Exchange</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab977-140">Relações</span><span class="sxs-lookup"><span data-stu-id="ab977-140">Relationships</span></span>
|<span data-ttu-id="ab977-141">Relação</span><span class="sxs-lookup"><span data-stu-id="ab977-141">Relationship</span></span>|<span data-ttu-id="ab977-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab977-142">Type</span></span>|<span data-ttu-id="ab977-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab977-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab977-144">conditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="ab977-144">conditionalAccessSettings</span></span>|[<span data-ttu-id="ab977-145">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="ab977-145">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="ab977-146">As configurações de acesso condicional do Exchange no local.</span><span class="sxs-lookup"><span data-stu-id="ab977-146">The Exchange on premises conditional access settings.</span></span> <span data-ttu-id="ab977-147">O acesso condicional no local exigirá que os dispositivos sejam registrados e estejam em conformidade para o acesso ao email</span><span class="sxs-lookup"><span data-stu-id="ab977-147">On premises conditional access will require devices to be both enrolled and compliant for mail access</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab977-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab977-148">JSON Representation</span></span>
<span data-ttu-id="ab977-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ab977-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExchangeOnPremisesPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "id": "String (identifier)",
  "notificationContent": "binary",
  "defaultAccessLevel": "String",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "String",
        "type": "String"
      },
      "accessLevel": "String"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "String",
      "type": "String"
    }
  ]
}
```





