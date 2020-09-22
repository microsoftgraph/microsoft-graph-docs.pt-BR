---
title: Criar iosLobAppProvisioningConfiguration
description: Criar um novo objeto iosLobAppProvisioningConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 486cbb24942d8b595cee229009bbfba46a4c62cf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036293"
---
# <a name="create-ioslobappprovisioningconfiguration"></a><span data-ttu-id="a51df-103">Criar iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="a51df-103">Create iosLobAppProvisioningConfiguration</span></span>

<span data-ttu-id="a51df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a51df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a51df-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a51df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a51df-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a51df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a51df-107">Criar um novo objeto [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a51df-107">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a51df-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a51df-108">Prerequisites</span></span>
<span data-ttu-id="a51df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a51df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a51df-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a51df-111">Permission type</span></span>|<span data-ttu-id="a51df-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a51df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a51df-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a51df-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a51df-114">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="a51df-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="a51df-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a51df-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="a51df-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="a51df-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="a51df-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a51df-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a51df-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a51df-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a51df-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a51df-119">Not supported.</span></span>|
|<span data-ttu-id="a51df-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a51df-120">Application</span></span>||
| <span data-ttu-id="a51df-121">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="a51df-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="a51df-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a51df-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="a51df-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="a51df-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="a51df-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a51df-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a51df-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a51df-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a51df-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a51df-126">Request headers</span></span>
|<span data-ttu-id="a51df-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a51df-127">Header</span></span>|<span data-ttu-id="a51df-128">Valor</span><span class="sxs-lookup"><span data-stu-id="a51df-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a51df-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="a51df-129">Authorization</span></span>|<span data-ttu-id="a51df-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a51df-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a51df-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a51df-131">Accept</span></span>|<span data-ttu-id="a51df-132">application/json</span><span class="sxs-lookup"><span data-stu-id="a51df-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a51df-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a51df-133">Request body</span></span>
<span data-ttu-id="a51df-134">No corpo da solicitação, forneça uma representação JSON do objeto iosLobAppProvisioningConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a51df-134">In the request body, supply a JSON representation for the iosLobAppProvisioningConfiguration object.</span></span>

<span data-ttu-id="a51df-135">A tabela a seguir mostra as propriedades que são necessárias ao criar iosLobAppProvisioningConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a51df-135">The following table shows the properties that are required when you create the iosLobAppProvisioningConfiguration.</span></span>

|<span data-ttu-id="a51df-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a51df-136">Property</span></span>|<span data-ttu-id="a51df-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="a51df-137">Type</span></span>|<span data-ttu-id="a51df-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="a51df-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a51df-139">id</span><span class="sxs-lookup"><span data-stu-id="a51df-139">id</span></span>|<span data-ttu-id="a51df-140">String</span><span class="sxs-lookup"><span data-stu-id="a51df-140">String</span></span>|<span data-ttu-id="a51df-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a51df-141">Key of the entity.</span></span>|
|<span data-ttu-id="a51df-142">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a51df-142">expirationDateTime</span></span>|<span data-ttu-id="a51df-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a51df-143">DateTimeOffset</span></span>|<span data-ttu-id="a51df-144">Data e hora de expiração do perfil opcional.</span><span class="sxs-lookup"><span data-stu-id="a51df-144">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="a51df-145">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="a51df-145">payloadFileName</span></span>|<span data-ttu-id="a51df-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a51df-146">String</span></span>|<span data-ttu-id="a51df-147">Nome do arquivo de carga (\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="a51df-147">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="a51df-148">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="a51df-148">\*.xml).</span></span>|
|<span data-ttu-id="a51df-149">payload</span><span class="sxs-lookup"><span data-stu-id="a51df-149">payload</span></span>|<span data-ttu-id="a51df-150">Binária</span><span class="sxs-lookup"><span data-stu-id="a51df-150">Binary</span></span>|<span data-ttu-id="a51df-151">Carga.</span><span class="sxs-lookup"><span data-stu-id="a51df-151">Payload.</span></span> <span data-ttu-id="a51df-152">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="a51df-152">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="a51df-153">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a51df-153">roleScopeTagIds</span></span>|<span data-ttu-id="a51df-154">Coleção String</span><span class="sxs-lookup"><span data-stu-id="a51df-154">String collection</span></span>|<span data-ttu-id="a51df-155">Lista de marcas de escopo para esta entidade de configuração de provisionamento do aplicativo LOB iOS.</span><span class="sxs-lookup"><span data-stu-id="a51df-155">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="a51df-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a51df-156">createdDateTime</span></span>|<span data-ttu-id="a51df-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a51df-157">DateTimeOffset</span></span>|<span data-ttu-id="a51df-158">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a51df-158">DateTime the object was created.</span></span>|
|<span data-ttu-id="a51df-159">description</span><span class="sxs-lookup"><span data-stu-id="a51df-159">description</span></span>|<span data-ttu-id="a51df-160">String</span><span class="sxs-lookup"><span data-stu-id="a51df-160">String</span></span>|<span data-ttu-id="a51df-161">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a51df-161">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="a51df-162">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a51df-162">lastModifiedDateTime</span></span>|<span data-ttu-id="a51df-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a51df-163">DateTimeOffset</span></span>|<span data-ttu-id="a51df-164">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a51df-164">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="a51df-165">displayName</span><span class="sxs-lookup"><span data-stu-id="a51df-165">displayName</span></span>|<span data-ttu-id="a51df-166">String</span><span class="sxs-lookup"><span data-stu-id="a51df-166">String</span></span>|<span data-ttu-id="a51df-167">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a51df-167">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="a51df-168">versão</span><span class="sxs-lookup"><span data-stu-id="a51df-168">version</span></span>|<span data-ttu-id="a51df-169">Int32</span><span class="sxs-lookup"><span data-stu-id="a51df-169">Int32</span></span>|<span data-ttu-id="a51df-170">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a51df-170">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="a51df-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="a51df-171">Response</span></span>
<span data-ttu-id="a51df-172">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a51df-172">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a51df-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a51df-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="a51df-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a51df-174">Request</span></span>
<span data-ttu-id="a51df-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a51df-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a51df-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="a51df-176">Response</span></span>
<span data-ttu-id="a51df-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a51df-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









