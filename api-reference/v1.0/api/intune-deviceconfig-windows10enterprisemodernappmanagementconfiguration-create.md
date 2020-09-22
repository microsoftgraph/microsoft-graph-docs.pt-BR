---
title: Criar windows10EnterpriseModernAppManagementConfiguration
description: Criar um novo objeto windows10EnterpriseModernAppManagementConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 56eae02a90b6cdebf0f4ff8f1ff35e8b41e0c6ed
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041740"
---
# <a name="create-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="75322-103">Criar windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="75322-103">Create windows10EnterpriseModernAppManagementConfiguration</span></span>

<span data-ttu-id="75322-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75322-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75322-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75322-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75322-106">Criar um novo objeto [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="75322-106">Create a new [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75322-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="75322-107">Prerequisites</span></span>
<span data-ttu-id="75322-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75322-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75322-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75322-110">Permission type</span></span>|<span data-ttu-id="75322-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="75322-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75322-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75322-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75322-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75322-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75322-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75322-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75322-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75322-115">Not supported.</span></span>|
|<span data-ttu-id="75322-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75322-116">Application</span></span>|<span data-ttu-id="75322-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75322-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75322-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75322-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="75322-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75322-119">Request headers</span></span>
|<span data-ttu-id="75322-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="75322-120">Header</span></span>|<span data-ttu-id="75322-121">Valor</span><span class="sxs-lookup"><span data-stu-id="75322-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75322-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="75322-122">Authorization</span></span>|<span data-ttu-id="75322-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75322-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75322-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="75322-124">Accept</span></span>|<span data-ttu-id="75322-125">application/json</span><span class="sxs-lookup"><span data-stu-id="75322-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75322-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75322-126">Request body</span></span>
<span data-ttu-id="75322-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10EnterpriseModernAppManagementConfiguration.</span><span class="sxs-lookup"><span data-stu-id="75322-127">In the request body, supply a JSON representation for the windows10EnterpriseModernAppManagementConfiguration object.</span></span>

<span data-ttu-id="75322-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10EnterpriseModernAppManagementConfiguration.</span><span class="sxs-lookup"><span data-stu-id="75322-128">The following table shows the properties that are required when you create the windows10EnterpriseModernAppManagementConfiguration.</span></span>

|<span data-ttu-id="75322-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75322-129">Property</span></span>|<span data-ttu-id="75322-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="75322-130">Type</span></span>|<span data-ttu-id="75322-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="75322-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75322-132">id</span><span class="sxs-lookup"><span data-stu-id="75322-132">id</span></span>|<span data-ttu-id="75322-133">String</span><span class="sxs-lookup"><span data-stu-id="75322-133">String</span></span>|<span data-ttu-id="75322-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="75322-134">Key of the entity.</span></span> <span data-ttu-id="75322-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75322-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75322-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75322-136">lastModifiedDateTime</span></span>|<span data-ttu-id="75322-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75322-137">DateTimeOffset</span></span>|<span data-ttu-id="75322-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="75322-138">DateTime the object was last modified.</span></span> <span data-ttu-id="75322-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75322-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75322-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75322-140">createdDateTime</span></span>|<span data-ttu-id="75322-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75322-141">DateTimeOffset</span></span>|<span data-ttu-id="75322-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="75322-142">DateTime the object was created.</span></span> <span data-ttu-id="75322-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75322-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75322-144">description</span><span class="sxs-lookup"><span data-stu-id="75322-144">description</span></span>|<span data-ttu-id="75322-145">String</span><span class="sxs-lookup"><span data-stu-id="75322-145">String</span></span>|<span data-ttu-id="75322-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75322-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="75322-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75322-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75322-148">displayName</span><span class="sxs-lookup"><span data-stu-id="75322-148">displayName</span></span>|<span data-ttu-id="75322-149">String</span><span class="sxs-lookup"><span data-stu-id="75322-149">String</span></span>|<span data-ttu-id="75322-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75322-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="75322-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75322-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75322-152">versão</span><span class="sxs-lookup"><span data-stu-id="75322-152">version</span></span>|<span data-ttu-id="75322-153">Int32</span><span class="sxs-lookup"><span data-stu-id="75322-153">Int32</span></span>|<span data-ttu-id="75322-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75322-154">Version of the device configuration.</span></span> <span data-ttu-id="75322-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75322-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75322-156">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="75322-156">uninstallBuiltInApps</span></span>|<span data-ttu-id="75322-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="75322-157">Boolean</span></span>|<span data-ttu-id="75322-158">Indica se deseja ou não desinstalar uma lista fixa de aplicativos internos do Windows.</span><span class="sxs-lookup"><span data-stu-id="75322-158">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="75322-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="75322-159">Response</span></span>
<span data-ttu-id="75322-160">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75322-160">If successful, this method returns a `201 Created` response code and a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75322-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75322-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="75322-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75322-162">Request</span></span>
<span data-ttu-id="75322-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75322-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="75322-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="75322-164">Response</span></span>
<span data-ttu-id="75322-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75322-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









