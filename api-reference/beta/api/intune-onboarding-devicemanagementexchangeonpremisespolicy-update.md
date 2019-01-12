---
title: Atualizar deviceManagementExchangeOnPremisesPolicy
description: Atualize as propriedades de um objeto deviceManagementExchangeOnPremisesPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3698a258f6d0dd5c84f430c8690a7f58ffd88b0b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974662"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="acdbe-103">Atualizar deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="acdbe-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="acdbe-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="acdbe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="acdbe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="acdbe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="acdbe-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="acdbe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="acdbe-107">Atualize as propriedades de um objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="acdbe-107">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="acdbe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="acdbe-108">Prerequisites</span></span>
<span data-ttu-id="acdbe-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acdbe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acdbe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="acdbe-111">Permission type</span></span>|<span data-ttu-id="acdbe-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="acdbe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acdbe-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="acdbe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="acdbe-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acdbe-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="acdbe-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="acdbe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acdbe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="acdbe-116">Not supported.</span></span>|
|<span data-ttu-id="acdbe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="acdbe-117">Application</span></span>|<span data-ttu-id="acdbe-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="acdbe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acdbe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="acdbe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="acdbe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="acdbe-120">Request headers</span></span>
|<span data-ttu-id="acdbe-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="acdbe-121">Header</span></span>|<span data-ttu-id="acdbe-122">Valor</span><span class="sxs-lookup"><span data-stu-id="acdbe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acdbe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="acdbe-123">Authorization</span></span>|<span data-ttu-id="acdbe-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="acdbe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acdbe-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="acdbe-125">Accept</span></span>|<span data-ttu-id="acdbe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="acdbe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acdbe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="acdbe-127">Request body</span></span>
<span data-ttu-id="acdbe-128">No corpo da solicitação, fornece uma representação JSON para o objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="acdbe-128">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="acdbe-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span><span class="sxs-lookup"><span data-stu-id="acdbe-129">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="acdbe-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="acdbe-130">Property</span></span>|<span data-ttu-id="acdbe-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="acdbe-131">Type</span></span>|<span data-ttu-id="acdbe-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="acdbe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acdbe-133">id</span><span class="sxs-lookup"><span data-stu-id="acdbe-133">id</span></span>|<span data-ttu-id="acdbe-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="acdbe-134">String</span></span>|<span data-ttu-id="acdbe-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="acdbe-135">Not yet documented</span></span>|
|<span data-ttu-id="acdbe-136">notificationContent</span><span class="sxs-lookup"><span data-stu-id="acdbe-136">notificationContent</span></span>|<span data-ttu-id="acdbe-137">Binária</span><span class="sxs-lookup"><span data-stu-id="acdbe-137">Binary</span></span>|<span data-ttu-id="acdbe-138">Texto de notificação que será enviado aos usuários em quarentena por essa política.</span><span class="sxs-lookup"><span data-stu-id="acdbe-138">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="acdbe-139">Isso é a matriz de bytes UTF8 codificado em HTML.</span><span class="sxs-lookup"><span data-stu-id="acdbe-139">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="acdbe-140">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="acdbe-140">defaultAccessLevel</span></span>|[<span data-ttu-id="acdbe-141">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="acdbe-141">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="acdbe-142">Estado de acesso padrão no Exchange.</span><span class="sxs-lookup"><span data-stu-id="acdbe-142">Default access state in Exchange.</span></span> <span data-ttu-id="acdbe-143">Esta regra se aplicam globalmente para toda a organização do Exchange.</span><span class="sxs-lookup"><span data-stu-id="acdbe-143">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="acdbe-144">Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="acdbe-144">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="acdbe-145">accessRules</span><span class="sxs-lookup"><span data-stu-id="acdbe-145">accessRules</span></span>|<span data-ttu-id="acdbe-146">coleção [deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)</span><span class="sxs-lookup"><span data-stu-id="acdbe-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="acdbe-147">A lista de acesso de dispositivo regras no Exchange.</span><span class="sxs-lookup"><span data-stu-id="acdbe-147">The list of device access rules in Exchange.</span></span> <span data-ttu-id="acdbe-148">As regras de acesso se aplicam globalmente para toda a organização do Exchange</span><span class="sxs-lookup"><span data-stu-id="acdbe-148">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="acdbe-149">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="acdbe-149">knownDeviceClasses</span></span>|<span data-ttu-id="acdbe-150">coleção [deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)</span><span class="sxs-lookup"><span data-stu-id="acdbe-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="acdbe-151">A lista de classes de dispositivo conhecido para o Exchange</span><span class="sxs-lookup"><span data-stu-id="acdbe-151">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="acdbe-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="acdbe-152">Response</span></span>
<span data-ttu-id="acdbe-153">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="acdbe-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acdbe-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="acdbe-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="acdbe-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="acdbe-155">Request</span></span>
<span data-ttu-id="acdbe-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="acdbe-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
Content-type: application/json
Content-length: 586

{
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

### <a name="response"></a><span data-ttu-id="acdbe-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="acdbe-157">Response</span></span>
<span data-ttu-id="acdbe-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="acdbe-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





