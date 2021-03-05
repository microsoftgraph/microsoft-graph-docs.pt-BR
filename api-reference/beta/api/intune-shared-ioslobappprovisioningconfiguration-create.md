---
title: Criar iosLobAppProvisioningConfiguration
description: Crie um novo objeto iosLobAppProvisioningConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bcd4d470f9f8754b152b3af5587b02ed90459134
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470820"
---
# <a name="create-ioslobappprovisioningconfiguration"></a><span data-ttu-id="7ed4e-103">Criar iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="7ed4e-103">Create iosLobAppProvisioningConfiguration</span></span>

<span data-ttu-id="7ed4e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ed4e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ed4e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7ed4e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ed4e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ed4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ed4e-107">Crie um novo [objeto iosLobAppProvisioningConfiguration.](../resources/intune-shared-ioslobappprovisioningconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ed4e-107">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ed4e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7ed4e-108">Prerequisites</span></span>
<span data-ttu-id="7ed4e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ed4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ed4e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ed4e-111">Permission type</span></span>|<span data-ttu-id="7ed4e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7ed4e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ed4e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ed4e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7ed4e-114">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="7ed4e-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="7ed4e-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ed4e-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="7ed4e-116">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="7ed4e-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="7ed4e-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ed4e-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7ed4e-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ed4e-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ed4e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ed4e-119">Not supported.</span></span>|
|<span data-ttu-id="7ed4e-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ed4e-120">Application</span></span>||
| <span data-ttu-id="7ed4e-121">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="7ed4e-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="7ed4e-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ed4e-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="7ed4e-123">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="7ed4e-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="7ed4e-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ed4e-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ed4e-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ed4e-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7ed4e-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ed4e-126">Request headers</span></span>
|<span data-ttu-id="7ed4e-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7ed4e-127">Header</span></span>|<span data-ttu-id="7ed4e-128">Valor</span><span class="sxs-lookup"><span data-stu-id="7ed4e-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ed4e-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ed4e-129">Authorization</span></span>|<span data-ttu-id="7ed4e-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ed4e-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ed4e-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7ed4e-131">Accept</span></span>|<span data-ttu-id="7ed4e-132">application/json</span><span class="sxs-lookup"><span data-stu-id="7ed4e-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ed4e-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ed4e-133">Request body</span></span>
<span data-ttu-id="7ed4e-134">No corpo da solicitação, fornece uma representação JSON para o objeto iosLobAppProvisioningConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7ed4e-134">In the request body, supply a JSON representation for the iosLobAppProvisioningConfiguration object.</span></span>

<span data-ttu-id="7ed4e-135">A tabela a seguir mostra as propriedades que são necessárias ao criar iosLobAppProvisioningConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7ed4e-135">The following table shows the properties that are required when you create the iosLobAppProvisioningConfiguration.</span></span>

|<span data-ttu-id="7ed4e-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ed4e-136">Property</span></span>|<span data-ttu-id="7ed4e-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ed4e-137">Type</span></span>|<span data-ttu-id="7ed4e-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ed4e-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ed4e-139">id</span><span class="sxs-lookup"><span data-stu-id="7ed4e-139">id</span></span>|<span data-ttu-id="7ed4e-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed4e-140">String</span></span>|<span data-ttu-id="7ed4e-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7ed4e-141">Key of the entity.</span></span>|
|<span data-ttu-id="7ed4e-142">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7ed4e-142">expirationDateTime</span></span>|<span data-ttu-id="7ed4e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ed4e-143">DateTimeOffset</span></span>|<span data-ttu-id="7ed4e-144">Data e hora opcionais de expiração do perfil.</span><span class="sxs-lookup"><span data-stu-id="7ed4e-144">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="7ed4e-145">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="7ed4e-145">payloadFileName</span></span>|<span data-ttu-id="7ed4e-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed4e-146">String</span></span>|<span data-ttu-id="7ed4e-147">Nome do arquivo de carga (\*.mobileprovision \| \*.xml).</span><span class="sxs-lookup"><span data-stu-id="7ed4e-147">Payload file name (\*.mobileprovision \| \*.xml).</span></span>|
|<span data-ttu-id="7ed4e-148">payload</span><span class="sxs-lookup"><span data-stu-id="7ed4e-148">payload</span></span>|<span data-ttu-id="7ed4e-149">Binária</span><span class="sxs-lookup"><span data-stu-id="7ed4e-149">Binary</span></span>|<span data-ttu-id="7ed4e-150">Carga.</span><span class="sxs-lookup"><span data-stu-id="7ed4e-150">Payload.</span></span> <span data-ttu-id="7ed4e-151">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="7ed4e-151">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="7ed4e-152">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7ed4e-152">roleScopeTagIds</span></span>|<span data-ttu-id="7ed4e-153">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed4e-153">String collection</span></span>|<span data-ttu-id="7ed4e-154">Lista de Marcas de Escopo para essa entidade de configuração de provisionamento de aplicativos LOB do iOS.</span><span class="sxs-lookup"><span data-stu-id="7ed4e-154">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="7ed4e-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ed4e-155">createdDateTime</span></span>|<span data-ttu-id="7ed4e-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ed4e-156">DateTimeOffset</span></span>|<span data-ttu-id="7ed4e-157">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7ed4e-157">DateTime the object was created.</span></span>|
|<span data-ttu-id="7ed4e-158">description</span><span class="sxs-lookup"><span data-stu-id="7ed4e-158">description</span></span>|<span data-ttu-id="7ed4e-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed4e-159">String</span></span>|<span data-ttu-id="7ed4e-160">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7ed4e-160">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="7ed4e-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ed4e-161">lastModifiedDateTime</span></span>|<span data-ttu-id="7ed4e-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ed4e-162">DateTimeOffset</span></span>|<span data-ttu-id="7ed4e-163">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7ed4e-163">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="7ed4e-164">displayName</span><span class="sxs-lookup"><span data-stu-id="7ed4e-164">displayName</span></span>|<span data-ttu-id="7ed4e-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed4e-165">String</span></span>|<span data-ttu-id="7ed4e-166">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7ed4e-166">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="7ed4e-167">versão</span><span class="sxs-lookup"><span data-stu-id="7ed4e-167">version</span></span>|<span data-ttu-id="7ed4e-168">Int32</span><span class="sxs-lookup"><span data-stu-id="7ed4e-168">Int32</span></span>|<span data-ttu-id="7ed4e-169">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7ed4e-169">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="7ed4e-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ed4e-170">Response</span></span>
<span data-ttu-id="7ed4e-171">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ed4e-171">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ed4e-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ed4e-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ed4e-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ed4e-173">Request</span></span>
<span data-ttu-id="7ed4e-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ed4e-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7ed4e-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ed4e-175">Response</span></span>
<span data-ttu-id="7ed4e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ed4e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







