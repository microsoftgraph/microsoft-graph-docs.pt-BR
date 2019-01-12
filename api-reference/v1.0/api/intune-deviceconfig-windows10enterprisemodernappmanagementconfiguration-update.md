---
title: Atualizar windows10EnterpriseModernAppManagementConfiguration
description: Atualizar as propriedades de um objeto windows10EnterpriseModernAppManagementConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 60d9388db921bb201edf88f3d608143b6b741de5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974971"
---
# <a name="update-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="af968-103">Atualizar windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="af968-103">Update windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="af968-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="af968-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af968-105">Atualizar as propriedades de um objeto [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af968-105">Update the properties of a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af968-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="af968-106">Prerequisites</span></span>
<span data-ttu-id="af968-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af968-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af968-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af968-109">Permission type</span></span>|<span data-ttu-id="af968-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="af968-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af968-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af968-111">Delegated (work or school account)</span></span>|<span data-ttu-id="af968-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af968-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="af968-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af968-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af968-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af968-114">Not supported.</span></span>|
|<span data-ttu-id="af968-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af968-115">Application</span></span>|<span data-ttu-id="af968-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af968-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af968-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af968-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="af968-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af968-118">Request headers</span></span>
|<span data-ttu-id="af968-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="af968-119">Header</span></span>|<span data-ttu-id="af968-120">Valor</span><span class="sxs-lookup"><span data-stu-id="af968-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af968-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="af968-121">Authorization</span></span>|<span data-ttu-id="af968-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af968-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af968-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="af968-123">Accept</span></span>|<span data-ttu-id="af968-124">application/json</span><span class="sxs-lookup"><span data-stu-id="af968-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af968-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af968-125">Request body</span></span>
<span data-ttu-id="af968-126">No corpo da solicitação, forneça uma representação JSON do objeto [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af968-126">In the request body, supply a JSON representation for the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

<span data-ttu-id="af968-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af968-127">The following table shows the properties that are required when you create the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span></span>

|<span data-ttu-id="af968-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af968-128">Property</span></span>|<span data-ttu-id="af968-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="af968-129">Type</span></span>|<span data-ttu-id="af968-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="af968-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af968-131">id</span><span class="sxs-lookup"><span data-stu-id="af968-131">id</span></span>|<span data-ttu-id="af968-132">String</span><span class="sxs-lookup"><span data-stu-id="af968-132">String</span></span>|<span data-ttu-id="af968-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="af968-133">Key of the entity.</span></span> <span data-ttu-id="af968-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af968-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af968-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af968-135">lastModifiedDateTime</span></span>|<span data-ttu-id="af968-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af968-136">DateTimeOffset</span></span>|<span data-ttu-id="af968-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="af968-137">DateTime the object was last modified.</span></span> <span data-ttu-id="af968-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af968-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af968-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af968-139">createdDateTime</span></span>|<span data-ttu-id="af968-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af968-140">DateTimeOffset</span></span>|<span data-ttu-id="af968-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="af968-141">DateTime the object was created.</span></span> <span data-ttu-id="af968-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af968-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af968-143">description</span><span class="sxs-lookup"><span data-stu-id="af968-143">description</span></span>|<span data-ttu-id="af968-144">String</span><span class="sxs-lookup"><span data-stu-id="af968-144">String</span></span>|<span data-ttu-id="af968-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="af968-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="af968-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af968-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af968-147">displayName</span><span class="sxs-lookup"><span data-stu-id="af968-147">displayName</span></span>|<span data-ttu-id="af968-148">String</span><span class="sxs-lookup"><span data-stu-id="af968-148">String</span></span>|<span data-ttu-id="af968-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="af968-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="af968-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af968-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af968-151">version</span><span class="sxs-lookup"><span data-stu-id="af968-151">version</span></span>|<span data-ttu-id="af968-152">Int32</span><span class="sxs-lookup"><span data-stu-id="af968-152">Int32</span></span>|<span data-ttu-id="af968-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="af968-153">Version of the device configuration.</span></span> <span data-ttu-id="af968-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af968-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af968-155">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="af968-155">uninstallBuiltInApps</span></span>|<span data-ttu-id="af968-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="af968-156">Boolean</span></span>|<span data-ttu-id="af968-157">Indica se deseja ou não desinstalar uma lista fixa de aplicativos internos do Windows.</span><span class="sxs-lookup"><span data-stu-id="af968-157">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="af968-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="af968-158">Response</span></span>
<span data-ttu-id="af968-159">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af968-159">If successful, this method returns a `200 OK` response code and an updated [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af968-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af968-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="af968-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af968-161">Request</span></span>
<span data-ttu-id="af968-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af968-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```

### <a name="response"></a><span data-ttu-id="af968-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="af968-163">Response</span></span>
<span data-ttu-id="af968-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af968-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "id": "d6577687-7687-d657-8776-57d6877657d6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```



