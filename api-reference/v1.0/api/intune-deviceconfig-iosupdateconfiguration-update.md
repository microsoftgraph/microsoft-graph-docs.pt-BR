---
title: Atualizar iosUpdateConfiguration
description: Atualizar as propriedades de um objeto iosUpdateConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dfc9be70f26b9d4ed58dfca1274a828237ebb473
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982222"
---
# <a name="update-iosupdateconfiguration"></a><span data-ttu-id="8c997-103">Atualizar iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="8c997-103">Update iosUpdateConfiguration</span></span>

> <span data-ttu-id="8c997-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8c997-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c997-105">Atualizar as propriedades de um objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8c997-105">Update the properties of a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c997-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8c997-106">Prerequisites</span></span>
<span data-ttu-id="8c997-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c997-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c997-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c997-109">Permission type</span></span>|<span data-ttu-id="8c997-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8c997-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c997-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c997-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8c997-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c997-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8c997-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c997-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c997-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c997-114">Not supported.</span></span>|
|<span data-ttu-id="8c997-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c997-115">Application</span></span>|<span data-ttu-id="8c997-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c997-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c997-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c997-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8c997-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c997-118">Request headers</span></span>
|<span data-ttu-id="8c997-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8c997-119">Header</span></span>|<span data-ttu-id="8c997-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8c997-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c997-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c997-121">Authorization</span></span>|<span data-ttu-id="8c997-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c997-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c997-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8c997-123">Accept</span></span>|<span data-ttu-id="8c997-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8c997-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c997-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c997-125">Request body</span></span>
<span data-ttu-id="8c997-126">No corpo da solicitação, forneça uma representação JSON do objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8c997-126">In the request body, supply a JSON representation for the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

<span data-ttu-id="8c997-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8c997-127">The following table shows the properties that are required when you create the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span></span>

|<span data-ttu-id="8c997-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c997-128">Property</span></span>|<span data-ttu-id="8c997-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c997-129">Type</span></span>|<span data-ttu-id="8c997-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c997-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c997-131">id</span><span class="sxs-lookup"><span data-stu-id="8c997-131">id</span></span>|<span data-ttu-id="8c997-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c997-132">String</span></span>|<span data-ttu-id="8c997-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8c997-133">Key of the entity.</span></span> <span data-ttu-id="8c997-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c997-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c997-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c997-135">lastModifiedDateTime</span></span>|<span data-ttu-id="8c997-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c997-136">DateTimeOffset</span></span>|<span data-ttu-id="8c997-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8c997-137">DateTime the object was last modified.</span></span> <span data-ttu-id="8c997-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c997-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c997-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c997-139">createdDateTime</span></span>|<span data-ttu-id="8c997-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c997-140">DateTimeOffset</span></span>|<span data-ttu-id="8c997-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8c997-141">DateTime the object was created.</span></span> <span data-ttu-id="8c997-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c997-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c997-143">description</span><span class="sxs-lookup"><span data-stu-id="8c997-143">description</span></span>|<span data-ttu-id="8c997-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c997-144">String</span></span>|<span data-ttu-id="8c997-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8c997-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8c997-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c997-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c997-147">displayName</span><span class="sxs-lookup"><span data-stu-id="8c997-147">displayName</span></span>|<span data-ttu-id="8c997-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c997-148">String</span></span>|<span data-ttu-id="8c997-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8c997-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8c997-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c997-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c997-151">version</span><span class="sxs-lookup"><span data-stu-id="8c997-151">version</span></span>|<span data-ttu-id="8c997-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8c997-152">Int32</span></span>|<span data-ttu-id="8c997-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8c997-153">Version of the device configuration.</span></span> <span data-ttu-id="8c997-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c997-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8c997-155">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="8c997-155">activeHoursStart</span></span>|<span data-ttu-id="8c997-156">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8c997-156">TimeOfDay</span></span>|<span data-ttu-id="8c997-157">Início do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="8c997-157">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="8c997-158">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="8c997-158">activeHoursEnd</span></span>|<span data-ttu-id="8c997-159">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8c997-159">TimeOfDay</span></span>|<span data-ttu-id="8c997-160">Término do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="8c997-160">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="8c997-161">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="8c997-161">scheduledInstallDays</span></span>|<span data-ttu-id="8c997-162">coleção [dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="8c997-162">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="8c997-163">Dias na semana para os quais o horário ativo está configurado.</span><span class="sxs-lookup"><span data-stu-id="8c997-163">Days in week for which active hours are configured.</span></span> <span data-ttu-id="8c997-164">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="8c997-164">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="8c997-165">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="8c997-165">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="8c997-166">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="8c997-166">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="8c997-167">Int32</span><span class="sxs-lookup"><span data-stu-id="8c997-167">Int32</span></span>|<span data-ttu-id="8c997-168">Deslocamento do horário UTC indicado em minutos</span><span class="sxs-lookup"><span data-stu-id="8c997-168">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="8c997-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c997-169">Response</span></span>
<span data-ttu-id="8c997-170">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c997-170">If successful, this method returns a `200 OK` response code and an updated [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c997-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c997-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c997-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c997-172">Request</span></span>
<span data-ttu-id="8c997-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c997-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="8c997-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c997-174">Response</span></span>
<span data-ttu-id="8c997-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c997-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



