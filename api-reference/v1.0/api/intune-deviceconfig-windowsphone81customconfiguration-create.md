---
title: Criar windowsPhone81CustomConfiguration
description: Cria um novo objeto windowsPhone81CustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 767ee7303de1ba67ab9d4fc512f5e9933dad6c27
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43399294"
---
# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="9303f-103">Criar windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="9303f-103">Create windowsPhone81CustomConfiguration</span></span>

<span data-ttu-id="9303f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9303f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9303f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9303f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9303f-106">Cria um novo objeto [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9303f-106">Create a new [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9303f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9303f-107">Prerequisites</span></span>
<span data-ttu-id="9303f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9303f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9303f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9303f-110">Permission type</span></span>|<span data-ttu-id="9303f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9303f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9303f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9303f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9303f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9303f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9303f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9303f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9303f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9303f-115">Not supported.</span></span>|
|<span data-ttu-id="9303f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9303f-116">Application</span></span>|<span data-ttu-id="9303f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9303f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9303f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9303f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9303f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9303f-119">Request headers</span></span>
|<span data-ttu-id="9303f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9303f-120">Header</span></span>|<span data-ttu-id="9303f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9303f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9303f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9303f-122">Authorization</span></span>|<span data-ttu-id="9303f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9303f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9303f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9303f-124">Accept</span></span>|<span data-ttu-id="9303f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9303f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9303f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9303f-126">Request body</span></span>
<span data-ttu-id="9303f-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9303f-127">In the request body, supply a JSON representation for the windowsPhone81CustomConfiguration object.</span></span>

<span data-ttu-id="9303f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9303f-128">The following table shows the properties that are required when you create the windowsPhone81CustomConfiguration.</span></span>

|<span data-ttu-id="9303f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9303f-129">Property</span></span>|<span data-ttu-id="9303f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9303f-130">Type</span></span>|<span data-ttu-id="9303f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9303f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9303f-132">id</span><span class="sxs-lookup"><span data-stu-id="9303f-132">id</span></span>|<span data-ttu-id="9303f-133">String</span><span class="sxs-lookup"><span data-stu-id="9303f-133">String</span></span>|<span data-ttu-id="9303f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9303f-134">Key of the entity.</span></span> <span data-ttu-id="9303f-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9303f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9303f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9303f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9303f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9303f-137">DateTimeOffset</span></span>|<span data-ttu-id="9303f-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9303f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9303f-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9303f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9303f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9303f-140">createdDateTime</span></span>|<span data-ttu-id="9303f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9303f-141">DateTimeOffset</span></span>|<span data-ttu-id="9303f-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9303f-142">DateTime the object was created.</span></span> <span data-ttu-id="9303f-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9303f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9303f-144">description</span><span class="sxs-lookup"><span data-stu-id="9303f-144">description</span></span>|<span data-ttu-id="9303f-145">String</span><span class="sxs-lookup"><span data-stu-id="9303f-145">String</span></span>|<span data-ttu-id="9303f-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9303f-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9303f-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9303f-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9303f-148">displayName</span><span class="sxs-lookup"><span data-stu-id="9303f-148">displayName</span></span>|<span data-ttu-id="9303f-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9303f-149">String</span></span>|<span data-ttu-id="9303f-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9303f-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9303f-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9303f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9303f-152">versão</span><span class="sxs-lookup"><span data-stu-id="9303f-152">version</span></span>|<span data-ttu-id="9303f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="9303f-153">Int32</span></span>|<span data-ttu-id="9303f-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9303f-154">Version of the device configuration.</span></span> <span data-ttu-id="9303f-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9303f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9303f-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="9303f-156">omaSettings</span></span>|<span data-ttu-id="9303f-157">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9303f-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="9303f-158">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="9303f-158">OMA settings.</span></span> <span data-ttu-id="9303f-159">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="9303f-159">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="9303f-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="9303f-160">Response</span></span>
<span data-ttu-id="9303f-161">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9303f-161">If successful, this method returns a `201 Created` response code and a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9303f-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9303f-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="9303f-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9303f-163">Request</span></span>
<span data-ttu-id="9303f-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9303f-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 409

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="9303f-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="9303f-165">Response</span></span>
<span data-ttu-id="9303f-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9303f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 581

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
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






