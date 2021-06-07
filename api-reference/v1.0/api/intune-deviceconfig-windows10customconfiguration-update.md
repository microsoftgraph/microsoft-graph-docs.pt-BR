---
title: Atualizar windows10CustomConfiguration
description: Atualizar as propriedades de um objeto windows10CustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 16126906fa4a4127298de60760bf76c0be982310
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758292"
---
# <a name="update-windows10customconfiguration"></a><span data-ttu-id="c7d51-103">Atualizar windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="c7d51-103">Update windows10CustomConfiguration</span></span>

<span data-ttu-id="c7d51-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7d51-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7d51-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7d51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7d51-106">Atualizar as propriedades de um objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7d51-106">Update the properties of a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7d51-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c7d51-107">Prerequisites</span></span>
<span data-ttu-id="c7d51-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7d51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7d51-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7d51-110">Permission type</span></span>|<span data-ttu-id="c7d51-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7d51-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7d51-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7d51-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c7d51-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7d51-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c7d51-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7d51-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7d51-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7d51-115">Not supported.</span></span>|
|<span data-ttu-id="c7d51-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7d51-116">Application</span></span>|<span data-ttu-id="c7d51-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7d51-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7d51-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7d51-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c7d51-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7d51-119">Request headers</span></span>
|<span data-ttu-id="c7d51-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7d51-120">Header</span></span>|<span data-ttu-id="c7d51-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c7d51-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7d51-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7d51-122">Authorization</span></span>|<span data-ttu-id="c7d51-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7d51-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7d51-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c7d51-124">Accept</span></span>|<span data-ttu-id="c7d51-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c7d51-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7d51-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7d51-126">Request body</span></span>
<span data-ttu-id="c7d51-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7d51-127">In the request body, supply a JSON representation for the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

<span data-ttu-id="c7d51-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7d51-128">The following table shows the properties that are required when you create the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span></span>

|<span data-ttu-id="c7d51-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7d51-129">Property</span></span>|<span data-ttu-id="c7d51-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7d51-130">Type</span></span>|<span data-ttu-id="c7d51-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7d51-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7d51-132">id</span><span class="sxs-lookup"><span data-stu-id="c7d51-132">id</span></span>|<span data-ttu-id="c7d51-133">String</span><span class="sxs-lookup"><span data-stu-id="c7d51-133">String</span></span>|<span data-ttu-id="c7d51-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c7d51-134">Key of the entity.</span></span> <span data-ttu-id="c7d51-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7d51-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7d51-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7d51-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c7d51-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7d51-137">DateTimeOffset</span></span>|<span data-ttu-id="c7d51-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c7d51-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c7d51-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7d51-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7d51-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7d51-140">createdDateTime</span></span>|<span data-ttu-id="c7d51-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7d51-141">DateTimeOffset</span></span>|<span data-ttu-id="c7d51-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c7d51-142">DateTime the object was created.</span></span> <span data-ttu-id="c7d51-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7d51-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7d51-144">description</span><span class="sxs-lookup"><span data-stu-id="c7d51-144">description</span></span>|<span data-ttu-id="c7d51-145">String</span><span class="sxs-lookup"><span data-stu-id="c7d51-145">String</span></span>|<span data-ttu-id="c7d51-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c7d51-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c7d51-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7d51-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7d51-148">displayName</span><span class="sxs-lookup"><span data-stu-id="c7d51-148">displayName</span></span>|<span data-ttu-id="c7d51-149">String</span><span class="sxs-lookup"><span data-stu-id="c7d51-149">String</span></span>|<span data-ttu-id="c7d51-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c7d51-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c7d51-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7d51-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7d51-152">versão</span><span class="sxs-lookup"><span data-stu-id="c7d51-152">version</span></span>|<span data-ttu-id="c7d51-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c7d51-153">Int32</span></span>|<span data-ttu-id="c7d51-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c7d51-154">Version of the device configuration.</span></span> <span data-ttu-id="c7d51-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7d51-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7d51-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="c7d51-156">omaSettings</span></span>|<span data-ttu-id="c7d51-157">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c7d51-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="c7d51-158">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="c7d51-158">OMA settings.</span></span> <span data-ttu-id="c7d51-159">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="c7d51-159">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c7d51-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7d51-160">Response</span></span>
<span data-ttu-id="c7d51-161">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7d51-161">If successful, this method returns a `200 OK` response code and an updated [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7d51-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7d51-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7d51-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7d51-163">Request</span></span>
<span data-ttu-id="c7d51-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7d51-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 378

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="c7d51-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7d51-165">Response</span></span>
<span data-ttu-id="c7d51-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7d51-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 550

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
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value"
    }
  ]
}
```




