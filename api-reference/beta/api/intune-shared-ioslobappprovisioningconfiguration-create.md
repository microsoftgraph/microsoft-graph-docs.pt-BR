---
title: Criar iosLobAppProvisioningConfiguration
description: Crie um novo objeto iosLobAppProvisioningConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8c78f8307ce3418b1bb27920b694ac87131023bd
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867718"
---
# <a name="create-ioslobappprovisioningconfiguration"></a><span data-ttu-id="d5aa9-103">Criar iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5aa9-103">Create iosLobAppProvisioningConfiguration</span></span>

<span data-ttu-id="d5aa9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5aa9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5aa9-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d5aa9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5aa9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d5aa9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5aa9-107">Crie um novo [objeto iosLobAppProvisioningConfiguration.](../resources/intune-shared-ioslobappprovisioningconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5aa9-107">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5aa9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d5aa9-108">Prerequisites</span></span>
<span data-ttu-id="d5aa9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5aa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5aa9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5aa9-111">Permission type</span></span>|<span data-ttu-id="d5aa9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d5aa9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5aa9-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5aa9-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d5aa9-114">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="d5aa9-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="d5aa9-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5aa9-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="d5aa9-116">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="d5aa9-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d5aa9-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5aa9-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d5aa9-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5aa9-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5aa9-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5aa9-119">Not supported.</span></span>|
|<span data-ttu-id="d5aa9-120">Application</span><span class="sxs-lookup"><span data-stu-id="d5aa9-120">Application</span></span>||
| <span data-ttu-id="d5aa9-121">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="d5aa9-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="d5aa9-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5aa9-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="d5aa9-123">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="d5aa9-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d5aa9-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5aa9-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5aa9-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5aa9-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d5aa9-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5aa9-126">Request headers</span></span>
|<span data-ttu-id="d5aa9-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d5aa9-127">Header</span></span>|<span data-ttu-id="d5aa9-128">Valor</span><span class="sxs-lookup"><span data-stu-id="d5aa9-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5aa9-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5aa9-129">Authorization</span></span>|<span data-ttu-id="d5aa9-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5aa9-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5aa9-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d5aa9-131">Accept</span></span>|<span data-ttu-id="d5aa9-132">application/json</span><span class="sxs-lookup"><span data-stu-id="d5aa9-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5aa9-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5aa9-133">Request body</span></span>
<span data-ttu-id="d5aa9-134">No corpo da solicitação, fornece uma representação JSON para o objeto iosLobAppProvisioningConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d5aa9-134">In the request body, supply a JSON representation for the iosLobAppProvisioningConfiguration object.</span></span>

<span data-ttu-id="d5aa9-135">A tabela a seguir mostra as propriedades que são necessárias ao criar iosLobAppProvisioningConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d5aa9-135">The following table shows the properties that are required when you create the iosLobAppProvisioningConfiguration.</span></span>

|<span data-ttu-id="d5aa9-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5aa9-136">Property</span></span>|<span data-ttu-id="d5aa9-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5aa9-137">Type</span></span>|<span data-ttu-id="d5aa9-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5aa9-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5aa9-139">id</span><span class="sxs-lookup"><span data-stu-id="d5aa9-139">id</span></span>|<span data-ttu-id="d5aa9-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5aa9-140">String</span></span>|<span data-ttu-id="d5aa9-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d5aa9-141">Key of the entity.</span></span>|
|<span data-ttu-id="d5aa9-142">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d5aa9-142">expirationDateTime</span></span>|<span data-ttu-id="d5aa9-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5aa9-143">DateTimeOffset</span></span>|<span data-ttu-id="d5aa9-144">Data e hora opcionais de expiração do perfil.</span><span class="sxs-lookup"><span data-stu-id="d5aa9-144">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="d5aa9-145">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="d5aa9-145">payloadFileName</span></span>|<span data-ttu-id="d5aa9-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5aa9-146">String</span></span>|<span data-ttu-id="d5aa9-147">Nome do arquivo de carga (\*.mobileprovision</span><span class="sxs-lookup"><span data-stu-id="d5aa9-147">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="d5aa9-148">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="d5aa9-148">\*.xml).</span></span>|
|<span data-ttu-id="d5aa9-149">payload</span><span class="sxs-lookup"><span data-stu-id="d5aa9-149">payload</span></span>|<span data-ttu-id="d5aa9-150">Binária</span><span class="sxs-lookup"><span data-stu-id="d5aa9-150">Binary</span></span>|<span data-ttu-id="d5aa9-151">Carga.</span><span class="sxs-lookup"><span data-stu-id="d5aa9-151">Payload.</span></span> <span data-ttu-id="d5aa9-152">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="d5aa9-152">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="d5aa9-153">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d5aa9-153">roleScopeTagIds</span></span>|<span data-ttu-id="d5aa9-154">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d5aa9-154">String collection</span></span>|<span data-ttu-id="d5aa9-155">Lista de Marcas de Escopo para essa entidade de configuração de provisionamento de aplicativos LOB do iOS.</span><span class="sxs-lookup"><span data-stu-id="d5aa9-155">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="d5aa9-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5aa9-156">createdDateTime</span></span>|<span data-ttu-id="d5aa9-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5aa9-157">DateTimeOffset</span></span>|<span data-ttu-id="d5aa9-158">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d5aa9-158">DateTime the object was created.</span></span>|
|<span data-ttu-id="d5aa9-159">description</span><span class="sxs-lookup"><span data-stu-id="d5aa9-159">description</span></span>|<span data-ttu-id="d5aa9-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5aa9-160">String</span></span>|<span data-ttu-id="d5aa9-161">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d5aa9-161">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="d5aa9-162">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5aa9-162">lastModifiedDateTime</span></span>|<span data-ttu-id="d5aa9-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5aa9-163">DateTimeOffset</span></span>|<span data-ttu-id="d5aa9-164">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d5aa9-164">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="d5aa9-165">displayName</span><span class="sxs-lookup"><span data-stu-id="d5aa9-165">displayName</span></span>|<span data-ttu-id="d5aa9-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5aa9-166">String</span></span>|<span data-ttu-id="d5aa9-167">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d5aa9-167">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="d5aa9-168">versão</span><span class="sxs-lookup"><span data-stu-id="d5aa9-168">version</span></span>|<span data-ttu-id="d5aa9-169">Int32</span><span class="sxs-lookup"><span data-stu-id="d5aa9-169">Int32</span></span>|<span data-ttu-id="d5aa9-170">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d5aa9-170">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="d5aa9-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5aa9-171">Response</span></span>
<span data-ttu-id="d5aa9-172">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5aa9-172">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5aa9-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5aa9-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5aa9-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5aa9-174">Request</span></span>
<span data-ttu-id="d5aa9-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5aa9-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d5aa9-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5aa9-176">Response</span></span>
<span data-ttu-id="d5aa9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5aa9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







