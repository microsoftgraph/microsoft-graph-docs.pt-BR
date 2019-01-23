---
title: Atualizar deviceManagementScript
description: Atualize as propriedades de um objeto deviceManagementScript.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7cdf0364745f97beec777b6971ab096e43e916ff
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399007"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="0cda3-103">Atualizar deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="0cda3-103">Update deviceManagementScript</span></span>

> <span data-ttu-id="0cda3-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="0cda3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0cda3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0cda3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0cda3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="0cda3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cda3-107">Atualize as propriedades de um objeto [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="0cda3-107">Update the properties of a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cda3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0cda3-108">Prerequisites</span></span>
<span data-ttu-id="0cda3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0cda3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0cda3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0cda3-111">Permission type</span></span>|<span data-ttu-id="0cda3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0cda3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cda3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0cda3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0cda3-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cda3-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0cda3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0cda3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cda3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cda3-116">Not supported.</span></span>|
|<span data-ttu-id="0cda3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0cda3-117">Application</span></span>|<span data-ttu-id="0cda3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cda3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cda3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cda3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="0cda3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0cda3-120">Request headers</span></span>
|<span data-ttu-id="0cda3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0cda3-121">Header</span></span>|<span data-ttu-id="0cda3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0cda3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cda3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0cda3-123">Authorization</span></span>|<span data-ttu-id="0cda3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0cda3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cda3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0cda3-125">Accept</span></span>|<span data-ttu-id="0cda3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0cda3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cda3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0cda3-127">Request body</span></span>
<span data-ttu-id="0cda3-128">No corpo da solicitação, fornece uma representação JSON para o objeto [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="0cda3-128">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="0cda3-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="0cda3-129">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>

|<span data-ttu-id="0cda3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0cda3-130">Property</span></span>|<span data-ttu-id="0cda3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cda3-131">Type</span></span>|<span data-ttu-id="0cda3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cda3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cda3-133">id</span><span class="sxs-lookup"><span data-stu-id="0cda3-133">id</span></span>|<span data-ttu-id="0cda3-134">String</span><span class="sxs-lookup"><span data-stu-id="0cda3-134">String</span></span>|<span data-ttu-id="0cda3-135">Identificador exclusivo para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0cda3-135">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="0cda3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0cda3-136">displayName</span></span>|<span data-ttu-id="0cda3-137">String</span><span class="sxs-lookup"><span data-stu-id="0cda3-137">String</span></span>|<span data-ttu-id="0cda3-138">Nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0cda3-138">Name of the device management script.</span></span>|
|<span data-ttu-id="0cda3-139">description</span><span class="sxs-lookup"><span data-stu-id="0cda3-139">description</span></span>|<span data-ttu-id="0cda3-140">String</span><span class="sxs-lookup"><span data-stu-id="0cda3-140">String</span></span>|<span data-ttu-id="0cda3-141">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0cda3-141">Optional description for the device management script.</span></span>|
|<span data-ttu-id="0cda3-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="0cda3-142">runSchedule</span></span>|[<span data-ttu-id="0cda3-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="0cda3-143">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="0cda3-144">O intervalo de script a ser executado.</span><span class="sxs-lookup"><span data-stu-id="0cda3-144">The interval for script to run.</span></span> <span data-ttu-id="0cda3-145">Se não definido o script será executado uma vez</span><span class="sxs-lookup"><span data-stu-id="0cda3-145">If not defined the script will run once</span></span>|
|<span data-ttu-id="0cda3-146">scriptContent</span><span class="sxs-lookup"><span data-stu-id="0cda3-146">scriptContent</span></span>|<span data-ttu-id="0cda3-147">Binária</span><span class="sxs-lookup"><span data-stu-id="0cda3-147">Binary</span></span>|<span data-ttu-id="0cda3-148">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="0cda3-148">The script content.</span></span>|
|<span data-ttu-id="0cda3-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0cda3-149">createdDateTime</span></span>|<span data-ttu-id="0cda3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cda3-150">DateTimeOffset</span></span>|<span data-ttu-id="0cda3-151">A data e hora em que o script de gerenciamento do dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="0cda3-151">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="0cda3-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0cda3-152">lastModifiedDateTime</span></span>|<span data-ttu-id="0cda3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cda3-153">DateTimeOffset</span></span>|<span data-ttu-id="0cda3-154">A data e a hora que da última modificação o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0cda3-154">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="0cda3-155">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="0cda3-155">runAsAccount</span></span>|[<span data-ttu-id="0cda3-156">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="0cda3-156">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="0cda3-157">Indica o tipo de contexto de execução em que do script de gerenciamento de dispositivo é executado.</span><span class="sxs-lookup"><span data-stu-id="0cda3-157">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="0cda3-158">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="0cda3-158">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="0cda3-159">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="0cda3-159">enforceSignatureCheck</span></span>|<span data-ttu-id="0cda3-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cda3-160">Boolean</span></span>|<span data-ttu-id="0cda3-161">Indica se a assinatura de script precisa ser verificada.</span><span class="sxs-lookup"><span data-stu-id="0cda3-161">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="0cda3-162">fileName</span><span class="sxs-lookup"><span data-stu-id="0cda3-162">fileName</span></span>|<span data-ttu-id="0cda3-163">String</span><span class="sxs-lookup"><span data-stu-id="0cda3-163">String</span></span>|<span data-ttu-id="0cda3-164">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="0cda3-164">Script file name.</span></span>|
|<span data-ttu-id="0cda3-165">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0cda3-165">roleScopeTagIds</span></span>|<span data-ttu-id="0cda3-166">String collection</span><span class="sxs-lookup"><span data-stu-id="0cda3-166">String collection</span></span>|<span data-ttu-id="0cda3-167">Lista de IDs de marca de escopo para essa instância do PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="0cda3-167">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="0cda3-168">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="0cda3-168">runAs32Bit</span></span>|<span data-ttu-id="0cda3-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cda3-169">Boolean</span></span>|<span data-ttu-id="0cda3-170">Um valor que indica se o script do PowerShell deve ser executado como de 32 bits</span><span class="sxs-lookup"><span data-stu-id="0cda3-170">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="0cda3-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cda3-171">Response</span></span>
<span data-ttu-id="0cda3-172">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cda3-172">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cda3-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0cda3-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cda3-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0cda3-174">Request</span></span>
<span data-ttu-id="0cda3-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0cda3-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
Content-type: application/json
Content-length: 443

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true
}
```

### <a name="response"></a><span data-ttu-id="0cda3-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cda3-176">Response</span></span>
<span data-ttu-id="0cda3-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0cda3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 615

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
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true
}
```




