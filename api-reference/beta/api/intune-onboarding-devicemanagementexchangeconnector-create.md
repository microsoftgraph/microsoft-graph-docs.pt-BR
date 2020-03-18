---
title: Criar deviceManagementExchangeConnector
description: Crie um novo objeto deviceManagementExchangeConnector.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7fe5f294f77d18e11197cc312397df8c46a5bac5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802934"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="9994a-103">Criar deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="9994a-103">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="9994a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9994a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9994a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9994a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9994a-106">Crie um novo objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="9994a-106">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9994a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9994a-107">Prerequisites</span></span>
<span data-ttu-id="9994a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9994a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9994a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9994a-110">Permission type</span></span>|<span data-ttu-id="9994a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9994a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9994a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9994a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9994a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9994a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9994a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9994a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9994a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9994a-115">Not supported.</span></span>|
|<span data-ttu-id="9994a-116">Application</span><span class="sxs-lookup"><span data-stu-id="9994a-116">Application</span></span>|<span data-ttu-id="9994a-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9994a-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9994a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9994a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="9994a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9994a-119">Request headers</span></span>
|<span data-ttu-id="9994a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9994a-120">Header</span></span>|<span data-ttu-id="9994a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9994a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9994a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9994a-122">Authorization</span></span>|<span data-ttu-id="9994a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9994a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9994a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9994a-124">Accept</span></span>|<span data-ttu-id="9994a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9994a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9994a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9994a-126">Request body</span></span>
<span data-ttu-id="9994a-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="9994a-127">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="9994a-128">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="9994a-128">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="9994a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9994a-129">Property</span></span>|<span data-ttu-id="9994a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9994a-130">Type</span></span>|<span data-ttu-id="9994a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9994a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9994a-132">id</span><span class="sxs-lookup"><span data-stu-id="9994a-132">id</span></span>|<span data-ttu-id="9994a-133">String</span><span class="sxs-lookup"><span data-stu-id="9994a-133">String</span></span>|<span data-ttu-id="9994a-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9994a-134">Not yet documented</span></span>|
|<span data-ttu-id="9994a-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9994a-135">lastSyncDateTime</span></span>|<span data-ttu-id="9994a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9994a-136">DateTimeOffset</span></span>|<span data-ttu-id="9994a-137">Hora da última sincronização do Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="9994a-137">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="9994a-138">status</span><span class="sxs-lookup"><span data-stu-id="9994a-138">status</span></span>|[<span data-ttu-id="9994a-139">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="9994a-139">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="9994a-140">Status do Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="9994a-140">Exchange Connector Status.</span></span> <span data-ttu-id="9994a-141">Os valores possíveis são: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="9994a-141">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="9994a-142">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="9994a-142">primarySmtpAddress</span></span>|<span data-ttu-id="9994a-143">String</span><span class="sxs-lookup"><span data-stu-id="9994a-143">String</span></span>|<span data-ttu-id="9994a-144">Endereço de email usado para configurar o serviço a serviço do Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="9994a-144">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="9994a-145">serverName</span><span class="sxs-lookup"><span data-stu-id="9994a-145">serverName</span></span>|<span data-ttu-id="9994a-146">String</span><span class="sxs-lookup"><span data-stu-id="9994a-146">String</span></span>|<span data-ttu-id="9994a-147">O nome do servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="9994a-147">The name of the Exchange server.</span></span>|
|<span data-ttu-id="9994a-148">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="9994a-148">connectorServerName</span></span>|<span data-ttu-id="9994a-149">String</span><span class="sxs-lookup"><span data-stu-id="9994a-149">String</span></span>|<span data-ttu-id="9994a-150">O nome do servidor que hospeda o Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="9994a-150">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="9994a-151">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="9994a-151">exchangeConnectorType</span></span>|[<span data-ttu-id="9994a-152">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="9994a-152">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="9994a-153">O tipo de Exchange Connector configurado.</span><span class="sxs-lookup"><span data-stu-id="9994a-153">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="9994a-154">Os valores possíveis são: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="9994a-154">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="9994a-155">versão</span><span class="sxs-lookup"><span data-stu-id="9994a-155">version</span></span>|<span data-ttu-id="9994a-156">String</span><span class="sxs-lookup"><span data-stu-id="9994a-156">String</span></span>|<span data-ttu-id="9994a-157">A versão do ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="9994a-157">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="9994a-158">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="9994a-158">exchangeAlias</span></span>|<span data-ttu-id="9994a-159">String</span><span class="sxs-lookup"><span data-stu-id="9994a-159">String</span></span>|<span data-ttu-id="9994a-160">Um alias atribuído a um servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="9994a-160">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="9994a-161">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="9994a-161">exchangeOrganization</span></span>|<span data-ttu-id="9994a-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9994a-162">String</span></span>|<span data-ttu-id="9994a-163">Organização do Exchange no servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="9994a-163">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="9994a-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="9994a-164">Response</span></span>
<span data-ttu-id="9994a-165">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9994a-165">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9994a-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9994a-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="9994a-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9994a-167">Request</span></span>
<span data-ttu-id="9994a-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9994a-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9994a-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="9994a-169">Response</span></span>
<span data-ttu-id="9994a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9994a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




