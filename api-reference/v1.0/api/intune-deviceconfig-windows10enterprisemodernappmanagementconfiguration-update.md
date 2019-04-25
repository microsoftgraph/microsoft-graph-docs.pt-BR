---
title: Atualizar windows10EnterpriseModernAppManagementConfiguration
description: Atualizar as propriedades de um objeto windows10EnterpriseModernAppManagementConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 11f9a96fc301e9175f9b9bce9302ac0da0562c5c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581489"
---
# <a name="update-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="de029-103">Atualizar windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="de029-103">Update windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="de029-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="de029-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de029-105">Atualizar as propriedades de um objeto [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="de029-105">Update the properties of a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de029-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="de029-106">Prerequisites</span></span>
<span data-ttu-id="de029-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de029-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de029-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de029-109">Permission type</span></span>|<span data-ttu-id="de029-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="de029-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de029-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de029-111">Delegated (work or school account)</span></span>|<span data-ttu-id="de029-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de029-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de029-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de029-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de029-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de029-114">Not supported.</span></span>|
|<span data-ttu-id="de029-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de029-115">Application</span></span>|<span data-ttu-id="de029-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de029-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de029-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de029-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="de029-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de029-118">Request headers</span></span>
|<span data-ttu-id="de029-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="de029-119">Header</span></span>|<span data-ttu-id="de029-120">Valor</span><span class="sxs-lookup"><span data-stu-id="de029-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de029-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="de029-121">Authorization</span></span>|<span data-ttu-id="de029-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de029-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de029-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="de029-123">Accept</span></span>|<span data-ttu-id="de029-124">application/json</span><span class="sxs-lookup"><span data-stu-id="de029-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de029-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de029-125">Request body</span></span>
<span data-ttu-id="de029-126">No corpo da solicitação, forneça uma representação JSON do objeto [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="de029-126">In the request body, supply a JSON representation for the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

<span data-ttu-id="de029-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="de029-127">The following table shows the properties that are required when you create the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span></span>

|<span data-ttu-id="de029-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de029-128">Property</span></span>|<span data-ttu-id="de029-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="de029-129">Type</span></span>|<span data-ttu-id="de029-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="de029-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de029-131">id</span><span class="sxs-lookup"><span data-stu-id="de029-131">id</span></span>|<span data-ttu-id="de029-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de029-132">String</span></span>|<span data-ttu-id="de029-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="de029-133">Key of the entity.</span></span> <span data-ttu-id="de029-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de029-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de029-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de029-135">lastModifiedDateTime</span></span>|<span data-ttu-id="de029-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de029-136">DateTimeOffset</span></span>|<span data-ttu-id="de029-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="de029-137">DateTime the object was last modified.</span></span> <span data-ttu-id="de029-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de029-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de029-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de029-139">createdDateTime</span></span>|<span data-ttu-id="de029-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de029-140">DateTimeOffset</span></span>|<span data-ttu-id="de029-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="de029-141">DateTime the object was created.</span></span> <span data-ttu-id="de029-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de029-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de029-143">description</span><span class="sxs-lookup"><span data-stu-id="de029-143">description</span></span>|<span data-ttu-id="de029-144">String</span><span class="sxs-lookup"><span data-stu-id="de029-144">String</span></span>|<span data-ttu-id="de029-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de029-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="de029-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de029-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de029-147">displayName</span><span class="sxs-lookup"><span data-stu-id="de029-147">displayName</span></span>|<span data-ttu-id="de029-148">String</span><span class="sxs-lookup"><span data-stu-id="de029-148">String</span></span>|<span data-ttu-id="de029-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de029-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="de029-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de029-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de029-151">versão</span><span class="sxs-lookup"><span data-stu-id="de029-151">version</span></span>|<span data-ttu-id="de029-152">Int32</span><span class="sxs-lookup"><span data-stu-id="de029-152">Int32</span></span>|<span data-ttu-id="de029-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de029-153">Version of the device configuration.</span></span> <span data-ttu-id="de029-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de029-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de029-155">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="de029-155">uninstallBuiltInApps</span></span>|<span data-ttu-id="de029-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="de029-156">Boolean</span></span>|<span data-ttu-id="de029-157">Indica se deseja ou não desinstalar uma lista fixa de aplicativos internos do Windows.</span><span class="sxs-lookup"><span data-stu-id="de029-157">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="de029-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="de029-158">Response</span></span>
<span data-ttu-id="de029-159">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de029-159">If successful, this method returns a `200 OK` response code and an updated [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de029-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de029-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="de029-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de029-161">Request</span></span>
<span data-ttu-id="de029-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de029-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="de029-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="de029-163">Response</span></span>
<span data-ttu-id="de029-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de029-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



