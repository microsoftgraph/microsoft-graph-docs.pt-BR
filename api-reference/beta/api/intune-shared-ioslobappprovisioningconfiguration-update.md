---
title: Atualizar iosLobAppProvisioningConfiguration
description: Atualiza as propriedades de um objeto iosLobAppProvisioningConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ed21829fda05a9b89d8440b9c2729439a8abe9ee
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538333"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="67178-103">Atualizar iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="67178-103">Update iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="67178-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67178-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67178-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67178-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67178-106">Atualiza as propriedades de um objeto [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="67178-106">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67178-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67178-107">Prerequisites</span></span>
<span data-ttu-id="67178-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67178-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67178-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67178-110">Permission type</span></span>|<span data-ttu-id="67178-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="67178-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67178-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67178-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="67178-113">&nbsp;&nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="67178-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="67178-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67178-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="67178-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="67178-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="67178-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67178-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="67178-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67178-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67178-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67178-118">Not supported.</span></span>|
|<span data-ttu-id="67178-119">Application</span><span class="sxs-lookup"><span data-stu-id="67178-119">Application</span></span>||
| <span data-ttu-id="67178-120">&nbsp;&nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="67178-120">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="67178-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67178-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="67178-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="67178-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="67178-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67178-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="67178-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67178-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="67178-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67178-125">Request headers</span></span>
|<span data-ttu-id="67178-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67178-126">Header</span></span>|<span data-ttu-id="67178-127">Valor</span><span class="sxs-lookup"><span data-stu-id="67178-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67178-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="67178-128">Authorization</span></span>|<span data-ttu-id="67178-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67178-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67178-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67178-130">Accept</span></span>|<span data-ttu-id="67178-131">application/json</span><span class="sxs-lookup"><span data-stu-id="67178-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67178-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67178-132">Request body</span></span>
<span data-ttu-id="67178-133">No corpo da solicitação, forneça uma representação JSON do objeto [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="67178-133">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="67178-134">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67178-134">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="67178-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67178-135">Property</span></span>|<span data-ttu-id="67178-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="67178-136">Type</span></span>|<span data-ttu-id="67178-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="67178-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67178-138">id</span><span class="sxs-lookup"><span data-stu-id="67178-138">id</span></span>|<span data-ttu-id="67178-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67178-139">String</span></span>|<span data-ttu-id="67178-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="67178-140">Key of the entity.</span></span>|
|<span data-ttu-id="67178-141">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="67178-141">expirationDateTime</span></span>|<span data-ttu-id="67178-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67178-142">DateTimeOffset</span></span>|<span data-ttu-id="67178-143">Data e hora de expiração do perfil opcional.</span><span class="sxs-lookup"><span data-stu-id="67178-143">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="67178-144">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="67178-144">payloadFileName</span></span>|<span data-ttu-id="67178-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67178-145">String</span></span>|<span data-ttu-id="67178-146">Nome do arquivo de carga (\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="67178-146">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="67178-147">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="67178-147">\*.xml).</span></span>|
|<span data-ttu-id="67178-148">payload</span><span class="sxs-lookup"><span data-stu-id="67178-148">payload</span></span>|<span data-ttu-id="67178-149">Binária</span><span class="sxs-lookup"><span data-stu-id="67178-149">Binary</span></span>|<span data-ttu-id="67178-150">Carga.</span><span class="sxs-lookup"><span data-stu-id="67178-150">Payload.</span></span> <span data-ttu-id="67178-151">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="67178-151">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="67178-152">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="67178-152">roleScopeTagIds</span></span>|<span data-ttu-id="67178-153">String collection</span><span class="sxs-lookup"><span data-stu-id="67178-153">String collection</span></span>|<span data-ttu-id="67178-154">Lista de marcas de escopo para esta entidade de configuração de provisionamento do aplicativo LOB iOS.</span><span class="sxs-lookup"><span data-stu-id="67178-154">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="67178-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67178-155">createdDateTime</span></span>|<span data-ttu-id="67178-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67178-156">DateTimeOffset</span></span>|<span data-ttu-id="67178-157">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="67178-157">DateTime the object was created.</span></span>|
|<span data-ttu-id="67178-158">description</span><span class="sxs-lookup"><span data-stu-id="67178-158">description</span></span>|<span data-ttu-id="67178-159">String</span><span class="sxs-lookup"><span data-stu-id="67178-159">String</span></span>|<span data-ttu-id="67178-160">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="67178-160">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="67178-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67178-161">lastModifiedDateTime</span></span>|<span data-ttu-id="67178-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67178-162">DateTimeOffset</span></span>|<span data-ttu-id="67178-163">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="67178-163">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="67178-164">displayName</span><span class="sxs-lookup"><span data-stu-id="67178-164">displayName</span></span>|<span data-ttu-id="67178-165">String</span><span class="sxs-lookup"><span data-stu-id="67178-165">String</span></span>|<span data-ttu-id="67178-166">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="67178-166">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="67178-167">versão</span><span class="sxs-lookup"><span data-stu-id="67178-167">version</span></span>|<span data-ttu-id="67178-168">Int32</span><span class="sxs-lookup"><span data-stu-id="67178-168">Int32</span></span>|<span data-ttu-id="67178-169">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="67178-169">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="67178-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="67178-170">Response</span></span>
<span data-ttu-id="67178-171">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67178-171">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67178-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67178-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="67178-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67178-173">Request</span></span>
<span data-ttu-id="67178-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67178-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
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

### <a name="response"></a><span data-ttu-id="67178-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="67178-175">Response</span></span>
<span data-ttu-id="67178-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67178-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






