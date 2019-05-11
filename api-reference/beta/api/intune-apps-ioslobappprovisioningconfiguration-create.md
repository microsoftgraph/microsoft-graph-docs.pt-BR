---
title: Criar iosLobAppProvisioningConfiguration
description: Criar um novo objeto iosLobAppProvisioningConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a848b7bb83146019f4eebc37c95a99ce4beba17
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33937019"
---
# <a name="create-ioslobappprovisioningconfiguration"></a><span data-ttu-id="fb192-103">Criar iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="fb192-103">Create iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="fb192-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fb192-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb192-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fb192-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb192-106">Criar um novo objeto [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fb192-106">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb192-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fb192-107">Prerequisites</span></span>
<span data-ttu-id="fb192-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb192-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb192-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb192-110">Permission type</span></span>|<span data-ttu-id="fb192-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fb192-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb192-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb192-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fb192-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb192-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fb192-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb192-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb192-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb192-115">Not supported.</span></span>|
|<span data-ttu-id="fb192-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb192-116">Application</span></span>|<span data-ttu-id="fb192-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb192-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb192-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb192-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fb192-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb192-119">Request headers</span></span>
|<span data-ttu-id="fb192-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb192-120">Header</span></span>|<span data-ttu-id="fb192-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fb192-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb192-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb192-122">Authorization</span></span>|<span data-ttu-id="fb192-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb192-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb192-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fb192-124">Accept</span></span>|<span data-ttu-id="fb192-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fb192-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb192-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb192-126">Request body</span></span>
<span data-ttu-id="fb192-127">No corpo da solicitação, forneça uma representação JSON do objeto iosLobAppProvisioningConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fb192-127">In the request body, supply a JSON representation for the iosLobAppProvisioningConfiguration object.</span></span>

<span data-ttu-id="fb192-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosLobAppProvisioningConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fb192-128">The following table shows the properties that are required when you create the iosLobAppProvisioningConfiguration.</span></span>

|<span data-ttu-id="fb192-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb192-129">Property</span></span>|<span data-ttu-id="fb192-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb192-130">Type</span></span>|<span data-ttu-id="fb192-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb192-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb192-132">id</span><span class="sxs-lookup"><span data-stu-id="fb192-132">id</span></span>|<span data-ttu-id="fb192-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb192-133">String</span></span>|<span data-ttu-id="fb192-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fb192-134">Key of the entity.</span></span>|
|<span data-ttu-id="fb192-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fb192-135">expirationDateTime</span></span>|<span data-ttu-id="fb192-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb192-136">DateTimeOffset</span></span>|<span data-ttu-id="fb192-137">Data e hora de expiração do perfil opcional.</span><span class="sxs-lookup"><span data-stu-id="fb192-137">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="fb192-138">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="fb192-138">payloadFileName</span></span>|<span data-ttu-id="fb192-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb192-139">String</span></span>|<span data-ttu-id="fb192-140">Nome do arquivo de carga (\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="fb192-140">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="fb192-141">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="fb192-141">\*.xml).</span></span>|
|<span data-ttu-id="fb192-142">payload</span><span class="sxs-lookup"><span data-stu-id="fb192-142">payload</span></span>|<span data-ttu-id="fb192-143">Binária</span><span class="sxs-lookup"><span data-stu-id="fb192-143">Binary</span></span>|<span data-ttu-id="fb192-144">Carga.</span><span class="sxs-lookup"><span data-stu-id="fb192-144">Payload.</span></span> <span data-ttu-id="fb192-145">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="fb192-145">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="fb192-146">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fb192-146">roleScopeTagIds</span></span>|<span data-ttu-id="fb192-147">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb192-147">String collection</span></span>|<span data-ttu-id="fb192-148">Lista de marcas de escopo para esta entidade de configuração de provisionamento do aplicativo LOB iOS.</span><span class="sxs-lookup"><span data-stu-id="fb192-148">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="fb192-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb192-149">createdDateTime</span></span>|<span data-ttu-id="fb192-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb192-150">DateTimeOffset</span></span>|<span data-ttu-id="fb192-151">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="fb192-151">DateTime the object was created.</span></span>|
|<span data-ttu-id="fb192-152">description</span><span class="sxs-lookup"><span data-stu-id="fb192-152">description</span></span>|<span data-ttu-id="fb192-153">String</span><span class="sxs-lookup"><span data-stu-id="fb192-153">String</span></span>|<span data-ttu-id="fb192-154">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fb192-154">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="fb192-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb192-155">lastModifiedDateTime</span></span>|<span data-ttu-id="fb192-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb192-156">DateTimeOffset</span></span>|<span data-ttu-id="fb192-157">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="fb192-157">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="fb192-158">displayName</span><span class="sxs-lookup"><span data-stu-id="fb192-158">displayName</span></span>|<span data-ttu-id="fb192-159">String</span><span class="sxs-lookup"><span data-stu-id="fb192-159">String</span></span>|<span data-ttu-id="fb192-160">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fb192-160">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="fb192-161">versão</span><span class="sxs-lookup"><span data-stu-id="fb192-161">version</span></span>|<span data-ttu-id="fb192-162">Int32</span><span class="sxs-lookup"><span data-stu-id="fb192-162">Int32</span></span>|<span data-ttu-id="fb192-163">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fb192-163">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="fb192-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb192-164">Response</span></span>
<span data-ttu-id="fb192-165">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb192-165">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb192-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb192-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb192-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb192-167">Request</span></span>
<span data-ttu-id="fb192-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb192-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations
Content-type: application/json
Content-length: 375

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="fb192-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb192-169">Response</span></span>
<span data-ttu-id="fb192-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb192-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 547

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "id": "e2a23631-3631-e2a2-3136-a2e23136a2e2",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```




