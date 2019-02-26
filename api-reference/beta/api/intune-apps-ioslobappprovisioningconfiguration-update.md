---
title: Atualizar iosLobAppProvisioningConfiguration
description: Atualiza as propriedades de um objeto iosLobAppProvisioningConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 191df244cf163d0a5980c9fc0c5ae3a444e3468c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173084"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="4bdc8-103">Atualizar iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="4bdc8-103">Update iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="4bdc8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4bdc8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4bdc8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4bdc8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bdc8-106">Atualiza as propriedades de um objeto [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4bdc8-106">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4bdc8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4bdc8-107">Prerequisites</span></span>
<span data-ttu-id="4bdc8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4bdc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4bdc8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4bdc8-110">Permission type</span></span>|<span data-ttu-id="4bdc8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4bdc8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bdc8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4bdc8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4bdc8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bdc8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4bdc8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4bdc8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bdc8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bdc8-115">Not supported.</span></span>|
|<span data-ttu-id="4bdc8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bdc8-116">Application</span></span>|<span data-ttu-id="4bdc8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bdc8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bdc8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4bdc8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4bdc8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4bdc8-119">Request headers</span></span>
|<span data-ttu-id="4bdc8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4bdc8-120">Header</span></span>|<span data-ttu-id="4bdc8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4bdc8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bdc8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4bdc8-122">Authorization</span></span>|<span data-ttu-id="4bdc8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4bdc8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bdc8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4bdc8-124">Accept</span></span>|<span data-ttu-id="4bdc8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4bdc8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bdc8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4bdc8-126">Request body</span></span>
<span data-ttu-id="4bdc8-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4bdc8-127">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="4bdc8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bdc8-128">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="4bdc8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4bdc8-129">Property</span></span>|<span data-ttu-id="4bdc8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bdc8-130">Type</span></span>|<span data-ttu-id="4bdc8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bdc8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bdc8-132">id</span><span class="sxs-lookup"><span data-stu-id="4bdc8-132">id</span></span>|<span data-ttu-id="4bdc8-133">String</span><span class="sxs-lookup"><span data-stu-id="4bdc8-133">String</span></span>|<span data-ttu-id="4bdc8-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4bdc8-134">Key of the entity.</span></span>|
|<span data-ttu-id="4bdc8-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4bdc8-135">expirationDateTime</span></span>|<span data-ttu-id="4bdc8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bdc8-136">DateTimeOffset</span></span>|<span data-ttu-id="4bdc8-137">Data e hora de expiração do perfil opcional.</span><span class="sxs-lookup"><span data-stu-id="4bdc8-137">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="4bdc8-138">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="4bdc8-138">payloadFileName</span></span>|<span data-ttu-id="4bdc8-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4bdc8-139">String</span></span>|<span data-ttu-id="4bdc8-140">Nome do arquivo de carga (\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="4bdc8-140">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="4bdc8-141">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="4bdc8-141">\*.xml).</span></span>|
|<span data-ttu-id="4bdc8-142">payload</span><span class="sxs-lookup"><span data-stu-id="4bdc8-142">payload</span></span>|<span data-ttu-id="4bdc8-143">Binária</span><span class="sxs-lookup"><span data-stu-id="4bdc8-143">Binary</span></span>|<span data-ttu-id="4bdc8-144">Carga.</span><span class="sxs-lookup"><span data-stu-id="4bdc8-144">Payload.</span></span> <span data-ttu-id="4bdc8-145">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="4bdc8-145">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="4bdc8-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4bdc8-146">createdDateTime</span></span>|<span data-ttu-id="4bdc8-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bdc8-147">DateTimeOffset</span></span>|<span data-ttu-id="4bdc8-148">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4bdc8-148">DateTime the object was created.</span></span>|
|<span data-ttu-id="4bdc8-149">description</span><span class="sxs-lookup"><span data-stu-id="4bdc8-149">description</span></span>|<span data-ttu-id="4bdc8-150">String</span><span class="sxs-lookup"><span data-stu-id="4bdc8-150">String</span></span>|<span data-ttu-id="4bdc8-151">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4bdc8-151">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="4bdc8-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4bdc8-152">lastModifiedDateTime</span></span>|<span data-ttu-id="4bdc8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bdc8-153">DateTimeOffset</span></span>|<span data-ttu-id="4bdc8-154">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4bdc8-154">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="4bdc8-155">displayName</span><span class="sxs-lookup"><span data-stu-id="4bdc8-155">displayName</span></span>|<span data-ttu-id="4bdc8-156">String</span><span class="sxs-lookup"><span data-stu-id="4bdc8-156">String</span></span>|<span data-ttu-id="4bdc8-157">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4bdc8-157">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="4bdc8-158">version</span><span class="sxs-lookup"><span data-stu-id="4bdc8-158">version</span></span>|<span data-ttu-id="4bdc8-159">Int32</span><span class="sxs-lookup"><span data-stu-id="4bdc8-159">Int32</span></span>|<span data-ttu-id="4bdc8-160">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4bdc8-160">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="4bdc8-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bdc8-161">Response</span></span>
<span data-ttu-id="4bdc8-162">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bdc8-162">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bdc8-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4bdc8-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="4bdc8-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bdc8-164">Request</span></span>
<span data-ttu-id="4bdc8-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bdc8-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
Content-type: application/json
Content-length: 313

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="4bdc8-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bdc8-166">Response</span></span>
<span data-ttu-id="4bdc8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4bdc8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 485

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "id": "e2a23631-3631-e2a2-3136-a2e23136a2e2",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```




