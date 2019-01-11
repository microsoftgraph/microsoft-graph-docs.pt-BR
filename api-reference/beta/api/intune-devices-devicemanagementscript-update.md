---
title: Atualizar deviceManagementScript
description: Atualize as propriedades de um objeto deviceManagementScript.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aaca6501f0a1c0fd206583af4e976b9afe9ac2cc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869290"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="53d9a-103">Atualizar deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="53d9a-103">Update deviceManagementScript</span></span>

> <span data-ttu-id="53d9a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="53d9a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53d9a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="53d9a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53d9a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="53d9a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53d9a-107">Atualize as propriedades de um objeto [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="53d9a-107">Update the properties of a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="53d9a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="53d9a-108">Prerequisites</span></span>
<span data-ttu-id="53d9a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53d9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53d9a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53d9a-111">Permission type</span></span>|<span data-ttu-id="53d9a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="53d9a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53d9a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53d9a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53d9a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53d9a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="53d9a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53d9a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53d9a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53d9a-116">Not supported.</span></span>|
|<span data-ttu-id="53d9a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53d9a-117">Application</span></span>|<span data-ttu-id="53d9a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53d9a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53d9a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53d9a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="53d9a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53d9a-120">Request headers</span></span>
|<span data-ttu-id="53d9a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="53d9a-121">Header</span></span>|<span data-ttu-id="53d9a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="53d9a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53d9a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="53d9a-123">Authorization</span></span>|<span data-ttu-id="53d9a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53d9a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53d9a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="53d9a-125">Accept</span></span>|<span data-ttu-id="53d9a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53d9a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53d9a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53d9a-127">Request body</span></span>
<span data-ttu-id="53d9a-128">No corpo da solicitação, fornece uma representação JSON para o objeto [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="53d9a-128">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="53d9a-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="53d9a-129">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>

|<span data-ttu-id="53d9a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53d9a-130">Property</span></span>|<span data-ttu-id="53d9a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="53d9a-131">Type</span></span>|<span data-ttu-id="53d9a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="53d9a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53d9a-133">id</span><span class="sxs-lookup"><span data-stu-id="53d9a-133">id</span></span>|<span data-ttu-id="53d9a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53d9a-134">String</span></span>|<span data-ttu-id="53d9a-135">Identificador exclusivo para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="53d9a-135">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="53d9a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="53d9a-136">displayName</span></span>|<span data-ttu-id="53d9a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53d9a-137">String</span></span>|<span data-ttu-id="53d9a-138">Nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="53d9a-138">Name of the device management script.</span></span>|
|<span data-ttu-id="53d9a-139">description</span><span class="sxs-lookup"><span data-stu-id="53d9a-139">description</span></span>|<span data-ttu-id="53d9a-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53d9a-140">String</span></span>|<span data-ttu-id="53d9a-141">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="53d9a-141">Optional description for the device management script.</span></span>|
|<span data-ttu-id="53d9a-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="53d9a-142">runSchedule</span></span>|[<span data-ttu-id="53d9a-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="53d9a-143">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="53d9a-144">O intervalo de script a ser executado.</span><span class="sxs-lookup"><span data-stu-id="53d9a-144">The interval for script to run.</span></span> <span data-ttu-id="53d9a-145">Se não definido o script será executado uma vez</span><span class="sxs-lookup"><span data-stu-id="53d9a-145">If not defined the script will run once</span></span>|
|<span data-ttu-id="53d9a-146">scriptContent</span><span class="sxs-lookup"><span data-stu-id="53d9a-146">scriptContent</span></span>|<span data-ttu-id="53d9a-147">Binária</span><span class="sxs-lookup"><span data-stu-id="53d9a-147">Binary</span></span>|<span data-ttu-id="53d9a-148">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="53d9a-148">The script content.</span></span>|
|<span data-ttu-id="53d9a-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53d9a-149">createdDateTime</span></span>|<span data-ttu-id="53d9a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53d9a-150">DateTimeOffset</span></span>|<span data-ttu-id="53d9a-151">A data e hora em que o script de gerenciamento do dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="53d9a-151">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="53d9a-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53d9a-152">lastModifiedDateTime</span></span>|<span data-ttu-id="53d9a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53d9a-153">DateTimeOffset</span></span>|<span data-ttu-id="53d9a-154">A data e a hora que da última modificação o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="53d9a-154">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="53d9a-155">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="53d9a-155">runAsAccount</span></span>|[<span data-ttu-id="53d9a-156">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="53d9a-156">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="53d9a-157">Indica o tipo de contexto de execução em que do script de gerenciamento de dispositivo é executado.</span><span class="sxs-lookup"><span data-stu-id="53d9a-157">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="53d9a-158">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="53d9a-158">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="53d9a-159">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="53d9a-159">enforceSignatureCheck</span></span>|<span data-ttu-id="53d9a-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="53d9a-160">Boolean</span></span>|<span data-ttu-id="53d9a-161">Indica se a assinatura de script precisa ser verificada.</span><span class="sxs-lookup"><span data-stu-id="53d9a-161">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="53d9a-162">fileName</span><span class="sxs-lookup"><span data-stu-id="53d9a-162">fileName</span></span>|<span data-ttu-id="53d9a-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53d9a-163">String</span></span>|<span data-ttu-id="53d9a-164">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="53d9a-164">Script file name.</span></span>|



## <a name="response"></a><span data-ttu-id="53d9a-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="53d9a-165">Response</span></span>
<span data-ttu-id="53d9a-166">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53d9a-166">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53d9a-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53d9a-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="53d9a-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53d9a-168">Request</span></span>
<span data-ttu-id="53d9a-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53d9a-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
Content-type: application/json
Content-length: 361

{
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value"
}
```

### <a name="response"></a><span data-ttu-id="53d9a-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="53d9a-170">Response</span></span>
<span data-ttu-id="53d9a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53d9a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 530

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "59ea4525-4525-59ea-2545-ea592545ea59",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value"
}
```





