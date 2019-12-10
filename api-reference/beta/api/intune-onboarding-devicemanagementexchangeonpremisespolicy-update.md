---
title: Atualizar deviceManagementExchangeOnPremisesPolicy
description: Atualiza as propriedades de um objeto deviceManagementExchangeOnPremisesPolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3fff7cd3bbcacbbfdbff9156c805381d59a6dffe
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941719"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="01601-103">Atualizar deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="01601-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="01601-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="01601-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01601-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="01601-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01601-106">Atualiza as propriedades de um objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="01601-106">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01601-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="01601-107">Prerequisites</span></span>
<span data-ttu-id="01601-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01601-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01601-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01601-110">Permission type</span></span>|<span data-ttu-id="01601-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="01601-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01601-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01601-112">Delegated (work or school account)</span></span>|<span data-ttu-id="01601-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01601-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="01601-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01601-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01601-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01601-115">Not supported.</span></span>|
|<span data-ttu-id="01601-116">Application</span><span class="sxs-lookup"><span data-stu-id="01601-116">Application</span></span>|<span data-ttu-id="01601-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01601-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01601-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01601-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="01601-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01601-119">Request headers</span></span>
|<span data-ttu-id="01601-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01601-120">Header</span></span>|<span data-ttu-id="01601-121">Valor</span><span class="sxs-lookup"><span data-stu-id="01601-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01601-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="01601-122">Authorization</span></span>|<span data-ttu-id="01601-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01601-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01601-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="01601-124">Accept</span></span>|<span data-ttu-id="01601-125">application/json</span><span class="sxs-lookup"><span data-stu-id="01601-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01601-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01601-126">Request body</span></span>
<span data-ttu-id="01601-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="01601-127">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="01601-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span><span class="sxs-lookup"><span data-stu-id="01601-128">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="01601-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01601-129">Property</span></span>|<span data-ttu-id="01601-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="01601-130">Type</span></span>|<span data-ttu-id="01601-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="01601-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01601-132">id</span><span class="sxs-lookup"><span data-stu-id="01601-132">id</span></span>|<span data-ttu-id="01601-133">String</span><span class="sxs-lookup"><span data-stu-id="01601-133">String</span></span>|<span data-ttu-id="01601-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="01601-134">Not yet documented</span></span>|
|<span data-ttu-id="01601-135">notificationContent</span><span class="sxs-lookup"><span data-stu-id="01601-135">notificationContent</span></span>|<span data-ttu-id="01601-136">Binária</span><span class="sxs-lookup"><span data-stu-id="01601-136">Binary</span></span>|<span data-ttu-id="01601-137">Texto de notificação que será enviado aos usuários colocados em quarentena por esta política.</span><span class="sxs-lookup"><span data-stu-id="01601-137">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="01601-138">Este é um HTML de matriz de bytes codificado por UTF8.</span><span class="sxs-lookup"><span data-stu-id="01601-138">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="01601-139">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="01601-139">defaultAccessLevel</span></span>|[<span data-ttu-id="01601-140">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="01601-140">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="01601-141">Estado de acesso padrão no Exchange.</span><span class="sxs-lookup"><span data-stu-id="01601-141">Default access state in Exchange.</span></span> <span data-ttu-id="01601-142">Essa regra se aplica globalmente a toda a organização do Exchange.</span><span class="sxs-lookup"><span data-stu-id="01601-142">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="01601-143">Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="01601-143">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="01601-144">accessRules</span><span class="sxs-lookup"><span data-stu-id="01601-144">accessRules</span></span>|<span data-ttu-id="01601-145">coleção [deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)</span><span class="sxs-lookup"><span data-stu-id="01601-145">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="01601-146">A lista de regras de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="01601-146">The list of device access rules in Exchange.</span></span> <span data-ttu-id="01601-147">As regras de acesso são aplicadas globalmente em toda a organização do Exchange</span><span class="sxs-lookup"><span data-stu-id="01601-147">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="01601-148">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="01601-148">knownDeviceClasses</span></span>|<span data-ttu-id="01601-149">coleção [deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)</span><span class="sxs-lookup"><span data-stu-id="01601-149">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="01601-150">A lista de classes de dispositivo conhecidas para o Exchange</span><span class="sxs-lookup"><span data-stu-id="01601-150">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="01601-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="01601-151">Response</span></span>
<span data-ttu-id="01601-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01601-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01601-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01601-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="01601-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01601-154">Request</span></span>
<span data-ttu-id="01601-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01601-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="01601-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="01601-156">Response</span></span>
<span data-ttu-id="01601-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01601-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





