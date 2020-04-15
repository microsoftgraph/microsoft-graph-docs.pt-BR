---
title: Criar iosUpdateConfiguration
description: Cria um novo objeto iosUpdateConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 790a4a7307b3da4d73c89cdfbfe9149ffb8f8e70
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467469"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="3208f-103">Criar iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="3208f-103">Create iosUpdateConfiguration</span></span>

<span data-ttu-id="3208f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3208f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3208f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3208f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3208f-106">Cria um novo objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3208f-106">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3208f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3208f-107">Prerequisites</span></span>
<span data-ttu-id="3208f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3208f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3208f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3208f-110">Permission type</span></span>|<span data-ttu-id="3208f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3208f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3208f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3208f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3208f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3208f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3208f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3208f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3208f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3208f-115">Not supported.</span></span>|
|<span data-ttu-id="3208f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3208f-116">Application</span></span>|<span data-ttu-id="3208f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3208f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3208f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3208f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3208f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3208f-119">Request headers</span></span>
|<span data-ttu-id="3208f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3208f-120">Header</span></span>|<span data-ttu-id="3208f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3208f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3208f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3208f-122">Authorization</span></span>|<span data-ttu-id="3208f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3208f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3208f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3208f-124">Accept</span></span>|<span data-ttu-id="3208f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3208f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3208f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3208f-126">Request body</span></span>
<span data-ttu-id="3208f-127">No corpo da solicitação, forneça uma representação JSON do objeto iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3208f-127">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="3208f-128">A tabela a seguir mostra as propriedades obrigatórias ao criar iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3208f-128">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="3208f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3208f-129">Property</span></span>|<span data-ttu-id="3208f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3208f-130">Type</span></span>|<span data-ttu-id="3208f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3208f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3208f-132">id</span><span class="sxs-lookup"><span data-stu-id="3208f-132">id</span></span>|<span data-ttu-id="3208f-133">String</span><span class="sxs-lookup"><span data-stu-id="3208f-133">String</span></span>|<span data-ttu-id="3208f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3208f-134">Key of the entity.</span></span> <span data-ttu-id="3208f-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3208f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3208f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3208f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3208f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3208f-137">DateTimeOffset</span></span>|<span data-ttu-id="3208f-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3208f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3208f-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3208f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3208f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3208f-140">createdDateTime</span></span>|<span data-ttu-id="3208f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3208f-141">DateTimeOffset</span></span>|<span data-ttu-id="3208f-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3208f-142">DateTime the object was created.</span></span> <span data-ttu-id="3208f-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3208f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3208f-144">description</span><span class="sxs-lookup"><span data-stu-id="3208f-144">description</span></span>|<span data-ttu-id="3208f-145">String</span><span class="sxs-lookup"><span data-stu-id="3208f-145">String</span></span>|<span data-ttu-id="3208f-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3208f-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3208f-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3208f-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3208f-148">displayName</span><span class="sxs-lookup"><span data-stu-id="3208f-148">displayName</span></span>|<span data-ttu-id="3208f-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3208f-149">String</span></span>|<span data-ttu-id="3208f-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3208f-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3208f-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3208f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3208f-152">versão</span><span class="sxs-lookup"><span data-stu-id="3208f-152">version</span></span>|<span data-ttu-id="3208f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3208f-153">Int32</span></span>|<span data-ttu-id="3208f-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3208f-154">Version of the device configuration.</span></span> <span data-ttu-id="3208f-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3208f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3208f-156">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="3208f-156">activeHoursStart</span></span>|<span data-ttu-id="3208f-157">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="3208f-157">TimeOfDay</span></span>|<span data-ttu-id="3208f-158">Início do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="3208f-158">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="3208f-159">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="3208f-159">activeHoursEnd</span></span>|<span data-ttu-id="3208f-160">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="3208f-160">TimeOfDay</span></span>|<span data-ttu-id="3208f-161">Término do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="3208f-161">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="3208f-162">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="3208f-162">scheduledInstallDays</span></span>|<span data-ttu-id="3208f-163">coleção [DayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="3208f-163">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="3208f-164">Dias na semana para os quais o horário ativo está configurado.</span><span class="sxs-lookup"><span data-stu-id="3208f-164">Days in week for which active hours are configured.</span></span> <span data-ttu-id="3208f-165">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="3208f-165">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="3208f-166">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="3208f-166">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="3208f-167">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="3208f-167">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="3208f-168">Int32</span><span class="sxs-lookup"><span data-stu-id="3208f-168">Int32</span></span>|<span data-ttu-id="3208f-169">Deslocamento do horário UTC indicado em minutos</span><span class="sxs-lookup"><span data-stu-id="3208f-169">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="3208f-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="3208f-170">Response</span></span>
<span data-ttu-id="3208f-171">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3208f-171">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3208f-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3208f-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="3208f-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3208f-173">Request</span></span>
<span data-ttu-id="3208f-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3208f-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3208f-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="3208f-175">Response</span></span>
<span data-ttu-id="3208f-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3208f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






