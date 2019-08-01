---
title: Criar iosUpdateConfiguration
description: Cria um novo objeto iosUpdateConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c874e504db0a0486e758056dd2ce33699821e613
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997649"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="6c3ec-103">Criar iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c3ec-103">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="6c3ec-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c3ec-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c3ec-105">Cria um novo objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c3ec-105">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c3ec-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6c3ec-106">Prerequisites</span></span>
<span data-ttu-id="6c3ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c3ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c3ec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c3ec-109">Permission type</span></span>|<span data-ttu-id="6c3ec-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6c3ec-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c3ec-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c3ec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6c3ec-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c3ec-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c3ec-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c3ec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c3ec-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c3ec-114">Not supported.</span></span>|
|<span data-ttu-id="6c3ec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c3ec-115">Application</span></span>|<span data-ttu-id="6c3ec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c3ec-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c3ec-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c3ec-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6c3ec-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c3ec-118">Request headers</span></span>
|<span data-ttu-id="6c3ec-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c3ec-119">Header</span></span>|<span data-ttu-id="6c3ec-120">Valor</span><span class="sxs-lookup"><span data-stu-id="6c3ec-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c3ec-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c3ec-121">Authorization</span></span>|<span data-ttu-id="6c3ec-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c3ec-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c3ec-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6c3ec-123">Accept</span></span>|<span data-ttu-id="6c3ec-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6c3ec-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c3ec-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c3ec-125">Request body</span></span>
<span data-ttu-id="6c3ec-126">No corpo da solicitação, forneça uma representação JSON do objeto iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6c3ec-126">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="6c3ec-127">A tabela a seguir mostra as propriedades obrigatórias ao criar iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6c3ec-127">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="6c3ec-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c3ec-128">Property</span></span>|<span data-ttu-id="6c3ec-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c3ec-129">Type</span></span>|<span data-ttu-id="6c3ec-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c3ec-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c3ec-131">id</span><span class="sxs-lookup"><span data-stu-id="6c3ec-131">id</span></span>|<span data-ttu-id="6c3ec-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c3ec-132">String</span></span>|<span data-ttu-id="6c3ec-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6c3ec-133">Key of the entity.</span></span> <span data-ttu-id="6c3ec-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c3ec-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c3ec-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c3ec-135">lastModifiedDateTime</span></span>|<span data-ttu-id="6c3ec-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c3ec-136">DateTimeOffset</span></span>|<span data-ttu-id="6c3ec-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6c3ec-137">DateTime the object was last modified.</span></span> <span data-ttu-id="6c3ec-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c3ec-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c3ec-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c3ec-139">createdDateTime</span></span>|<span data-ttu-id="6c3ec-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c3ec-140">DateTimeOffset</span></span>|<span data-ttu-id="6c3ec-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6c3ec-141">DateTime the object was created.</span></span> <span data-ttu-id="6c3ec-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c3ec-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c3ec-143">descrição</span><span class="sxs-lookup"><span data-stu-id="6c3ec-143">description</span></span>|<span data-ttu-id="6c3ec-144">String</span><span class="sxs-lookup"><span data-stu-id="6c3ec-144">String</span></span>|<span data-ttu-id="6c3ec-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c3ec-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6c3ec-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c3ec-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c3ec-147">displayName</span><span class="sxs-lookup"><span data-stu-id="6c3ec-147">displayName</span></span>|<span data-ttu-id="6c3ec-148">String</span><span class="sxs-lookup"><span data-stu-id="6c3ec-148">String</span></span>|<span data-ttu-id="6c3ec-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c3ec-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6c3ec-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c3ec-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c3ec-151">versão</span><span class="sxs-lookup"><span data-stu-id="6c3ec-151">version</span></span>|<span data-ttu-id="6c3ec-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6c3ec-152">Int32</span></span>|<span data-ttu-id="6c3ec-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c3ec-153">Version of the device configuration.</span></span> <span data-ttu-id="6c3ec-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c3ec-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c3ec-155">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="6c3ec-155">activeHoursStart</span></span>|<span data-ttu-id="6c3ec-156">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6c3ec-156">TimeOfDay</span></span>|<span data-ttu-id="6c3ec-157">Início do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="6c3ec-157">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="6c3ec-158">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="6c3ec-158">activeHoursEnd</span></span>|<span data-ttu-id="6c3ec-159">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6c3ec-159">TimeOfDay</span></span>|<span data-ttu-id="6c3ec-160">Término do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="6c3ec-160">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="6c3ec-161">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="6c3ec-161">scheduledInstallDays</span></span>|<span data-ttu-id="6c3ec-162">coleção [DayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="6c3ec-162">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="6c3ec-163">Dias na semana para os quais o horário ativo está configurado.</span><span class="sxs-lookup"><span data-stu-id="6c3ec-163">Days in week for which active hours are configured.</span></span> <span data-ttu-id="6c3ec-164">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="6c3ec-164">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="6c3ec-165">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="6c3ec-165">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="6c3ec-166">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="6c3ec-166">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="6c3ec-167">Int32</span><span class="sxs-lookup"><span data-stu-id="6c3ec-167">Int32</span></span>|<span data-ttu-id="6c3ec-168">Deslocamento do horário UTC indicado em minutos</span><span class="sxs-lookup"><span data-stu-id="6c3ec-168">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="6c3ec-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c3ec-169">Response</span></span>
<span data-ttu-id="6c3ec-170">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c3ec-170">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c3ec-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c3ec-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c3ec-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c3ec-172">Request</span></span>
<span data-ttu-id="6c3ec-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c3ec-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6
}
```

### <a name="response"></a><span data-ttu-id="6c3ec-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c3ec-174">Response</span></span>
<span data-ttu-id="6c3ec-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c3ec-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 497

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6
}
```



