---
title: Atualizar iosLobAppProvisioningConfiguration
description: Atualiza as propriedades de um objeto iosLobAppProvisioningConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 157c653ed36f87c6c6a8f2ee5a28da05eb784d44
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729900"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="48630-103">Atualizar iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="48630-103">Update iosLobAppProvisioningConfiguration</span></span>

<span data-ttu-id="48630-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48630-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="48630-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="48630-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48630-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="48630-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48630-107">Atualiza as propriedades de um objeto [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="48630-107">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48630-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="48630-108">Prerequisites</span></span>
<span data-ttu-id="48630-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48630-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48630-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48630-111">Permission type</span></span>|<span data-ttu-id="48630-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="48630-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48630-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48630-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="48630-114">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="48630-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="48630-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48630-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="48630-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="48630-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="48630-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48630-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="48630-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48630-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48630-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48630-119">Not supported.</span></span>|
|<span data-ttu-id="48630-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48630-120">Application</span></span>||
| <span data-ttu-id="48630-121">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="48630-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="48630-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48630-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="48630-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="48630-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="48630-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48630-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="48630-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48630-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="48630-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48630-126">Request headers</span></span>
|<span data-ttu-id="48630-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="48630-127">Header</span></span>|<span data-ttu-id="48630-128">Valor</span><span class="sxs-lookup"><span data-stu-id="48630-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48630-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="48630-129">Authorization</span></span>|<span data-ttu-id="48630-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48630-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48630-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="48630-131">Accept</span></span>|<span data-ttu-id="48630-132">application/json</span><span class="sxs-lookup"><span data-stu-id="48630-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48630-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48630-133">Request body</span></span>
<span data-ttu-id="48630-134">No corpo da solicitação, forneça uma representação JSON do objeto [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="48630-134">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="48630-135">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48630-135">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="48630-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48630-136">Property</span></span>|<span data-ttu-id="48630-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="48630-137">Type</span></span>|<span data-ttu-id="48630-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="48630-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48630-139">id</span><span class="sxs-lookup"><span data-stu-id="48630-139">id</span></span>|<span data-ttu-id="48630-140">String</span><span class="sxs-lookup"><span data-stu-id="48630-140">String</span></span>|<span data-ttu-id="48630-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="48630-141">Key of the entity.</span></span>|
|<span data-ttu-id="48630-142">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="48630-142">expirationDateTime</span></span>|<span data-ttu-id="48630-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48630-143">DateTimeOffset</span></span>|<span data-ttu-id="48630-144">Data e hora de expiração do perfil opcional.</span><span class="sxs-lookup"><span data-stu-id="48630-144">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="48630-145">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="48630-145">payloadFileName</span></span>|<span data-ttu-id="48630-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48630-146">String</span></span>|<span data-ttu-id="48630-147">Nome do arquivo de carga (\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="48630-147">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="48630-148">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="48630-148">\*.xml).</span></span>|
|<span data-ttu-id="48630-149">payload</span><span class="sxs-lookup"><span data-stu-id="48630-149">payload</span></span>|<span data-ttu-id="48630-150">Binária</span><span class="sxs-lookup"><span data-stu-id="48630-150">Binary</span></span>|<span data-ttu-id="48630-151">Carga.</span><span class="sxs-lookup"><span data-stu-id="48630-151">Payload.</span></span> <span data-ttu-id="48630-152">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="48630-152">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="48630-153">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="48630-153">roleScopeTagIds</span></span>|<span data-ttu-id="48630-154">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="48630-154">String collection</span></span>|<span data-ttu-id="48630-155">Lista de marcas de escopo para esta entidade de configuração de provisionamento do aplicativo LOB iOS.</span><span class="sxs-lookup"><span data-stu-id="48630-155">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="48630-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48630-156">createdDateTime</span></span>|<span data-ttu-id="48630-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48630-157">DateTimeOffset</span></span>|<span data-ttu-id="48630-158">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="48630-158">DateTime the object was created.</span></span>|
|<span data-ttu-id="48630-159">description</span><span class="sxs-lookup"><span data-stu-id="48630-159">description</span></span>|<span data-ttu-id="48630-160">String</span><span class="sxs-lookup"><span data-stu-id="48630-160">String</span></span>|<span data-ttu-id="48630-161">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="48630-161">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="48630-162">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48630-162">lastModifiedDateTime</span></span>|<span data-ttu-id="48630-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48630-163">DateTimeOffset</span></span>|<span data-ttu-id="48630-164">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="48630-164">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="48630-165">displayName</span><span class="sxs-lookup"><span data-stu-id="48630-165">displayName</span></span>|<span data-ttu-id="48630-166">String</span><span class="sxs-lookup"><span data-stu-id="48630-166">String</span></span>|<span data-ttu-id="48630-167">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="48630-167">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="48630-168">versão</span><span class="sxs-lookup"><span data-stu-id="48630-168">version</span></span>|<span data-ttu-id="48630-169">Int32</span><span class="sxs-lookup"><span data-stu-id="48630-169">Int32</span></span>|<span data-ttu-id="48630-170">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="48630-170">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="48630-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="48630-171">Response</span></span>
<span data-ttu-id="48630-172">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48630-172">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48630-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48630-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="48630-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48630-174">Request</span></span>
<span data-ttu-id="48630-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="48630-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="48630-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="48630-176">Response</span></span>
<span data-ttu-id="48630-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48630-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








