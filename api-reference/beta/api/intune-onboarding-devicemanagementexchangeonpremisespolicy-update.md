---
title: Atualizar deviceManagementExchangeOnPremisesPolicy
description: Atualiza as propriedades de um objeto deviceManagementExchangeOnPremisesPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 329cac4b7fa550a648f0c820f02a1f69705efc0e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32528838"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="1778e-103">Atualizar deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="1778e-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="1778e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1778e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1778e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1778e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1778e-106">Atualiza as propriedades de um objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="1778e-106">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1778e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1778e-107">Prerequisites</span></span>
<span data-ttu-id="1778e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1778e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1778e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1778e-110">Permission type</span></span>|<span data-ttu-id="1778e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1778e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1778e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1778e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1778e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1778e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1778e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1778e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1778e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1778e-115">Not supported.</span></span>|
|<span data-ttu-id="1778e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1778e-116">Application</span></span>|<span data-ttu-id="1778e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1778e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1778e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1778e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="1778e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1778e-119">Request headers</span></span>
|<span data-ttu-id="1778e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1778e-120">Header</span></span>|<span data-ttu-id="1778e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1778e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1778e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1778e-122">Authorization</span></span>|<span data-ttu-id="1778e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1778e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1778e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1778e-124">Accept</span></span>|<span data-ttu-id="1778e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1778e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1778e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1778e-126">Request body</span></span>
<span data-ttu-id="1778e-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="1778e-127">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="1778e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1778e-128">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="1778e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1778e-129">Property</span></span>|<span data-ttu-id="1778e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1778e-130">Type</span></span>|<span data-ttu-id="1778e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1778e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1778e-132">id</span><span class="sxs-lookup"><span data-stu-id="1778e-132">id</span></span>|<span data-ttu-id="1778e-133">String</span><span class="sxs-lookup"><span data-stu-id="1778e-133">String</span></span>|<span data-ttu-id="1778e-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1778e-134">Not yet documented</span></span>|
|<span data-ttu-id="1778e-135">notificationContent</span><span class="sxs-lookup"><span data-stu-id="1778e-135">notificationContent</span></span>|<span data-ttu-id="1778e-136">Binário</span><span class="sxs-lookup"><span data-stu-id="1778e-136">Binary</span></span>|<span data-ttu-id="1778e-137">Texto de notificação que será enviado aos usuários colocados em quarentena por esta política.</span><span class="sxs-lookup"><span data-stu-id="1778e-137">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="1778e-138">Este é um HTML de matriz de bytes codificado por UTF8.</span><span class="sxs-lookup"><span data-stu-id="1778e-138">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="1778e-139">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="1778e-139">defaultAccessLevel</span></span>|[<span data-ttu-id="1778e-140">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="1778e-140">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="1778e-141">Estado de acesso padrão no Exchange.</span><span class="sxs-lookup"><span data-stu-id="1778e-141">Default access state in Exchange.</span></span> <span data-ttu-id="1778e-142">Essa regra se aplica globalmente a toda a organização do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1778e-142">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="1778e-143">Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="1778e-143">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="1778e-144">accessRules</span><span class="sxs-lookup"><span data-stu-id="1778e-144">accessRules</span></span>|<span data-ttu-id="1778e-145">coleção [deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)</span><span class="sxs-lookup"><span data-stu-id="1778e-145">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="1778e-146">A lista de regras de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="1778e-146">The list of device access rules in Exchange.</span></span> <span data-ttu-id="1778e-147">As regras de acesso são aplicadas globalmente em toda a organização do Exchange</span><span class="sxs-lookup"><span data-stu-id="1778e-147">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="1778e-148">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="1778e-148">knownDeviceClasses</span></span>|<span data-ttu-id="1778e-149">coleção [deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)</span><span class="sxs-lookup"><span data-stu-id="1778e-149">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="1778e-150">A lista de classes de dispositivo conhecidas para o Exchange</span><span class="sxs-lookup"><span data-stu-id="1778e-150">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="1778e-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="1778e-151">Response</span></span>
<span data-ttu-id="1778e-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1778e-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1778e-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1778e-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="1778e-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1778e-154">Request</span></span>
<span data-ttu-id="1778e-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1778e-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1778e-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="1778e-156">Response</span></span>
<span data-ttu-id="1778e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1778e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





