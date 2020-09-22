---
title: Atualizar deviceManagementExchangeOnPremisesPolicy
description: Atualiza as propriedades de um objeto deviceManagementExchangeOnPremisesPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 733691e67d0002848e84f4f9e105068f98e2d914
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072183"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="f2988-103">Atualizar deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="f2988-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

<span data-ttu-id="f2988-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2988-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2988-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2988-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2988-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2988-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2988-107">Atualiza as propriedades de um objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="f2988-107">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2988-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2988-108">Prerequisites</span></span>
<span data-ttu-id="f2988-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2988-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2988-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2988-111">Permission type</span></span>|<span data-ttu-id="f2988-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2988-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2988-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2988-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2988-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2988-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f2988-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2988-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2988-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2988-116">Not supported.</span></span>|
|<span data-ttu-id="f2988-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2988-117">Application</span></span>|<span data-ttu-id="f2988-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2988-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2988-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2988-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="f2988-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2988-120">Request headers</span></span>
|<span data-ttu-id="f2988-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2988-121">Header</span></span>|<span data-ttu-id="f2988-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f2988-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2988-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2988-123">Authorization</span></span>|<span data-ttu-id="f2988-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2988-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2988-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2988-125">Accept</span></span>|<span data-ttu-id="f2988-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2988-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2988-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2988-127">Request body</span></span>
<span data-ttu-id="f2988-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="f2988-128">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="f2988-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f2988-129">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="f2988-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2988-130">Property</span></span>|<span data-ttu-id="f2988-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2988-131">Type</span></span>|<span data-ttu-id="f2988-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2988-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2988-133">id</span><span class="sxs-lookup"><span data-stu-id="f2988-133">id</span></span>|<span data-ttu-id="f2988-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2988-134">String</span></span>|<span data-ttu-id="f2988-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f2988-135">Not yet documented</span></span>|
|<span data-ttu-id="f2988-136">notificationContent</span><span class="sxs-lookup"><span data-stu-id="f2988-136">notificationContent</span></span>|<span data-ttu-id="f2988-137">Binária</span><span class="sxs-lookup"><span data-stu-id="f2988-137">Binary</span></span>|<span data-ttu-id="f2988-138">Texto de notificação que será enviado aos usuários colocados em quarentena por esta política.</span><span class="sxs-lookup"><span data-stu-id="f2988-138">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="f2988-139">Este é um HTML de matriz de bytes codificado por UTF8.</span><span class="sxs-lookup"><span data-stu-id="f2988-139">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="f2988-140">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="f2988-140">defaultAccessLevel</span></span>|[<span data-ttu-id="f2988-141">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="f2988-141">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="f2988-142">Estado de acesso padrão no Exchange.</span><span class="sxs-lookup"><span data-stu-id="f2988-142">Default access state in Exchange.</span></span> <span data-ttu-id="f2988-143">Essa regra se aplica globalmente a toda a organização do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f2988-143">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="f2988-144">Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="f2988-144">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="f2988-145">accessRules</span><span class="sxs-lookup"><span data-stu-id="f2988-145">accessRules</span></span>|<span data-ttu-id="f2988-146">coleção [deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)</span><span class="sxs-lookup"><span data-stu-id="f2988-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="f2988-147">A lista de regras de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="f2988-147">The list of device access rules in Exchange.</span></span> <span data-ttu-id="f2988-148">As regras de acesso são aplicadas globalmente em toda a organização do Exchange</span><span class="sxs-lookup"><span data-stu-id="f2988-148">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="f2988-149">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="f2988-149">knownDeviceClasses</span></span>|<span data-ttu-id="f2988-150">coleção [deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)</span><span class="sxs-lookup"><span data-stu-id="f2988-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="f2988-151">A lista de classes de dispositivo conhecidas para o Exchange</span><span class="sxs-lookup"><span data-stu-id="f2988-151">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="f2988-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2988-152">Response</span></span>
<span data-ttu-id="f2988-153">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2988-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2988-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2988-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2988-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2988-155">Request</span></span>
<span data-ttu-id="f2988-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2988-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f2988-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2988-157">Response</span></span>
<span data-ttu-id="f2988-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2988-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






