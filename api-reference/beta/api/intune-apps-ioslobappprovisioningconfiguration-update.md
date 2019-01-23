---
title: Atualizar iosLobAppProvisioningConfiguration
description: Atualize as propriedades de um objeto iosLobAppProvisioningConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d98e19b922b1fd9cd2c9205eae89c0637dca9436
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402668"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="6e7be-103">Atualizar iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e7be-103">Update iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="6e7be-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="6e7be-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6e7be-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6e7be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e7be-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="6e7be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e7be-107">Atualize as propriedades de um objeto [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6e7be-107">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e7be-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6e7be-108">Prerequisites</span></span>
<span data-ttu-id="6e7be-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6e7be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6e7be-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e7be-111">Permission type</span></span>|<span data-ttu-id="6e7be-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6e7be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e7be-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e7be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e7be-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e7be-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6e7be-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e7be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e7be-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e7be-116">Not supported.</span></span>|
|<span data-ttu-id="6e7be-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e7be-117">Application</span></span>|<span data-ttu-id="6e7be-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e7be-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e7be-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e7be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6e7be-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e7be-120">Request headers</span></span>
|<span data-ttu-id="6e7be-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e7be-121">Header</span></span>|<span data-ttu-id="6e7be-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6e7be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e7be-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e7be-123">Authorization</span></span>|<span data-ttu-id="6e7be-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e7be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e7be-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6e7be-125">Accept</span></span>|<span data-ttu-id="6e7be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e7be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e7be-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e7be-127">Request body</span></span>
<span data-ttu-id="6e7be-128">No corpo da solicitação, fornece uma representação JSON para o objeto [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6e7be-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="6e7be-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e7be-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="6e7be-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e7be-130">Property</span></span>|<span data-ttu-id="6e7be-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e7be-131">Type</span></span>|<span data-ttu-id="6e7be-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e7be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e7be-133">id</span><span class="sxs-lookup"><span data-stu-id="6e7be-133">id</span></span>|<span data-ttu-id="6e7be-134">String</span><span class="sxs-lookup"><span data-stu-id="6e7be-134">String</span></span>|<span data-ttu-id="6e7be-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6e7be-135">Key of the entity.</span></span>|
|<span data-ttu-id="6e7be-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6e7be-136">expirationDateTime</span></span>|<span data-ttu-id="6e7be-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e7be-137">DateTimeOffset</span></span>|<span data-ttu-id="6e7be-138">Data de validade do perfil opcional e hora.</span><span class="sxs-lookup"><span data-stu-id="6e7be-138">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="6e7be-139">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="6e7be-139">payloadFileName</span></span>|<span data-ttu-id="6e7be-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e7be-140">String</span></span>|<span data-ttu-id="6e7be-141">Nome do arquivo de carga (\*.mobileprovision</span><span class="sxs-lookup"><span data-stu-id="6e7be-141">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="6e7be-142">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="6e7be-142">\*.xml).</span></span>|
|<span data-ttu-id="6e7be-143">payload</span><span class="sxs-lookup"><span data-stu-id="6e7be-143">payload</span></span>|<span data-ttu-id="6e7be-144">Binária</span><span class="sxs-lookup"><span data-stu-id="6e7be-144">Binary</span></span>|<span data-ttu-id="6e7be-145">Carga.</span><span class="sxs-lookup"><span data-stu-id="6e7be-145">Payload.</span></span> <span data-ttu-id="6e7be-146">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="6e7be-146">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="6e7be-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e7be-147">createdDateTime</span></span>|<span data-ttu-id="6e7be-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e7be-148">DateTimeOffset</span></span>|<span data-ttu-id="6e7be-149">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6e7be-149">DateTime the object was created.</span></span>|
|<span data-ttu-id="6e7be-150">description</span><span class="sxs-lookup"><span data-stu-id="6e7be-150">description</span></span>|<span data-ttu-id="6e7be-151">String</span><span class="sxs-lookup"><span data-stu-id="6e7be-151">String</span></span>|<span data-ttu-id="6e7be-152">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6e7be-152">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="6e7be-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e7be-153">lastModifiedDateTime</span></span>|<span data-ttu-id="6e7be-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e7be-154">DateTimeOffset</span></span>|<span data-ttu-id="6e7be-155">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6e7be-155">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="6e7be-156">displayName</span><span class="sxs-lookup"><span data-stu-id="6e7be-156">displayName</span></span>|<span data-ttu-id="6e7be-157">String</span><span class="sxs-lookup"><span data-stu-id="6e7be-157">String</span></span>|<span data-ttu-id="6e7be-158">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6e7be-158">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="6e7be-159">version</span><span class="sxs-lookup"><span data-stu-id="6e7be-159">version</span></span>|<span data-ttu-id="6e7be-160">Int32</span><span class="sxs-lookup"><span data-stu-id="6e7be-160">Int32</span></span>|<span data-ttu-id="6e7be-161">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6e7be-161">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="6e7be-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e7be-162">Response</span></span>
<span data-ttu-id="6e7be-163">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e7be-163">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e7be-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e7be-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e7be-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e7be-165">Request</span></span>
<span data-ttu-id="6e7be-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e7be-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6e7be-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e7be-167">Response</span></span>
<span data-ttu-id="6e7be-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e7be-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




