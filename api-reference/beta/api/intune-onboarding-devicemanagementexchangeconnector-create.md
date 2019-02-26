---
title: Criar deviceManagementExchangeConnector
description: Crie um novo objeto deviceManagementExchangeConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4aee6dbffccf6ed486e11103ec1d211e8c314ec
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164208"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="c4ed1-103">Criar deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="c4ed1-103">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="c4ed1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4ed1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4ed1-106">Crie um novo objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="c4ed1-106">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4ed1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4ed1-107">Prerequisites</span></span>
<span data-ttu-id="c4ed1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c4ed1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c4ed1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4ed1-110">Permission type</span></span>|<span data-ttu-id="c4ed1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c4ed1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4ed1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4ed1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c4ed1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4ed1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c4ed1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4ed1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4ed1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-115">Not supported.</span></span>|
|<span data-ttu-id="c4ed1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4ed1-116">Application</span></span>|<span data-ttu-id="c4ed1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4ed1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4ed1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="c4ed1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4ed1-119">Request headers</span></span>
|<span data-ttu-id="c4ed1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4ed1-120">Header</span></span>|<span data-ttu-id="c4ed1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c4ed1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4ed1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4ed1-122">Authorization</span></span>|<span data-ttu-id="c4ed1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4ed1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c4ed1-124">Accept</span></span>|<span data-ttu-id="c4ed1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c4ed1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4ed1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4ed1-126">Request body</span></span>
<span data-ttu-id="c4ed1-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-127">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="c4ed1-128">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-128">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="c4ed1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4ed1-129">Property</span></span>|<span data-ttu-id="c4ed1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4ed1-130">Type</span></span>|<span data-ttu-id="c4ed1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4ed1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4ed1-132">id</span><span class="sxs-lookup"><span data-stu-id="c4ed1-132">id</span></span>|<span data-ttu-id="c4ed1-133">String</span><span class="sxs-lookup"><span data-stu-id="c4ed1-133">String</span></span>|<span data-ttu-id="c4ed1-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c4ed1-134">Not yet documented</span></span>|
|<span data-ttu-id="c4ed1-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c4ed1-135">lastSyncDateTime</span></span>|<span data-ttu-id="c4ed1-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4ed1-136">DateTimeOffset</span></span>|<span data-ttu-id="c4ed1-137">Hora da última sincronização do Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="c4ed1-137">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="c4ed1-138">status</span><span class="sxs-lookup"><span data-stu-id="c4ed1-138">status</span></span>|[<span data-ttu-id="c4ed1-139">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="c4ed1-139">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="c4ed1-140">Status do Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-140">Exchange Connector Status.</span></span> <span data-ttu-id="c4ed1-141">Os valores possíveis são: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-141">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="c4ed1-142">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="c4ed1-142">primarySmtpAddress</span></span>|<span data-ttu-id="c4ed1-143">String</span><span class="sxs-lookup"><span data-stu-id="c4ed1-143">String</span></span>|<span data-ttu-id="c4ed1-144">Endereço de email usado para configurar o serviço a serviço do Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-144">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="c4ed1-145">serverName</span><span class="sxs-lookup"><span data-stu-id="c4ed1-145">serverName</span></span>|<span data-ttu-id="c4ed1-146">String</span><span class="sxs-lookup"><span data-stu-id="c4ed1-146">String</span></span>|<span data-ttu-id="c4ed1-147">O nome do servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-147">The name of the Exchange server.</span></span>|
|<span data-ttu-id="c4ed1-148">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="c4ed1-148">connectorServerName</span></span>|<span data-ttu-id="c4ed1-149">String</span><span class="sxs-lookup"><span data-stu-id="c4ed1-149">String</span></span>|<span data-ttu-id="c4ed1-150">O nome do servidor que hospeda o Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-150">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="c4ed1-151">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="c4ed1-151">exchangeConnectorType</span></span>|[<span data-ttu-id="c4ed1-152">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="c4ed1-152">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="c4ed1-153">O tipo de Exchange Connector configurado.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-153">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="c4ed1-154">Os valores possíveis são: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-154">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="c4ed1-155">version</span><span class="sxs-lookup"><span data-stu-id="c4ed1-155">version</span></span>|<span data-ttu-id="c4ed1-156">String</span><span class="sxs-lookup"><span data-stu-id="c4ed1-156">String</span></span>|<span data-ttu-id="c4ed1-157">A versão do ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="c4ed1-157">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="c4ed1-158">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="c4ed1-158">exchangeAlias</span></span>|<span data-ttu-id="c4ed1-159">String</span><span class="sxs-lookup"><span data-stu-id="c4ed1-159">String</span></span>|<span data-ttu-id="c4ed1-160">Um alias atribuído a um servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="c4ed1-160">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="c4ed1-161">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="c4ed1-161">exchangeOrganization</span></span>|<span data-ttu-id="c4ed1-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4ed1-162">String</span></span>|<span data-ttu-id="c4ed1-163">Organização do Exchange no servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="c4ed1-163">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="c4ed1-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4ed1-164">Response</span></span>
<span data-ttu-id="c4ed1-165">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-165">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4ed1-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4ed1-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4ed1-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4ed1-167">Request</span></span>
<span data-ttu-id="c4ed1-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c4ed1-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4ed1-169">Response</span></span>
<span data-ttu-id="c4ed1-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4ed1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




