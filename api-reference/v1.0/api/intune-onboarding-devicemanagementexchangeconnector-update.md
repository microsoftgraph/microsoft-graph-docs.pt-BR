---
title: Atualizar deviceManagementExchangeConnector
description: Atualizar as propriedades de um objeto deviceManagementExchangeConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4d19f4ecd790b4edf712f878c19ae3998c1f217d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935035"
---
# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="abc4f-103">Atualizar deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="abc4f-103">Update deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="abc4f-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="abc4f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abc4f-105">Atualizar as propriedades de um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="abc4f-105">Update the properties of a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="abc4f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="abc4f-106">Prerequisites</span></span>
<span data-ttu-id="abc4f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abc4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abc4f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abc4f-109">Permission type</span></span>|<span data-ttu-id="abc4f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="abc4f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abc4f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abc4f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="abc4f-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abc4f-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="abc4f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abc4f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abc4f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abc4f-114">Not supported.</span></span>|
|<span data-ttu-id="abc4f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="abc4f-115">Application</span></span>|<span data-ttu-id="abc4f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abc4f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abc4f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abc4f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="abc4f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abc4f-118">Request headers</span></span>
|<span data-ttu-id="abc4f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="abc4f-119">Header</span></span>|<span data-ttu-id="abc4f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="abc4f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abc4f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="abc4f-121">Authorization</span></span>|<span data-ttu-id="abc4f-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abc4f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abc4f-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="abc4f-123">Accept</span></span>|<span data-ttu-id="abc4f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="abc4f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abc4f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abc4f-125">Request body</span></span>
<span data-ttu-id="abc4f-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="abc4f-126">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="abc4f-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="abc4f-127">The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>

|<span data-ttu-id="abc4f-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abc4f-128">Property</span></span>|<span data-ttu-id="abc4f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="abc4f-129">Type</span></span>|<span data-ttu-id="abc4f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="abc4f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abc4f-131">id</span><span class="sxs-lookup"><span data-stu-id="abc4f-131">id</span></span>|<span data-ttu-id="abc4f-132">String</span><span class="sxs-lookup"><span data-stu-id="abc4f-132">String</span></span>|<span data-ttu-id="abc4f-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="abc4f-133">Not yet documented</span></span>|
|<span data-ttu-id="abc4f-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="abc4f-134">lastSyncDateTime</span></span>|<span data-ttu-id="abc4f-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abc4f-135">DateTimeOffset</span></span>|<span data-ttu-id="abc4f-136">Hora da última sincronização do Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="abc4f-136">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="abc4f-137">status</span><span class="sxs-lookup"><span data-stu-id="abc4f-137">status</span></span>|[<span data-ttu-id="abc4f-138">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="abc4f-138">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="abc4f-139">Status de conector do Exchange.</span><span class="sxs-lookup"><span data-stu-id="abc4f-139">Exchange Connector Status.</span></span> <span data-ttu-id="abc4f-140">Os valores possíveis são: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="abc4f-140">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="abc4f-141">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="abc4f-141">primarySmtpAddress</span></span>|<span data-ttu-id="abc4f-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abc4f-142">String</span></span>|<span data-ttu-id="abc4f-143">Endereço de email usado para configurar o serviço a serviço do Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="abc4f-143">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="abc4f-144">serverName</span><span class="sxs-lookup"><span data-stu-id="abc4f-144">serverName</span></span>|<span data-ttu-id="abc4f-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abc4f-145">String</span></span>|<span data-ttu-id="abc4f-146">O nome do servidor do Exchange.</span><span class="sxs-lookup"><span data-stu-id="abc4f-146">The name of the Exchange server.</span></span>|
|<span data-ttu-id="abc4f-147">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="abc4f-147">connectorServerName</span></span>|<span data-ttu-id="abc4f-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abc4f-148">String</span></span>|<span data-ttu-id="abc4f-149">O nome do servidor que hospeda o Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="abc4f-149">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="abc4f-150">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="abc4f-150">exchangeConnectorType</span></span>|[<span data-ttu-id="abc4f-151">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="abc4f-151">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="abc4f-152">O tipo de Exchange Connector configurado.</span><span class="sxs-lookup"><span data-stu-id="abc4f-152">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="abc4f-153">Os valores possíveis são: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="abc4f-153">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="abc4f-154">version</span><span class="sxs-lookup"><span data-stu-id="abc4f-154">version</span></span>|<span data-ttu-id="abc4f-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abc4f-155">String</span></span>|<span data-ttu-id="abc4f-156">A versão do ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="abc4f-156">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="abc4f-157">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="abc4f-157">exchangeAlias</span></span>|<span data-ttu-id="abc4f-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abc4f-158">String</span></span>|<span data-ttu-id="abc4f-159">Um alias atribuído a um servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="abc4f-159">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="abc4f-160">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="abc4f-160">exchangeOrganization</span></span>|<span data-ttu-id="abc4f-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abc4f-161">String</span></span>|<span data-ttu-id="abc4f-162">Organização do Exchange no servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="abc4f-162">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="abc4f-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="abc4f-163">Response</span></span>
<span data-ttu-id="abc4f-164">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abc4f-164">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abc4f-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abc4f-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="abc4f-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abc4f-166">Request</span></span>
<span data-ttu-id="abc4f-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abc4f-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
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

### <a name="response"></a><span data-ttu-id="abc4f-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="abc4f-168">Response</span></span>
<span data-ttu-id="abc4f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="abc4f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



