---
title: Criar windows10CustomConfiguration
description: Cria um novo objeto windows10CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f96011e85d155ca1b40249cc46359a82975a5d6e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016927"
---
# <a name="create-windows10customconfiguration"></a><span data-ttu-id="775ed-103">Criar windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="775ed-103">Create windows10CustomConfiguration</span></span>

> <span data-ttu-id="775ed-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="775ed-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="775ed-105">Cria um novo objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="775ed-105">Create a new [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="775ed-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="775ed-106">Prerequisites</span></span>
<span data-ttu-id="775ed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="775ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="775ed-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="775ed-109">Permission type</span></span>|<span data-ttu-id="775ed-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="775ed-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="775ed-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="775ed-111">Delegated (work or school account)</span></span>|<span data-ttu-id="775ed-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="775ed-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="775ed-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="775ed-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="775ed-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="775ed-114">Not supported.</span></span>|
|<span data-ttu-id="775ed-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="775ed-115">Application</span></span>|<span data-ttu-id="775ed-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="775ed-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="775ed-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="775ed-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="775ed-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="775ed-118">Request headers</span></span>
|<span data-ttu-id="775ed-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="775ed-119">Header</span></span>|<span data-ttu-id="775ed-120">Valor</span><span class="sxs-lookup"><span data-stu-id="775ed-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="775ed-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="775ed-121">Authorization</span></span>|<span data-ttu-id="775ed-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="775ed-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="775ed-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="775ed-123">Accept</span></span>|<span data-ttu-id="775ed-124">application/json</span><span class="sxs-lookup"><span data-stu-id="775ed-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="775ed-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="775ed-125">Request body</span></span>
<span data-ttu-id="775ed-126">No corpo da solicitação, forneça uma representação JSON do objeto windows10CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="775ed-126">In the request body, supply a JSON representation for the windows10CustomConfiguration object.</span></span>

<span data-ttu-id="775ed-127">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="775ed-127">The following table shows the properties that are required when you create the windows10CustomConfiguration.</span></span>

|<span data-ttu-id="775ed-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="775ed-128">Property</span></span>|<span data-ttu-id="775ed-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="775ed-129">Type</span></span>|<span data-ttu-id="775ed-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="775ed-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="775ed-131">id</span><span class="sxs-lookup"><span data-stu-id="775ed-131">id</span></span>|<span data-ttu-id="775ed-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="775ed-132">String</span></span>|<span data-ttu-id="775ed-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="775ed-133">Key of the entity.</span></span> <span data-ttu-id="775ed-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="775ed-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="775ed-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="775ed-135">lastModifiedDateTime</span></span>|<span data-ttu-id="775ed-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="775ed-136">DateTimeOffset</span></span>|<span data-ttu-id="775ed-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="775ed-137">DateTime the object was last modified.</span></span> <span data-ttu-id="775ed-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="775ed-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="775ed-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="775ed-139">createdDateTime</span></span>|<span data-ttu-id="775ed-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="775ed-140">DateTimeOffset</span></span>|<span data-ttu-id="775ed-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="775ed-141">DateTime the object was created.</span></span> <span data-ttu-id="775ed-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="775ed-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="775ed-143">descrição</span><span class="sxs-lookup"><span data-stu-id="775ed-143">description</span></span>|<span data-ttu-id="775ed-144">String</span><span class="sxs-lookup"><span data-stu-id="775ed-144">String</span></span>|<span data-ttu-id="775ed-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="775ed-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="775ed-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="775ed-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="775ed-147">displayName</span><span class="sxs-lookup"><span data-stu-id="775ed-147">displayName</span></span>|<span data-ttu-id="775ed-148">String</span><span class="sxs-lookup"><span data-stu-id="775ed-148">String</span></span>|<span data-ttu-id="775ed-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="775ed-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="775ed-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="775ed-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="775ed-151">versão</span><span class="sxs-lookup"><span data-stu-id="775ed-151">version</span></span>|<span data-ttu-id="775ed-152">Int32</span><span class="sxs-lookup"><span data-stu-id="775ed-152">Int32</span></span>|<span data-ttu-id="775ed-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="775ed-153">Version of the device configuration.</span></span> <span data-ttu-id="775ed-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="775ed-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="775ed-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="775ed-155">omaSettings</span></span>|<span data-ttu-id="775ed-156">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="775ed-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="775ed-157">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="775ed-157">OMA settings.</span></span> <span data-ttu-id="775ed-158">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="775ed-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="775ed-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="775ed-159">Response</span></span>
<span data-ttu-id="775ed-160">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="775ed-160">If successful, this method returns a `201 Created` response code and a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="775ed-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="775ed-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="775ed-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="775ed-162">Request</span></span>
<span data-ttu-id="775ed-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="775ed-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="775ed-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="775ed-164">Response</span></span>
<span data-ttu-id="775ed-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="775ed-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 576

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```



