---
title: Criar iosLobAppProvisioningConfiguration
description: Criar um novo objeto iosLobAppProvisioningConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 178f4f30c944749d9913dffe5a2ee583e1de97d7
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199417"
---
# <a name="create-ioslobappprovisioningconfiguration"></a><span data-ttu-id="ecf8c-103">Criar iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="ecf8c-103">Create iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="ecf8c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ecf8c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ecf8c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ecf8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecf8c-106">Criar um novo objeto [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ecf8c-106">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecf8c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ecf8c-107">Prerequisites</span></span>
<span data-ttu-id="ecf8c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecf8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecf8c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ecf8c-110">Permission type</span></span>|<span data-ttu-id="ecf8c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ecf8c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecf8c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ecf8c-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ecf8c-113">&nbsp;&nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="ecf8c-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="ecf8c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecf8c-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="ecf8c-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="ecf8c-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="ecf8c-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecf8c-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ecf8c-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ecf8c-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecf8c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecf8c-118">Not supported.</span></span>|
|<span data-ttu-id="ecf8c-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ecf8c-119">Application</span></span>||
| <span data-ttu-id="ecf8c-120">&nbsp;&nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="ecf8c-120">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="ecf8c-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecf8c-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="ecf8c-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="ecf8c-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="ecf8c-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecf8c-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecf8c-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ecf8c-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ecf8c-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ecf8c-125">Request headers</span></span>
|<span data-ttu-id="ecf8c-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ecf8c-126">Header</span></span>|<span data-ttu-id="ecf8c-127">Valor</span><span class="sxs-lookup"><span data-stu-id="ecf8c-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecf8c-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="ecf8c-128">Authorization</span></span>|<span data-ttu-id="ecf8c-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecf8c-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecf8c-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ecf8c-130">Accept</span></span>|<span data-ttu-id="ecf8c-131">application/json</span><span class="sxs-lookup"><span data-stu-id="ecf8c-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecf8c-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ecf8c-132">Request body</span></span>
<span data-ttu-id="ecf8c-133">No corpo da solicitação, forneça uma representação JSON do objeto iosLobAppProvisioningConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ecf8c-133">In the request body, supply a JSON representation for the iosLobAppProvisioningConfiguration object.</span></span>

<span data-ttu-id="ecf8c-134">A tabela a seguir mostra as propriedades que são necessárias ao criar iosLobAppProvisioningConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ecf8c-134">The following table shows the properties that are required when you create the iosLobAppProvisioningConfiguration.</span></span>

|<span data-ttu-id="ecf8c-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ecf8c-135">Property</span></span>|<span data-ttu-id="ecf8c-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="ecf8c-136">Type</span></span>|<span data-ttu-id="ecf8c-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecf8c-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecf8c-138">id</span><span class="sxs-lookup"><span data-stu-id="ecf8c-138">id</span></span>|<span data-ttu-id="ecf8c-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecf8c-139">String</span></span>|<span data-ttu-id="ecf8c-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ecf8c-140">Key of the entity.</span></span>|
|<span data-ttu-id="ecf8c-141">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ecf8c-141">expirationDateTime</span></span>|<span data-ttu-id="ecf8c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecf8c-142">DateTimeOffset</span></span>|<span data-ttu-id="ecf8c-143">Data e hora de expiração do perfil opcional.</span><span class="sxs-lookup"><span data-stu-id="ecf8c-143">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="ecf8c-144">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="ecf8c-144">payloadFileName</span></span>|<span data-ttu-id="ecf8c-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecf8c-145">String</span></span>|<span data-ttu-id="ecf8c-146">Nome do arquivo de carga (\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="ecf8c-146">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="ecf8c-147">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="ecf8c-147">\*.xml).</span></span>|
|<span data-ttu-id="ecf8c-148">payload</span><span class="sxs-lookup"><span data-stu-id="ecf8c-148">payload</span></span>|<span data-ttu-id="ecf8c-149">Binária</span><span class="sxs-lookup"><span data-stu-id="ecf8c-149">Binary</span></span>|<span data-ttu-id="ecf8c-150">Carga.</span><span class="sxs-lookup"><span data-stu-id="ecf8c-150">Payload.</span></span> <span data-ttu-id="ecf8c-151">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="ecf8c-151">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="ecf8c-152">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ecf8c-152">roleScopeTagIds</span></span>|<span data-ttu-id="ecf8c-153">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecf8c-153">String collection</span></span>|<span data-ttu-id="ecf8c-154">Lista de marcas de escopo para esta entidade de configuração de provisionamento do aplicativo LOB iOS.</span><span class="sxs-lookup"><span data-stu-id="ecf8c-154">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="ecf8c-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ecf8c-155">createdDateTime</span></span>|<span data-ttu-id="ecf8c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecf8c-156">DateTimeOffset</span></span>|<span data-ttu-id="ecf8c-157">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ecf8c-157">DateTime the object was created.</span></span>|
|<span data-ttu-id="ecf8c-158">descrição</span><span class="sxs-lookup"><span data-stu-id="ecf8c-158">description</span></span>|<span data-ttu-id="ecf8c-159">String</span><span class="sxs-lookup"><span data-stu-id="ecf8c-159">String</span></span>|<span data-ttu-id="ecf8c-160">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ecf8c-160">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="ecf8c-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ecf8c-161">lastModifiedDateTime</span></span>|<span data-ttu-id="ecf8c-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecf8c-162">DateTimeOffset</span></span>|<span data-ttu-id="ecf8c-163">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ecf8c-163">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="ecf8c-164">displayName</span><span class="sxs-lookup"><span data-stu-id="ecf8c-164">displayName</span></span>|<span data-ttu-id="ecf8c-165">String</span><span class="sxs-lookup"><span data-stu-id="ecf8c-165">String</span></span>|<span data-ttu-id="ecf8c-166">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ecf8c-166">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="ecf8c-167">versão</span><span class="sxs-lookup"><span data-stu-id="ecf8c-167">version</span></span>|<span data-ttu-id="ecf8c-168">Int32</span><span class="sxs-lookup"><span data-stu-id="ecf8c-168">Int32</span></span>|<span data-ttu-id="ecf8c-169">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ecf8c-169">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="ecf8c-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecf8c-170">Response</span></span>
<span data-ttu-id="ecf8c-171">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ecf8c-171">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecf8c-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ecf8c-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecf8c-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ecf8c-173">Request</span></span>
<span data-ttu-id="ecf8c-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ecf8c-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ecf8c-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecf8c-175">Response</span></span>
<span data-ttu-id="ecf8c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ecf8c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




