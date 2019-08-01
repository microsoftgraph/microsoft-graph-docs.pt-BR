---
title: Criar androidWorkProfileCustomConfiguration
description: Criar um novo objeto androidWorkProfileCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c70226b876054c5a01edbae3c9d3fee000bfd422
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997831"
---
# <a name="create-androidworkprofilecustomconfiguration"></a><span data-ttu-id="1979c-103">Criar androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="1979c-103">Create androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="1979c-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1979c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1979c-105">Criar um novo objeto [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1979c-105">Create a new [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1979c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1979c-106">Prerequisites</span></span>
<span data-ttu-id="1979c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1979c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1979c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1979c-109">Permission type</span></span>|<span data-ttu-id="1979c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1979c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1979c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1979c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1979c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1979c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1979c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1979c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1979c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1979c-114">Not supported.</span></span>|
|<span data-ttu-id="1979c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1979c-115">Application</span></span>|<span data-ttu-id="1979c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1979c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1979c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1979c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1979c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1979c-118">Request headers</span></span>
|<span data-ttu-id="1979c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1979c-119">Header</span></span>|<span data-ttu-id="1979c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="1979c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1979c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1979c-121">Authorization</span></span>|<span data-ttu-id="1979c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1979c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1979c-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1979c-123">Accept</span></span>|<span data-ttu-id="1979c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1979c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1979c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1979c-125">Request body</span></span>
<span data-ttu-id="1979c-126">No corpo da solicitação, forneça uma representação JSON do objeto androidWorkProfileCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1979c-126">In the request body, supply a JSON representation for the androidWorkProfileCustomConfiguration object.</span></span>

<span data-ttu-id="1979c-127">A tabela a seguir mostra as propriedades que são necessárias ao criar androidWorkProfileCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1979c-127">The following table shows the properties that are required when you create the androidWorkProfileCustomConfiguration.</span></span>

|<span data-ttu-id="1979c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1979c-128">Property</span></span>|<span data-ttu-id="1979c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="1979c-129">Type</span></span>|<span data-ttu-id="1979c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="1979c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1979c-131">id</span><span class="sxs-lookup"><span data-stu-id="1979c-131">id</span></span>|<span data-ttu-id="1979c-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1979c-132">String</span></span>|<span data-ttu-id="1979c-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1979c-133">Key of the entity.</span></span> <span data-ttu-id="1979c-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1979c-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1979c-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1979c-135">lastModifiedDateTime</span></span>|<span data-ttu-id="1979c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1979c-136">DateTimeOffset</span></span>|<span data-ttu-id="1979c-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1979c-137">DateTime the object was last modified.</span></span> <span data-ttu-id="1979c-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1979c-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1979c-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1979c-139">createdDateTime</span></span>|<span data-ttu-id="1979c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1979c-140">DateTimeOffset</span></span>|<span data-ttu-id="1979c-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1979c-141">DateTime the object was created.</span></span> <span data-ttu-id="1979c-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1979c-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1979c-143">descrição</span><span class="sxs-lookup"><span data-stu-id="1979c-143">description</span></span>|<span data-ttu-id="1979c-144">String</span><span class="sxs-lookup"><span data-stu-id="1979c-144">String</span></span>|<span data-ttu-id="1979c-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1979c-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1979c-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1979c-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1979c-147">displayName</span><span class="sxs-lookup"><span data-stu-id="1979c-147">displayName</span></span>|<span data-ttu-id="1979c-148">String</span><span class="sxs-lookup"><span data-stu-id="1979c-148">String</span></span>|<span data-ttu-id="1979c-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1979c-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1979c-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1979c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1979c-151">versão</span><span class="sxs-lookup"><span data-stu-id="1979c-151">version</span></span>|<span data-ttu-id="1979c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="1979c-152">Int32</span></span>|<span data-ttu-id="1979c-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1979c-153">Version of the device configuration.</span></span> <span data-ttu-id="1979c-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1979c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1979c-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="1979c-155">omaSettings</span></span>|<span data-ttu-id="1979c-156">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1979c-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="1979c-157">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="1979c-157">OMA settings.</span></span> <span data-ttu-id="1979c-158">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="1979c-158">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="1979c-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="1979c-159">Response</span></span>
<span data-ttu-id="1979c-160">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1979c-160">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1979c-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1979c-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="1979c-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1979c-162">Request</span></span>
<span data-ttu-id="1979c-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1979c-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 413

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="1979c-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="1979c-164">Response</span></span>
<span data-ttu-id="1979c-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1979c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 585

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
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



