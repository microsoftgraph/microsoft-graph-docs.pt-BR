---
title: Criar deviceManagementExchangeConnector
description: Crie um novo objeto deviceManagementExchangeConnector.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2226d76903612062e97ec382bd67be1fc253c6d7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33900174"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="51ee8-103">Criar deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="51ee8-103">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="51ee8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="51ee8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51ee8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="51ee8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51ee8-106">Crie um novo objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="51ee8-106">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51ee8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51ee8-107">Prerequisites</span></span>
<span data-ttu-id="51ee8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51ee8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51ee8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51ee8-110">Permission type</span></span>|<span data-ttu-id="51ee8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="51ee8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51ee8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51ee8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51ee8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51ee8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="51ee8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51ee8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51ee8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51ee8-115">Not supported.</span></span>|
|<span data-ttu-id="51ee8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51ee8-116">Application</span></span>|<span data-ttu-id="51ee8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51ee8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51ee8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51ee8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="51ee8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51ee8-119">Request headers</span></span>
|<span data-ttu-id="51ee8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51ee8-120">Header</span></span>|<span data-ttu-id="51ee8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="51ee8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51ee8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="51ee8-122">Authorization</span></span>|<span data-ttu-id="51ee8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51ee8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51ee8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="51ee8-124">Accept</span></span>|<span data-ttu-id="51ee8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="51ee8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51ee8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51ee8-126">Request body</span></span>
<span data-ttu-id="51ee8-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="51ee8-127">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="51ee8-128">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="51ee8-128">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="51ee8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51ee8-129">Property</span></span>|<span data-ttu-id="51ee8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="51ee8-130">Type</span></span>|<span data-ttu-id="51ee8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="51ee8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51ee8-132">id</span><span class="sxs-lookup"><span data-stu-id="51ee8-132">id</span></span>|<span data-ttu-id="51ee8-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51ee8-133">String</span></span>|<span data-ttu-id="51ee8-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="51ee8-134">Not yet documented</span></span>|
|<span data-ttu-id="51ee8-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="51ee8-135">lastSyncDateTime</span></span>|<span data-ttu-id="51ee8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51ee8-136">DateTimeOffset</span></span>|<span data-ttu-id="51ee8-137">Hora da última sincronização do Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="51ee8-137">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="51ee8-138">status</span><span class="sxs-lookup"><span data-stu-id="51ee8-138">status</span></span>|[<span data-ttu-id="51ee8-139">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="51ee8-139">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="51ee8-140">Status do Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="51ee8-140">Exchange Connector Status.</span></span> <span data-ttu-id="51ee8-141">Os valores possíveis são: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="51ee8-141">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="51ee8-142">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="51ee8-142">primarySmtpAddress</span></span>|<span data-ttu-id="51ee8-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51ee8-143">String</span></span>|<span data-ttu-id="51ee8-144">Endereço de email usado para configurar o serviço a serviço do Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="51ee8-144">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="51ee8-145">serverName</span><span class="sxs-lookup"><span data-stu-id="51ee8-145">serverName</span></span>|<span data-ttu-id="51ee8-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51ee8-146">String</span></span>|<span data-ttu-id="51ee8-147">O nome do servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="51ee8-147">The name of the Exchange server.</span></span>|
|<span data-ttu-id="51ee8-148">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="51ee8-148">connectorServerName</span></span>|<span data-ttu-id="51ee8-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51ee8-149">String</span></span>|<span data-ttu-id="51ee8-150">O nome do servidor que hospeda o Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="51ee8-150">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="51ee8-151">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="51ee8-151">exchangeConnectorType</span></span>|[<span data-ttu-id="51ee8-152">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="51ee8-152">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="51ee8-153">O tipo de Exchange Connector configurado.</span><span class="sxs-lookup"><span data-stu-id="51ee8-153">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="51ee8-154">Os valores possíveis são: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="51ee8-154">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="51ee8-155">versão</span><span class="sxs-lookup"><span data-stu-id="51ee8-155">version</span></span>|<span data-ttu-id="51ee8-156">String</span><span class="sxs-lookup"><span data-stu-id="51ee8-156">String</span></span>|<span data-ttu-id="51ee8-157">A versão do ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="51ee8-157">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="51ee8-158">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="51ee8-158">exchangeAlias</span></span>|<span data-ttu-id="51ee8-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51ee8-159">String</span></span>|<span data-ttu-id="51ee8-160">Um alias atribuído a um servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="51ee8-160">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="51ee8-161">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="51ee8-161">exchangeOrganization</span></span>|<span data-ttu-id="51ee8-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51ee8-162">String</span></span>|<span data-ttu-id="51ee8-163">Organização do Exchange no servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="51ee8-163">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="51ee8-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="51ee8-164">Response</span></span>
<span data-ttu-id="51ee8-165">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51ee8-165">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51ee8-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51ee8-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="51ee8-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51ee8-167">Request</span></span>
<span data-ttu-id="51ee8-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51ee8-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors
Content-type: application/json
Content-length: 490

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

### <a name="response"></a><span data-ttu-id="51ee8-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="51ee8-169">Response</span></span>
<span data-ttu-id="51ee8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51ee8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```




