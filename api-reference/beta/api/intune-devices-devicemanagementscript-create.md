---
title: Criar deviceManagementScript
description: Crie um novo objeto de deviceManagementScript.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be0ffb8b912b25684ba0ed3dc383a995fb872f3b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409269"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="fdabe-103">Criar deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="fdabe-103">Create deviceManagementScript</span></span>

> <span data-ttu-id="fdabe-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="fdabe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fdabe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fdabe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fdabe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="fdabe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdabe-107">Crie um novo objeto de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="fdabe-107">Create a new [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdabe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fdabe-108">Prerequisites</span></span>
<span data-ttu-id="fdabe-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fdabe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fdabe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdabe-111">Permission type</span></span>|<span data-ttu-id="fdabe-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fdabe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdabe-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdabe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fdabe-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdabe-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fdabe-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdabe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdabe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdabe-116">Not supported.</span></span>|
|<span data-ttu-id="fdabe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdabe-117">Application</span></span>|<span data-ttu-id="fdabe-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdabe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdabe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdabe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="fdabe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdabe-120">Request headers</span></span>
|<span data-ttu-id="fdabe-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fdabe-121">Header</span></span>|<span data-ttu-id="fdabe-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fdabe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdabe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdabe-123">Authorization</span></span>|<span data-ttu-id="fdabe-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdabe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdabe-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fdabe-125">Accept</span></span>|<span data-ttu-id="fdabe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fdabe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdabe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdabe-127">Request body</span></span>
<span data-ttu-id="fdabe-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementScript.</span><span class="sxs-lookup"><span data-stu-id="fdabe-128">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="fdabe-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o deviceManagementScript.</span><span class="sxs-lookup"><span data-stu-id="fdabe-129">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="fdabe-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fdabe-130">Property</span></span>|<span data-ttu-id="fdabe-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdabe-131">Type</span></span>|<span data-ttu-id="fdabe-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdabe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdabe-133">id</span><span class="sxs-lookup"><span data-stu-id="fdabe-133">id</span></span>|<span data-ttu-id="fdabe-134">String</span><span class="sxs-lookup"><span data-stu-id="fdabe-134">String</span></span>|<span data-ttu-id="fdabe-135">Identificador exclusivo para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fdabe-135">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="fdabe-136">displayName</span><span class="sxs-lookup"><span data-stu-id="fdabe-136">displayName</span></span>|<span data-ttu-id="fdabe-137">String</span><span class="sxs-lookup"><span data-stu-id="fdabe-137">String</span></span>|<span data-ttu-id="fdabe-138">Nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fdabe-138">Name of the device management script.</span></span>|
|<span data-ttu-id="fdabe-139">description</span><span class="sxs-lookup"><span data-stu-id="fdabe-139">description</span></span>|<span data-ttu-id="fdabe-140">String</span><span class="sxs-lookup"><span data-stu-id="fdabe-140">String</span></span>|<span data-ttu-id="fdabe-141">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fdabe-141">Optional description for the device management script.</span></span>|
|<span data-ttu-id="fdabe-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="fdabe-142">runSchedule</span></span>|[<span data-ttu-id="fdabe-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="fdabe-143">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="fdabe-144">O intervalo de script a ser executado.</span><span class="sxs-lookup"><span data-stu-id="fdabe-144">The interval for script to run.</span></span> <span data-ttu-id="fdabe-145">Se não definido o script será executado uma vez</span><span class="sxs-lookup"><span data-stu-id="fdabe-145">If not defined the script will run once</span></span>|
|<span data-ttu-id="fdabe-146">scriptContent</span><span class="sxs-lookup"><span data-stu-id="fdabe-146">scriptContent</span></span>|<span data-ttu-id="fdabe-147">Binária</span><span class="sxs-lookup"><span data-stu-id="fdabe-147">Binary</span></span>|<span data-ttu-id="fdabe-148">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="fdabe-148">The script content.</span></span>|
|<span data-ttu-id="fdabe-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fdabe-149">createdDateTime</span></span>|<span data-ttu-id="fdabe-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdabe-150">DateTimeOffset</span></span>|<span data-ttu-id="fdabe-151">A data e hora em que o script de gerenciamento do dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="fdabe-151">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="fdabe-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fdabe-152">lastModifiedDateTime</span></span>|<span data-ttu-id="fdabe-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdabe-153">DateTimeOffset</span></span>|<span data-ttu-id="fdabe-154">A data e a hora que da última modificação o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fdabe-154">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="fdabe-155">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="fdabe-155">runAsAccount</span></span>|[<span data-ttu-id="fdabe-156">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="fdabe-156">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="fdabe-157">Indica o tipo de contexto de execução em que do script de gerenciamento de dispositivo é executado.</span><span class="sxs-lookup"><span data-stu-id="fdabe-157">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="fdabe-158">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="fdabe-158">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="fdabe-159">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="fdabe-159">enforceSignatureCheck</span></span>|<span data-ttu-id="fdabe-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdabe-160">Boolean</span></span>|<span data-ttu-id="fdabe-161">Indica se a assinatura de script precisa ser verificada.</span><span class="sxs-lookup"><span data-stu-id="fdabe-161">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="fdabe-162">fileName</span><span class="sxs-lookup"><span data-stu-id="fdabe-162">fileName</span></span>|<span data-ttu-id="fdabe-163">String</span><span class="sxs-lookup"><span data-stu-id="fdabe-163">String</span></span>|<span data-ttu-id="fdabe-164">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="fdabe-164">Script file name.</span></span>|
|<span data-ttu-id="fdabe-165">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fdabe-165">roleScopeTagIds</span></span>|<span data-ttu-id="fdabe-166">String collection</span><span class="sxs-lookup"><span data-stu-id="fdabe-166">String collection</span></span>|<span data-ttu-id="fdabe-167">Lista de IDs de marca de escopo para essa instância do PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="fdabe-167">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="fdabe-168">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="fdabe-168">runAs32Bit</span></span>|<span data-ttu-id="fdabe-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdabe-169">Boolean</span></span>|<span data-ttu-id="fdabe-170">Um valor que indica se o script do PowerShell deve ser executado como de 32 bits</span><span class="sxs-lookup"><span data-stu-id="fdabe-170">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="fdabe-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdabe-171">Response</span></span>
<span data-ttu-id="fdabe-172">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdabe-172">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdabe-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdabe-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdabe-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdabe-174">Request</span></span>
<span data-ttu-id="fdabe-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdabe-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
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

### <a name="response"></a><span data-ttu-id="fdabe-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdabe-176">Response</span></span>
<span data-ttu-id="fdabe-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fdabe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




