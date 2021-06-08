---
title: Criar windows10EnterpriseModernAppManagementConfiguration
description: Criar um novo objeto windows10EnterpriseModernAppManagementConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5d24727218a61ba03302857e9a3b079a0e40d876
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760542"
---
# <a name="create-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="27738-103">Criar windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="27738-103">Create windows10EnterpriseModernAppManagementConfiguration</span></span>

<span data-ttu-id="27738-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27738-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27738-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="27738-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27738-106">Criar um novo objeto [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="27738-106">Create a new [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27738-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27738-107">Prerequisites</span></span>
<span data-ttu-id="27738-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27738-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27738-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27738-110">Permission type</span></span>|<span data-ttu-id="27738-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27738-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27738-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27738-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27738-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27738-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="27738-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27738-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27738-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27738-115">Not supported.</span></span>|
|<span data-ttu-id="27738-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27738-116">Application</span></span>|<span data-ttu-id="27738-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27738-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="27738-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27738-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="27738-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27738-119">Request headers</span></span>
|<span data-ttu-id="27738-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27738-120">Header</span></span>|<span data-ttu-id="27738-121">Valor</span><span class="sxs-lookup"><span data-stu-id="27738-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27738-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="27738-122">Authorization</span></span>|<span data-ttu-id="27738-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27738-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27738-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="27738-124">Accept</span></span>|<span data-ttu-id="27738-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27738-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27738-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27738-126">Request body</span></span>
<span data-ttu-id="27738-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10EnterpriseModernAppManagementConfiguration.</span><span class="sxs-lookup"><span data-stu-id="27738-127">In the request body, supply a JSON representation for the windows10EnterpriseModernAppManagementConfiguration object.</span></span>

<span data-ttu-id="27738-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10EnterpriseModernAppManagementConfiguration.</span><span class="sxs-lookup"><span data-stu-id="27738-128">The following table shows the properties that are required when you create the windows10EnterpriseModernAppManagementConfiguration.</span></span>

|<span data-ttu-id="27738-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27738-129">Property</span></span>|<span data-ttu-id="27738-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="27738-130">Type</span></span>|<span data-ttu-id="27738-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="27738-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27738-132">id</span><span class="sxs-lookup"><span data-stu-id="27738-132">id</span></span>|<span data-ttu-id="27738-133">String</span><span class="sxs-lookup"><span data-stu-id="27738-133">String</span></span>|<span data-ttu-id="27738-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="27738-134">Key of the entity.</span></span> <span data-ttu-id="27738-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27738-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27738-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27738-136">lastModifiedDateTime</span></span>|<span data-ttu-id="27738-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27738-137">DateTimeOffset</span></span>|<span data-ttu-id="27738-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="27738-138">DateTime the object was last modified.</span></span> <span data-ttu-id="27738-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27738-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27738-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27738-140">createdDateTime</span></span>|<span data-ttu-id="27738-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27738-141">DateTimeOffset</span></span>|<span data-ttu-id="27738-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="27738-142">DateTime the object was created.</span></span> <span data-ttu-id="27738-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27738-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27738-144">description</span><span class="sxs-lookup"><span data-stu-id="27738-144">description</span></span>|<span data-ttu-id="27738-145">String</span><span class="sxs-lookup"><span data-stu-id="27738-145">String</span></span>|<span data-ttu-id="27738-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27738-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="27738-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27738-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27738-148">displayName</span><span class="sxs-lookup"><span data-stu-id="27738-148">displayName</span></span>|<span data-ttu-id="27738-149">String</span><span class="sxs-lookup"><span data-stu-id="27738-149">String</span></span>|<span data-ttu-id="27738-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27738-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="27738-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27738-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27738-152">versão</span><span class="sxs-lookup"><span data-stu-id="27738-152">version</span></span>|<span data-ttu-id="27738-153">Int32</span><span class="sxs-lookup"><span data-stu-id="27738-153">Int32</span></span>|<span data-ttu-id="27738-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27738-154">Version of the device configuration.</span></span> <span data-ttu-id="27738-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27738-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27738-156">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="27738-156">uninstallBuiltInApps</span></span>|<span data-ttu-id="27738-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="27738-157">Boolean</span></span>|<span data-ttu-id="27738-158">Indica se deseja ou não desinstalar uma lista fixa de aplicativos internos do Windows.</span><span class="sxs-lookup"><span data-stu-id="27738-158">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="27738-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="27738-159">Response</span></span>
<span data-ttu-id="27738-160">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27738-160">If successful, this method returns a `201 Created` response code and a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27738-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27738-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="27738-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27738-162">Request</span></span>
<span data-ttu-id="27738-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27738-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="27738-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="27738-164">Response</span></span>
<span data-ttu-id="27738-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27738-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




