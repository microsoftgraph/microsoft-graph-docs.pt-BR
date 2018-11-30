---
title: Criar deviceManagementExchangeConnector
description: Crie um novo objeto deviceManagementExchangeConnector.
ms.openlocfilehash: 710f2a1d43f95a8a3ca6f6f154a667b78e8c0795
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004024"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="940aa-103">Criar deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="940aa-103">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="940aa-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="940aa-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="940aa-105">Crie um novo objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="940aa-105">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="940aa-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="940aa-106">Prerequisites</span></span>
<span data-ttu-id="940aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="940aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="940aa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="940aa-109">Permission type</span></span>|<span data-ttu-id="940aa-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="940aa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="940aa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="940aa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="940aa-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="940aa-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="940aa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="940aa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="940aa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="940aa-114">Not supported.</span></span>|
|<span data-ttu-id="940aa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="940aa-115">Application</span></span>|<span data-ttu-id="940aa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="940aa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="940aa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="940aa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="940aa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="940aa-118">Request headers</span></span>
|<span data-ttu-id="940aa-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="940aa-119">Header</span></span>|<span data-ttu-id="940aa-120">Valor</span><span class="sxs-lookup"><span data-stu-id="940aa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="940aa-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="940aa-121">Authorization</span></span>|<span data-ttu-id="940aa-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="940aa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="940aa-123">Accept</span><span class="sxs-lookup"><span data-stu-id="940aa-123">Accept</span></span>|<span data-ttu-id="940aa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="940aa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="940aa-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="940aa-125">Request body</span></span>
<span data-ttu-id="940aa-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="940aa-126">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="940aa-127">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="940aa-127">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="940aa-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="940aa-128">Property</span></span>|<span data-ttu-id="940aa-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="940aa-129">Type</span></span>|<span data-ttu-id="940aa-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="940aa-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="940aa-131">id</span><span class="sxs-lookup"><span data-stu-id="940aa-131">id</span></span>|<span data-ttu-id="940aa-132">String</span><span class="sxs-lookup"><span data-stu-id="940aa-132">String</span></span>|<span data-ttu-id="940aa-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="940aa-133">Not yet documented</span></span>|
|<span data-ttu-id="940aa-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="940aa-134">lastSyncDateTime</span></span>|<span data-ttu-id="940aa-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="940aa-135">DateTimeOffset</span></span>|<span data-ttu-id="940aa-136">Hora da última sincronização do Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="940aa-136">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="940aa-137">status</span><span class="sxs-lookup"><span data-stu-id="940aa-137">status</span></span>|[<span data-ttu-id="940aa-138">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="940aa-138">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="940aa-139">Status de conector do Exchange.</span><span class="sxs-lookup"><span data-stu-id="940aa-139">Exchange Connector Status.</span></span> <span data-ttu-id="940aa-140">Os valores possíveis são: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="940aa-140">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="940aa-141">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="940aa-141">primarySmtpAddress</span></span>|<span data-ttu-id="940aa-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="940aa-142">String</span></span>|<span data-ttu-id="940aa-143">Endereço de email usado para configurar o serviço a serviço do Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="940aa-143">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="940aa-144">serverName</span><span class="sxs-lookup"><span data-stu-id="940aa-144">serverName</span></span>|<span data-ttu-id="940aa-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="940aa-145">String</span></span>|<span data-ttu-id="940aa-146">O nome do servidor do Exchange.</span><span class="sxs-lookup"><span data-stu-id="940aa-146">The name of the Exchange server.</span></span>|
|<span data-ttu-id="940aa-147">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="940aa-147">connectorServerName</span></span>|<span data-ttu-id="940aa-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="940aa-148">String</span></span>|<span data-ttu-id="940aa-149">O nome do servidor que hospeda o Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="940aa-149">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="940aa-150">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="940aa-150">exchangeConnectorType</span></span>|[<span data-ttu-id="940aa-151">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="940aa-151">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="940aa-152">O tipo de Exchange Connector configurado.</span><span class="sxs-lookup"><span data-stu-id="940aa-152">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="940aa-153">Os valores possíveis são: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="940aa-153">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="940aa-154">version</span><span class="sxs-lookup"><span data-stu-id="940aa-154">version</span></span>|<span data-ttu-id="940aa-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="940aa-155">String</span></span>|<span data-ttu-id="940aa-156">A versão do ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="940aa-156">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="940aa-157">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="940aa-157">exchangeAlias</span></span>|<span data-ttu-id="940aa-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="940aa-158">String</span></span>|<span data-ttu-id="940aa-159">Um alias atribuído a um servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="940aa-159">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="940aa-160">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="940aa-160">exchangeOrganization</span></span>|<span data-ttu-id="940aa-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="940aa-161">String</span></span>|<span data-ttu-id="940aa-162">Organização do Exchange no servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="940aa-162">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="940aa-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="940aa-163">Response</span></span>
<span data-ttu-id="940aa-164">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="940aa-164">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="940aa-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="940aa-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="940aa-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="940aa-166">Request</span></span>
<span data-ttu-id="940aa-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="940aa-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
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

### <a name="response"></a><span data-ttu-id="940aa-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="940aa-168">Response</span></span>
<span data-ttu-id="940aa-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="940aa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



