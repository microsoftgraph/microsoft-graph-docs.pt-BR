---
title: Atualizar deviceManagementExchangeOnPremisesPolicy
description: Atualize as propriedades de um objeto deviceManagementExchangeOnPremisesPolicy.
ms.openlocfilehash: afc3df27d79b2cefab434126da8971f0fff5c8e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034338"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="b0922-103">Atualizar deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="b0922-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="b0922-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b0922-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0922-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b0922-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0922-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b0922-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0922-107">Atualize as propriedades de um objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="b0922-107">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b0922-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b0922-108">Prerequisites</span></span>
<span data-ttu-id="b0922-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0922-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0922-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0922-111">Permission type</span></span>|<span data-ttu-id="b0922-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b0922-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0922-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0922-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0922-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0922-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b0922-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0922-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0922-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0922-116">Not supported.</span></span>|
|<span data-ttu-id="b0922-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0922-117">Application</span></span>|<span data-ttu-id="b0922-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0922-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0922-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0922-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="b0922-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0922-120">Request headers</span></span>
|<span data-ttu-id="b0922-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0922-121">Header</span></span>|<span data-ttu-id="b0922-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b0922-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0922-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0922-123">Authorization</span></span>|<span data-ttu-id="b0922-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0922-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0922-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b0922-125">Accept</span></span>|<span data-ttu-id="b0922-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0922-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0922-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0922-127">Request body</span></span>
<span data-ttu-id="b0922-128">No corpo da solicitação, fornece uma representação JSON para o objeto [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="b0922-128">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="b0922-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0922-129">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="b0922-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0922-130">Property</span></span>|<span data-ttu-id="b0922-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0922-131">Type</span></span>|<span data-ttu-id="b0922-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0922-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0922-133">id</span><span class="sxs-lookup"><span data-stu-id="b0922-133">id</span></span>|<span data-ttu-id="b0922-134">String</span><span class="sxs-lookup"><span data-stu-id="b0922-134">String</span></span>|<span data-ttu-id="b0922-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b0922-135">Not yet documented</span></span>|
|<span data-ttu-id="b0922-136">notificationContent</span><span class="sxs-lookup"><span data-stu-id="b0922-136">notificationContent</span></span>|<span data-ttu-id="b0922-137">Binário</span><span class="sxs-lookup"><span data-stu-id="b0922-137">Binary</span></span>|<span data-ttu-id="b0922-138">Texto de notificação que será enviado aos usuários em quarentena por essa política.</span><span class="sxs-lookup"><span data-stu-id="b0922-138">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="b0922-139">Isso é a matriz de bytes UTF8 codificado em HTML.</span><span class="sxs-lookup"><span data-stu-id="b0922-139">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="b0922-140">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="b0922-140">defaultAccessLevel</span></span>|[<span data-ttu-id="b0922-141">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="b0922-141">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="b0922-142">Estado de acesso padrão no Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0922-142">Default access state in Exchange.</span></span> <span data-ttu-id="b0922-143">Esta regra se aplicam globalmente para toda a organização do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0922-143">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="b0922-144">Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="b0922-144">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="b0922-145">accessRules</span><span class="sxs-lookup"><span data-stu-id="b0922-145">accessRules</span></span>|<span data-ttu-id="b0922-146">coleção [deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)</span><span class="sxs-lookup"><span data-stu-id="b0922-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="b0922-147">A lista de acesso de dispositivo regras no Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0922-147">The list of device access rules in Exchange.</span></span> <span data-ttu-id="b0922-148">As regras de acesso se aplicam globalmente para toda a organização do Exchange</span><span class="sxs-lookup"><span data-stu-id="b0922-148">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="b0922-149">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="b0922-149">knownDeviceClasses</span></span>|<span data-ttu-id="b0922-150">coleção [deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)</span><span class="sxs-lookup"><span data-stu-id="b0922-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="b0922-151">A lista de classes de dispositivo conhecido para o Exchange</span><span class="sxs-lookup"><span data-stu-id="b0922-151">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="b0922-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0922-152">Response</span></span>
<span data-ttu-id="b0922-153">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0922-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0922-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0922-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="b0922-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0922-155">Request</span></span>
<span data-ttu-id="b0922-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0922-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b0922-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0922-157">Response</span></span>
<span data-ttu-id="b0922-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0922-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





