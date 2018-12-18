---
title: Criar iosLobAppProvisioningConfiguration
description: Crie um novo objeto de iosLobAppProvisioningConfiguration.
author: tfitzmac
ms.openlocfilehash: 80d6b607d514758942ccd5f8334315fd62c0270a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333646"
---
# <a name="create-ioslobappprovisioningconfiguration"></a><span data-ttu-id="a8ac4-103">Criar iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8ac4-103">Create iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="a8ac4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a8ac4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8ac4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a8ac4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8ac4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a8ac4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8ac4-107">Crie um novo objeto de [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a8ac4-107">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a8ac4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a8ac4-108">Prerequisites</span></span>
<span data-ttu-id="a8ac4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8ac4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8ac4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8ac4-111">Permission type</span></span>|<span data-ttu-id="a8ac4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a8ac4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8ac4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8ac4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8ac4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8ac4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a8ac4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8ac4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8ac4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8ac4-116">Not supported.</span></span>|
|<span data-ttu-id="a8ac4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8ac4-117">Application</span></span>|<span data-ttu-id="a8ac4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8ac4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8ac4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8ac4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a8ac4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8ac4-120">Request headers</span></span>
|<span data-ttu-id="a8ac4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8ac4-121">Header</span></span>|<span data-ttu-id="a8ac4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a8ac4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8ac4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8ac4-123">Authorization</span></span>|<span data-ttu-id="a8ac4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8ac4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8ac4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a8ac4-125">Accept</span></span>|<span data-ttu-id="a8ac4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8ac4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8ac4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8ac4-127">Request body</span></span>
<span data-ttu-id="a8ac4-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosLobAppProvisioningConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a8ac4-128">In the request body, supply a JSON representation for the iosLobAppProvisioningConfiguration object.</span></span>

<span data-ttu-id="a8ac4-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o iosLobAppProvisioningConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a8ac4-129">The following table shows the properties that are required when you create the iosLobAppProvisioningConfiguration.</span></span>

|<span data-ttu-id="a8ac4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8ac4-130">Property</span></span>|<span data-ttu-id="a8ac4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8ac4-131">Type</span></span>|<span data-ttu-id="a8ac4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8ac4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8ac4-133">id</span><span class="sxs-lookup"><span data-stu-id="a8ac4-133">id</span></span>|<span data-ttu-id="a8ac4-134">String</span><span class="sxs-lookup"><span data-stu-id="a8ac4-134">String</span></span>|<span data-ttu-id="a8ac4-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a8ac4-135">Key of the entity.</span></span>|
|<span data-ttu-id="a8ac4-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a8ac4-136">expirationDateTime</span></span>|<span data-ttu-id="a8ac4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8ac4-137">DateTimeOffset</span></span>|<span data-ttu-id="a8ac4-138">Data de validade do perfil opcional e hora.</span><span class="sxs-lookup"><span data-stu-id="a8ac4-138">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="a8ac4-139">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="a8ac4-139">payloadFileName</span></span>|<span data-ttu-id="a8ac4-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8ac4-140">String</span></span>|<span data-ttu-id="a8ac4-141">Nome do arquivo de carga (\*.mobileprovision</span><span class="sxs-lookup"><span data-stu-id="a8ac4-141">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="a8ac4-142">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="a8ac4-142">\*.xml).</span></span>|
|<span data-ttu-id="a8ac4-143">payload</span><span class="sxs-lookup"><span data-stu-id="a8ac4-143">payload</span></span>|<span data-ttu-id="a8ac4-144">Binária</span><span class="sxs-lookup"><span data-stu-id="a8ac4-144">Binary</span></span>|<span data-ttu-id="a8ac4-145">Carga.</span><span class="sxs-lookup"><span data-stu-id="a8ac4-145">Payload.</span></span> <span data-ttu-id="a8ac4-146">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="a8ac4-146">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="a8ac4-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8ac4-147">createdDateTime</span></span>|<span data-ttu-id="a8ac4-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8ac4-148">DateTimeOffset</span></span>|<span data-ttu-id="a8ac4-149">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a8ac4-149">DateTime the object was created.</span></span>|
|<span data-ttu-id="a8ac4-150">description</span><span class="sxs-lookup"><span data-stu-id="a8ac4-150">description</span></span>|<span data-ttu-id="a8ac4-151">String</span><span class="sxs-lookup"><span data-stu-id="a8ac4-151">String</span></span>|<span data-ttu-id="a8ac4-152">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a8ac4-152">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="a8ac4-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8ac4-153">lastModifiedDateTime</span></span>|<span data-ttu-id="a8ac4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8ac4-154">DateTimeOffset</span></span>|<span data-ttu-id="a8ac4-155">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a8ac4-155">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="a8ac4-156">displayName</span><span class="sxs-lookup"><span data-stu-id="a8ac4-156">displayName</span></span>|<span data-ttu-id="a8ac4-157">String</span><span class="sxs-lookup"><span data-stu-id="a8ac4-157">String</span></span>|<span data-ttu-id="a8ac4-158">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a8ac4-158">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="a8ac4-159">version</span><span class="sxs-lookup"><span data-stu-id="a8ac4-159">version</span></span>|<span data-ttu-id="a8ac4-160">Int32</span><span class="sxs-lookup"><span data-stu-id="a8ac4-160">Int32</span></span>|<span data-ttu-id="a8ac4-161">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a8ac4-161">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="a8ac4-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8ac4-162">Response</span></span>
<span data-ttu-id="a8ac4-163">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8ac4-163">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8ac4-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8ac4-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="a8ac4-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8ac4-165">Request</span></span>
<span data-ttu-id="a8ac4-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8ac4-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations
Content-type: application/json
Content-length: 377

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="a8ac4-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8ac4-167">Response</span></span>
<span data-ttu-id="a8ac4-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8ac4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





