---
title: Atualizar deviceManagementExchangeConnector
description: Atualizar as propriedades de um objeto deviceManagementExchangeConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 990a78d6c50e1c6669ee900a5155b919381c459f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156930"
---
# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="f6720-103">Atualizar deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="f6720-103">Update deviceManagementExchangeConnector</span></span>

<span data-ttu-id="f6720-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6720-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6720-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f6720-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6720-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f6720-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6720-107">Atualizar as propriedades de um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="f6720-107">Update the properties of a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6720-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f6720-108">Prerequisites</span></span>
<span data-ttu-id="f6720-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6720-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6720-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6720-111">Permission type</span></span>|<span data-ttu-id="f6720-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f6720-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6720-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6720-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6720-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6720-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f6720-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6720-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6720-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6720-116">Not supported.</span></span>|
|<span data-ttu-id="f6720-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6720-117">Application</span></span>|<span data-ttu-id="f6720-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6720-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6720-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6720-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="f6720-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6720-120">Request headers</span></span>
|<span data-ttu-id="f6720-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f6720-121">Header</span></span>|<span data-ttu-id="f6720-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f6720-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6720-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6720-123">Authorization</span></span>|<span data-ttu-id="f6720-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6720-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6720-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f6720-125">Accept</span></span>|<span data-ttu-id="f6720-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6720-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6720-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6720-127">Request body</span></span>
<span data-ttu-id="f6720-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="f6720-128">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="f6720-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="f6720-129">The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>

|<span data-ttu-id="f6720-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6720-130">Property</span></span>|<span data-ttu-id="f6720-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6720-131">Type</span></span>|<span data-ttu-id="f6720-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6720-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6720-133">id</span><span class="sxs-lookup"><span data-stu-id="f6720-133">id</span></span>|<span data-ttu-id="f6720-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6720-134">String</span></span>|<span data-ttu-id="f6720-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f6720-135">Not yet documented</span></span>|
|<span data-ttu-id="f6720-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f6720-136">lastSyncDateTime</span></span>|<span data-ttu-id="f6720-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6720-137">DateTimeOffset</span></span>|<span data-ttu-id="f6720-138">Hora da última sincronização do Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="f6720-138">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="f6720-139">status</span><span class="sxs-lookup"><span data-stu-id="f6720-139">status</span></span>|[<span data-ttu-id="f6720-140">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="f6720-140">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="f6720-141">Status do Conector do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6720-141">Exchange Connector Status.</span></span> <span data-ttu-id="f6720-142">Os valores possíveis são: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="f6720-142">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="f6720-143">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="f6720-143">primarySmtpAddress</span></span>|<span data-ttu-id="f6720-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6720-144">String</span></span>|<span data-ttu-id="f6720-145">Endereço de email usado para configurar o serviço a serviço do Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="f6720-145">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="f6720-146">serverName</span><span class="sxs-lookup"><span data-stu-id="f6720-146">serverName</span></span>|<span data-ttu-id="f6720-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6720-147">String</span></span>|<span data-ttu-id="f6720-148">O nome do servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6720-148">The name of the Exchange server.</span></span>|
|<span data-ttu-id="f6720-149">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="f6720-149">connectorServerName</span></span>|<span data-ttu-id="f6720-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6720-150">String</span></span>|<span data-ttu-id="f6720-151">O nome do servidor que hospeda o Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="f6720-151">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="f6720-152">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="f6720-152">exchangeConnectorType</span></span>|[<span data-ttu-id="f6720-153">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="f6720-153">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="f6720-154">O tipo de Exchange Connector configurado.</span><span class="sxs-lookup"><span data-stu-id="f6720-154">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="f6720-155">Os valores possíveis são: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="f6720-155">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="f6720-156">versão</span><span class="sxs-lookup"><span data-stu-id="f6720-156">version</span></span>|<span data-ttu-id="f6720-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6720-157">String</span></span>|<span data-ttu-id="f6720-158">A versão do ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="f6720-158">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="f6720-159">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="f6720-159">exchangeAlias</span></span>|<span data-ttu-id="f6720-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6720-160">String</span></span>|<span data-ttu-id="f6720-161">Um alias atribuído a um servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="f6720-161">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="f6720-162">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="f6720-162">exchangeOrganization</span></span>|<span data-ttu-id="f6720-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6720-163">String</span></span>|<span data-ttu-id="f6720-164">Organização do Exchange no servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="f6720-164">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="f6720-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6720-165">Response</span></span>
<span data-ttu-id="f6720-166">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6720-166">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6720-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6720-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6720-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6720-168">Request</span></span>
<span data-ttu-id="f6720-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6720-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
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

### <a name="response"></a><span data-ttu-id="f6720-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6720-170">Response</span></span>
<span data-ttu-id="f6720-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f6720-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




