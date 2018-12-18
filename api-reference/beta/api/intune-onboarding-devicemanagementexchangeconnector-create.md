---
title: Criar deviceManagementExchangeConnector
description: Crie um novo objeto deviceManagementExchangeConnector.
author: tfitzmac
ms.openlocfilehash: 04794c97edef8495f2132cf556680678a5b63edf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348192"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="01285-103">Criar deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="01285-103">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="01285-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="01285-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01285-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="01285-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01285-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="01285-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01285-107">Crie um novo objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="01285-107">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="01285-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="01285-108">Prerequisites</span></span>
<span data-ttu-id="01285-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01285-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01285-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01285-111">Permission type</span></span>|<span data-ttu-id="01285-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="01285-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01285-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01285-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01285-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01285-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="01285-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01285-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01285-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01285-116">Not supported.</span></span>|
|<span data-ttu-id="01285-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01285-117">Application</span></span>|<span data-ttu-id="01285-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01285-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01285-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01285-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="01285-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01285-120">Request headers</span></span>
|<span data-ttu-id="01285-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01285-121">Header</span></span>|<span data-ttu-id="01285-122">Valor</span><span class="sxs-lookup"><span data-stu-id="01285-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01285-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="01285-123">Authorization</span></span>|<span data-ttu-id="01285-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01285-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01285-125">Accept</span><span class="sxs-lookup"><span data-stu-id="01285-125">Accept</span></span>|<span data-ttu-id="01285-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01285-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01285-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01285-127">Request body</span></span>
<span data-ttu-id="01285-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="01285-128">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="01285-129">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="01285-129">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="01285-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01285-130">Property</span></span>|<span data-ttu-id="01285-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="01285-131">Type</span></span>|<span data-ttu-id="01285-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="01285-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01285-133">id</span><span class="sxs-lookup"><span data-stu-id="01285-133">id</span></span>|<span data-ttu-id="01285-134">String</span><span class="sxs-lookup"><span data-stu-id="01285-134">String</span></span>|<span data-ttu-id="01285-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="01285-135">Not yet documented</span></span>|
|<span data-ttu-id="01285-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="01285-136">lastSyncDateTime</span></span>|<span data-ttu-id="01285-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01285-137">DateTimeOffset</span></span>|<span data-ttu-id="01285-138">Hora da última sincronização do Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="01285-138">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="01285-139">status</span><span class="sxs-lookup"><span data-stu-id="01285-139">status</span></span>|[<span data-ttu-id="01285-140">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="01285-140">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="01285-141">Status de conector do Exchange.</span><span class="sxs-lookup"><span data-stu-id="01285-141">Exchange Connector Status.</span></span> <span data-ttu-id="01285-142">Os valores possíveis são: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="01285-142">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="01285-143">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="01285-143">primarySmtpAddress</span></span>|<span data-ttu-id="01285-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01285-144">String</span></span>|<span data-ttu-id="01285-145">Endereço de email usado para configurar o serviço a serviço do Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="01285-145">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="01285-146">serverName</span><span class="sxs-lookup"><span data-stu-id="01285-146">serverName</span></span>|<span data-ttu-id="01285-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01285-147">String</span></span>|<span data-ttu-id="01285-148">O nome do servidor do Exchange.</span><span class="sxs-lookup"><span data-stu-id="01285-148">The name of the Exchange server.</span></span>|
|<span data-ttu-id="01285-149">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="01285-149">connectorServerName</span></span>|<span data-ttu-id="01285-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01285-150">String</span></span>|<span data-ttu-id="01285-151">O nome do servidor que hospeda o Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="01285-151">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="01285-152">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="01285-152">exchangeConnectorType</span></span>|[<span data-ttu-id="01285-153">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="01285-153">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="01285-154">O tipo de Exchange Connector configurado.</span><span class="sxs-lookup"><span data-stu-id="01285-154">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="01285-155">Os valores possíveis são: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="01285-155">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="01285-156">version</span><span class="sxs-lookup"><span data-stu-id="01285-156">version</span></span>|<span data-ttu-id="01285-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01285-157">String</span></span>|<span data-ttu-id="01285-158">A versão do ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="01285-158">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="01285-159">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="01285-159">exchangeAlias</span></span>|<span data-ttu-id="01285-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01285-160">String</span></span>|<span data-ttu-id="01285-161">Um alias atribuído a um servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="01285-161">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="01285-162">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="01285-162">exchangeOrganization</span></span>|<span data-ttu-id="01285-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01285-163">String</span></span>|<span data-ttu-id="01285-164">Organização do Exchange no servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="01285-164">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="01285-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="01285-165">Response</span></span>
<span data-ttu-id="01285-166">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01285-166">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01285-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01285-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="01285-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01285-168">Request</span></span>
<span data-ttu-id="01285-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01285-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="01285-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="01285-170">Response</span></span>
<span data-ttu-id="01285-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01285-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





