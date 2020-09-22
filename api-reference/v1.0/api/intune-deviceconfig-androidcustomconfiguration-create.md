---
title: Criar androidCustomConfiguration
description: Criar um novo objeto androidCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: abf611369cdd2a1cc429cb18f0c3d5deae2678df
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083775"
---
# <a name="create-androidcustomconfiguration"></a><span data-ttu-id="777bb-103">Criar androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="777bb-103">Create androidCustomConfiguration</span></span>

<span data-ttu-id="777bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="777bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="777bb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="777bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="777bb-106">Criar um novo objeto [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="777bb-106">Create a new [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="777bb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="777bb-107">Prerequisites</span></span>
<span data-ttu-id="777bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="777bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="777bb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="777bb-110">Permission type</span></span>|<span data-ttu-id="777bb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="777bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="777bb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="777bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="777bb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="777bb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="777bb-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="777bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="777bb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="777bb-115">Not supported.</span></span>|
|<span data-ttu-id="777bb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="777bb-116">Application</span></span>|<span data-ttu-id="777bb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="777bb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="777bb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="777bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="777bb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="777bb-119">Request headers</span></span>
|<span data-ttu-id="777bb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="777bb-120">Header</span></span>|<span data-ttu-id="777bb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="777bb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="777bb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="777bb-122">Authorization</span></span>|<span data-ttu-id="777bb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="777bb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="777bb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="777bb-124">Accept</span></span>|<span data-ttu-id="777bb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="777bb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="777bb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="777bb-126">Request body</span></span>
<span data-ttu-id="777bb-127">No corpo da solicitação, forneça uma representação JSON do objeto androidCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="777bb-127">In the request body, supply a JSON representation for the androidCustomConfiguration object.</span></span>

<span data-ttu-id="777bb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="777bb-128">The following table shows the properties that are required when you create the androidCustomConfiguration.</span></span>

|<span data-ttu-id="777bb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="777bb-129">Property</span></span>|<span data-ttu-id="777bb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="777bb-130">Type</span></span>|<span data-ttu-id="777bb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="777bb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="777bb-132">id</span><span class="sxs-lookup"><span data-stu-id="777bb-132">id</span></span>|<span data-ttu-id="777bb-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="777bb-133">String</span></span>|<span data-ttu-id="777bb-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="777bb-134">Key of the entity.</span></span> <span data-ttu-id="777bb-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="777bb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="777bb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="777bb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="777bb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="777bb-137">DateTimeOffset</span></span>|<span data-ttu-id="777bb-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="777bb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="777bb-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="777bb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="777bb-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="777bb-140">createdDateTime</span></span>|<span data-ttu-id="777bb-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="777bb-141">DateTimeOffset</span></span>|<span data-ttu-id="777bb-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="777bb-142">DateTime the object was created.</span></span> <span data-ttu-id="777bb-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="777bb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="777bb-144">description</span><span class="sxs-lookup"><span data-stu-id="777bb-144">description</span></span>|<span data-ttu-id="777bb-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="777bb-145">String</span></span>|<span data-ttu-id="777bb-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="777bb-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="777bb-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="777bb-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="777bb-148">displayName</span><span class="sxs-lookup"><span data-stu-id="777bb-148">displayName</span></span>|<span data-ttu-id="777bb-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="777bb-149">String</span></span>|<span data-ttu-id="777bb-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="777bb-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="777bb-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="777bb-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="777bb-152">versão</span><span class="sxs-lookup"><span data-stu-id="777bb-152">version</span></span>|<span data-ttu-id="777bb-153">Int32</span><span class="sxs-lookup"><span data-stu-id="777bb-153">Int32</span></span>|<span data-ttu-id="777bb-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="777bb-154">Version of the device configuration.</span></span> <span data-ttu-id="777bb-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="777bb-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="777bb-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="777bb-156">omaSettings</span></span>|<span data-ttu-id="777bb-157">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="777bb-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="777bb-158">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="777bb-158">OMA settings.</span></span> <span data-ttu-id="777bb-159">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="777bb-159">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="777bb-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="777bb-160">Response</span></span>
<span data-ttu-id="777bb-161">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="777bb-161">If successful, this method returns a `201 Created` response code and a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="777bb-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="777bb-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="777bb-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="777bb-163">Request</span></span>
<span data-ttu-id="777bb-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="777bb-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 402

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="777bb-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="777bb-165">Response</span></span>
<span data-ttu-id="777bb-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="777bb-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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









