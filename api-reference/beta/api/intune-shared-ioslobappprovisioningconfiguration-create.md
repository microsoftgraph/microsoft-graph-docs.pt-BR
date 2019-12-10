---
title: Criar iosLobAppProvisioningConfiguration
description: Criar um novo objeto iosLobAppProvisioningConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f6b260334bfc2a81d48df06107a864c4a0efa018
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939855"
---
# <a name="create-ioslobappprovisioningconfiguration"></a><span data-ttu-id="270e2-103">Criar iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="270e2-103">Create iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="270e2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="270e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="270e2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="270e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="270e2-106">Criar um novo objeto [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="270e2-106">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="270e2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="270e2-107">Prerequisites</span></span>
<span data-ttu-id="270e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="270e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="270e2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="270e2-110">Permission type</span></span>|<span data-ttu-id="270e2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="270e2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="270e2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="270e2-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="270e2-113">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="270e2-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="270e2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="270e2-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="270e2-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="270e2-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="270e2-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="270e2-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="270e2-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="270e2-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="270e2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="270e2-118">Not supported.</span></span>|
|<span data-ttu-id="270e2-119">Application</span><span class="sxs-lookup"><span data-stu-id="270e2-119">Application</span></span>||
| <span data-ttu-id="270e2-120">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="270e2-120">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="270e2-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="270e2-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="270e2-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="270e2-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="270e2-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="270e2-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="270e2-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="270e2-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="270e2-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="270e2-125">Request headers</span></span>
|<span data-ttu-id="270e2-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="270e2-126">Header</span></span>|<span data-ttu-id="270e2-127">Valor</span><span class="sxs-lookup"><span data-stu-id="270e2-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="270e2-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="270e2-128">Authorization</span></span>|<span data-ttu-id="270e2-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="270e2-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="270e2-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="270e2-130">Accept</span></span>|<span data-ttu-id="270e2-131">application/json</span><span class="sxs-lookup"><span data-stu-id="270e2-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="270e2-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="270e2-132">Request body</span></span>
<span data-ttu-id="270e2-133">No corpo da solicitação, forneça uma representação JSON do objeto iosLobAppProvisioningConfiguration.</span><span class="sxs-lookup"><span data-stu-id="270e2-133">In the request body, supply a JSON representation for the iosLobAppProvisioningConfiguration object.</span></span>

<span data-ttu-id="270e2-134">A tabela a seguir mostra as propriedades que são necessárias ao criar iosLobAppProvisioningConfiguration.</span><span class="sxs-lookup"><span data-stu-id="270e2-134">The following table shows the properties that are required when you create the iosLobAppProvisioningConfiguration.</span></span>

|<span data-ttu-id="270e2-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="270e2-135">Property</span></span>|<span data-ttu-id="270e2-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="270e2-136">Type</span></span>|<span data-ttu-id="270e2-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="270e2-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="270e2-138">id</span><span class="sxs-lookup"><span data-stu-id="270e2-138">id</span></span>|<span data-ttu-id="270e2-139">String</span><span class="sxs-lookup"><span data-stu-id="270e2-139">String</span></span>|<span data-ttu-id="270e2-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="270e2-140">Key of the entity.</span></span>|
|<span data-ttu-id="270e2-141">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="270e2-141">expirationDateTime</span></span>|<span data-ttu-id="270e2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="270e2-142">DateTimeOffset</span></span>|<span data-ttu-id="270e2-143">Data e hora de expiração do perfil opcional.</span><span class="sxs-lookup"><span data-stu-id="270e2-143">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="270e2-144">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="270e2-144">payloadFileName</span></span>|<span data-ttu-id="270e2-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="270e2-145">String</span></span>|<span data-ttu-id="270e2-146">Nome do arquivo de carga (\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="270e2-146">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="270e2-147">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="270e2-147">\*.xml).</span></span>|
|<span data-ttu-id="270e2-148">payload</span><span class="sxs-lookup"><span data-stu-id="270e2-148">payload</span></span>|<span data-ttu-id="270e2-149">Binária</span><span class="sxs-lookup"><span data-stu-id="270e2-149">Binary</span></span>|<span data-ttu-id="270e2-150">Carga.</span><span class="sxs-lookup"><span data-stu-id="270e2-150">Payload.</span></span> <span data-ttu-id="270e2-151">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="270e2-151">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="270e2-152">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="270e2-152">roleScopeTagIds</span></span>|<span data-ttu-id="270e2-153">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="270e2-153">String collection</span></span>|<span data-ttu-id="270e2-154">Lista de marcas de escopo para esta entidade de configuração de provisionamento do aplicativo LOB iOS.</span><span class="sxs-lookup"><span data-stu-id="270e2-154">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="270e2-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="270e2-155">createdDateTime</span></span>|<span data-ttu-id="270e2-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="270e2-156">DateTimeOffset</span></span>|<span data-ttu-id="270e2-157">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="270e2-157">DateTime the object was created.</span></span>|
|<span data-ttu-id="270e2-158">description</span><span class="sxs-lookup"><span data-stu-id="270e2-158">description</span></span>|<span data-ttu-id="270e2-159">String</span><span class="sxs-lookup"><span data-stu-id="270e2-159">String</span></span>|<span data-ttu-id="270e2-160">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="270e2-160">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="270e2-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="270e2-161">lastModifiedDateTime</span></span>|<span data-ttu-id="270e2-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="270e2-162">DateTimeOffset</span></span>|<span data-ttu-id="270e2-163">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="270e2-163">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="270e2-164">displayName</span><span class="sxs-lookup"><span data-stu-id="270e2-164">displayName</span></span>|<span data-ttu-id="270e2-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="270e2-165">String</span></span>|<span data-ttu-id="270e2-166">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="270e2-166">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="270e2-167">versão</span><span class="sxs-lookup"><span data-stu-id="270e2-167">version</span></span>|<span data-ttu-id="270e2-168">Int32</span><span class="sxs-lookup"><span data-stu-id="270e2-168">Int32</span></span>|<span data-ttu-id="270e2-169">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="270e2-169">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="270e2-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="270e2-170">Response</span></span>
<span data-ttu-id="270e2-171">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="270e2-171">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="270e2-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="270e2-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="270e2-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="270e2-173">Request</span></span>
<span data-ttu-id="270e2-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="270e2-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="270e2-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="270e2-175">Response</span></span>
<span data-ttu-id="270e2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="270e2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








