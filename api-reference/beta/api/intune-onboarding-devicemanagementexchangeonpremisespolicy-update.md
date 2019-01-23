---
title: Atualizar deviceManagementExchangeOnPremisesPolicy
description: Atualize as propriedades de um objeto deviceManagementExchangeOnPremisesPolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 633f1b80895bd84c27c57b5cee26aa286b1d0e49
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407204"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="6bdb1-103">Atualizar deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="6bdb1-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="6bdb1-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="6bdb1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6bdb1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6bdb1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6bdb1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="6bdb1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bdb1-107">Atualize as propriedades de um objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="6bdb1-107">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6bdb1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6bdb1-108">Prerequisites</span></span>
<span data-ttu-id="6bdb1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6bdb1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6bdb1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6bdb1-111">Permission type</span></span>|<span data-ttu-id="6bdb1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6bdb1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bdb1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6bdb1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6bdb1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bdb1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6bdb1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6bdb1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bdb1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bdb1-116">Not supported.</span></span>|
|<span data-ttu-id="6bdb1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6bdb1-117">Application</span></span>|<span data-ttu-id="6bdb1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bdb1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bdb1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6bdb1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="6bdb1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6bdb1-120">Request headers</span></span>
|<span data-ttu-id="6bdb1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6bdb1-121">Header</span></span>|<span data-ttu-id="6bdb1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6bdb1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bdb1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6bdb1-123">Authorization</span></span>|<span data-ttu-id="6bdb1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bdb1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bdb1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6bdb1-125">Accept</span></span>|<span data-ttu-id="6bdb1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6bdb1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bdb1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6bdb1-127">Request body</span></span>
<span data-ttu-id="6bdb1-128">No corpo da solicitação, fornece uma representação JSON para o objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="6bdb1-128">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="6bdb1-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6bdb1-129">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="6bdb1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6bdb1-130">Property</span></span>|<span data-ttu-id="6bdb1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bdb1-131">Type</span></span>|<span data-ttu-id="6bdb1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bdb1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bdb1-133">id</span><span class="sxs-lookup"><span data-stu-id="6bdb1-133">id</span></span>|<span data-ttu-id="6bdb1-134">String</span><span class="sxs-lookup"><span data-stu-id="6bdb1-134">String</span></span>|<span data-ttu-id="6bdb1-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6bdb1-135">Not yet documented</span></span>|
|<span data-ttu-id="6bdb1-136">notificationContent</span><span class="sxs-lookup"><span data-stu-id="6bdb1-136">notificationContent</span></span>|<span data-ttu-id="6bdb1-137">Binária</span><span class="sxs-lookup"><span data-stu-id="6bdb1-137">Binary</span></span>|<span data-ttu-id="6bdb1-138">Texto de notificação que será enviado aos usuários em quarentena por essa política.</span><span class="sxs-lookup"><span data-stu-id="6bdb1-138">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="6bdb1-139">Isso é a matriz de bytes UTF8 codificado em HTML.</span><span class="sxs-lookup"><span data-stu-id="6bdb1-139">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="6bdb1-140">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="6bdb1-140">defaultAccessLevel</span></span>|[<span data-ttu-id="6bdb1-141">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="6bdb1-141">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="6bdb1-142">Estado de acesso padrão no Exchange.</span><span class="sxs-lookup"><span data-stu-id="6bdb1-142">Default access state in Exchange.</span></span> <span data-ttu-id="6bdb1-143">Esta regra se aplicam globalmente para toda a organização do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6bdb1-143">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="6bdb1-144">Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="6bdb1-144">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="6bdb1-145">accessRules</span><span class="sxs-lookup"><span data-stu-id="6bdb1-145">accessRules</span></span>|<span data-ttu-id="6bdb1-146">coleção [deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)</span><span class="sxs-lookup"><span data-stu-id="6bdb1-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="6bdb1-147">A lista de acesso de dispositivo regras no Exchange.</span><span class="sxs-lookup"><span data-stu-id="6bdb1-147">The list of device access rules in Exchange.</span></span> <span data-ttu-id="6bdb1-148">As regras de acesso se aplicam globalmente para toda a organização do Exchange</span><span class="sxs-lookup"><span data-stu-id="6bdb1-148">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="6bdb1-149">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="6bdb1-149">knownDeviceClasses</span></span>|<span data-ttu-id="6bdb1-150">coleção [deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)</span><span class="sxs-lookup"><span data-stu-id="6bdb1-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="6bdb1-151">A lista de classes de dispositivo conhecido para o Exchange</span><span class="sxs-lookup"><span data-stu-id="6bdb1-151">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="6bdb1-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bdb1-152">Response</span></span>
<span data-ttu-id="6bdb1-153">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6bdb1-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bdb1-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6bdb1-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="6bdb1-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bdb1-155">Request</span></span>
<span data-ttu-id="6bdb1-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6bdb1-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6bdb1-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bdb1-157">Response</span></span>
<span data-ttu-id="6bdb1-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6bdb1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




