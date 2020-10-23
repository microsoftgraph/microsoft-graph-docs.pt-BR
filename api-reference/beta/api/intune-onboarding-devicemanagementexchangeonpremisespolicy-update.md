---
title: Atualizar deviceManagementExchangeOnPremisesPolicy
description: Atualiza as propriedades de um objeto deviceManagementExchangeOnPremisesPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1748a71bafe7f96313e0df44c73b4d88af1b70d5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727658"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="69ce0-103">Atualizar deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="69ce0-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

<span data-ttu-id="69ce0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69ce0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69ce0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="69ce0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69ce0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="69ce0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69ce0-107">Atualiza as propriedades de um objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="69ce0-107">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69ce0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="69ce0-108">Prerequisites</span></span>
<span data-ttu-id="69ce0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69ce0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69ce0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69ce0-111">Permission type</span></span>|<span data-ttu-id="69ce0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="69ce0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69ce0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69ce0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69ce0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69ce0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="69ce0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69ce0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69ce0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69ce0-116">Not supported.</span></span>|
|<span data-ttu-id="69ce0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69ce0-117">Application</span></span>|<span data-ttu-id="69ce0-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69ce0-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69ce0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69ce0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="69ce0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69ce0-120">Request headers</span></span>
|<span data-ttu-id="69ce0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="69ce0-121">Header</span></span>|<span data-ttu-id="69ce0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="69ce0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69ce0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="69ce0-123">Authorization</span></span>|<span data-ttu-id="69ce0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69ce0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69ce0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="69ce0-125">Accept</span></span>|<span data-ttu-id="69ce0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69ce0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69ce0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69ce0-127">Request body</span></span>
<span data-ttu-id="69ce0-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="69ce0-128">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="69ce0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span><span class="sxs-lookup"><span data-stu-id="69ce0-129">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="69ce0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69ce0-130">Property</span></span>|<span data-ttu-id="69ce0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="69ce0-131">Type</span></span>|<span data-ttu-id="69ce0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="69ce0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69ce0-133">id</span><span class="sxs-lookup"><span data-stu-id="69ce0-133">id</span></span>|<span data-ttu-id="69ce0-134">String</span><span class="sxs-lookup"><span data-stu-id="69ce0-134">String</span></span>|<span data-ttu-id="69ce0-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="69ce0-135">Not yet documented</span></span>|
|<span data-ttu-id="69ce0-136">notificationContent</span><span class="sxs-lookup"><span data-stu-id="69ce0-136">notificationContent</span></span>|<span data-ttu-id="69ce0-137">Binária</span><span class="sxs-lookup"><span data-stu-id="69ce0-137">Binary</span></span>|<span data-ttu-id="69ce0-138">Texto de notificação que será enviado aos usuários colocados em quarentena por esta política.</span><span class="sxs-lookup"><span data-stu-id="69ce0-138">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="69ce0-139">Este é um HTML de matriz de bytes codificado por UTF8.</span><span class="sxs-lookup"><span data-stu-id="69ce0-139">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="69ce0-140">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="69ce0-140">defaultAccessLevel</span></span>|[<span data-ttu-id="69ce0-141">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="69ce0-141">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="69ce0-142">Estado de acesso padrão no Exchange.</span><span class="sxs-lookup"><span data-stu-id="69ce0-142">Default access state in Exchange.</span></span> <span data-ttu-id="69ce0-143">Essa regra se aplica globalmente a toda a organização do Exchange.</span><span class="sxs-lookup"><span data-stu-id="69ce0-143">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="69ce0-144">Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="69ce0-144">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="69ce0-145">accessRules</span><span class="sxs-lookup"><span data-stu-id="69ce0-145">accessRules</span></span>|<span data-ttu-id="69ce0-146">coleção [deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)</span><span class="sxs-lookup"><span data-stu-id="69ce0-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="69ce0-147">A lista de regras de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="69ce0-147">The list of device access rules in Exchange.</span></span> <span data-ttu-id="69ce0-148">As regras de acesso são aplicadas globalmente em toda a organização do Exchange</span><span class="sxs-lookup"><span data-stu-id="69ce0-148">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="69ce0-149">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="69ce0-149">knownDeviceClasses</span></span>|<span data-ttu-id="69ce0-150">coleção [deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)</span><span class="sxs-lookup"><span data-stu-id="69ce0-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="69ce0-151">A lista de classes de dispositivo conhecidas para o Exchange</span><span class="sxs-lookup"><span data-stu-id="69ce0-151">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="69ce0-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="69ce0-152">Response</span></span>
<span data-ttu-id="69ce0-153">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69ce0-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69ce0-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69ce0-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="69ce0-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69ce0-155">Request</span></span>
<span data-ttu-id="69ce0-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="69ce0-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
Content-type: application/json
Content-length: 665

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
  "defaultAccessLevel": "allow",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      },
      "accessLevel": "allow"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "Name value",
      "type": "model"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="69ce0-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="69ce0-157">Response</span></span>
<span data-ttu-id="69ce0-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69ce0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 714

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "id": "16e76336-6336-16e7-3663-e7163663e716",
  "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
  "defaultAccessLevel": "allow",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      },
      "accessLevel": "allow"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "Name value",
      "type": "model"
    }
  ]
}
```





