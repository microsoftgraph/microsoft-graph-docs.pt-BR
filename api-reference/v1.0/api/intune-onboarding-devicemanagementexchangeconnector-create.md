---
title: Criar deviceManagementExchangeConnector
description: Crie um novo objeto deviceManagementExchangeConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 292562a2a7083e63f083d0ccad5e11071a27ce96
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256438"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="02e89-103">Criar deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="02e89-103">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="02e89-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02e89-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02e89-105">Crie um novo objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="02e89-105">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02e89-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02e89-106">Prerequisites</span></span>
<span data-ttu-id="02e89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="02e89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="02e89-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02e89-109">Permission type</span></span>|<span data-ttu-id="02e89-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02e89-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02e89-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02e89-111">Delegated (work or school account)</span></span>|<span data-ttu-id="02e89-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02e89-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="02e89-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02e89-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02e89-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02e89-114">Not supported.</span></span>|
|<span data-ttu-id="02e89-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02e89-115">Application</span></span>|<span data-ttu-id="02e89-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02e89-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02e89-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02e89-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="02e89-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02e89-118">Request headers</span></span>
|<span data-ttu-id="02e89-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02e89-119">Header</span></span>|<span data-ttu-id="02e89-120">Valor</span><span class="sxs-lookup"><span data-stu-id="02e89-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02e89-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="02e89-121">Authorization</span></span>|<span data-ttu-id="02e89-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02e89-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02e89-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02e89-123">Accept</span></span>|<span data-ttu-id="02e89-124">application/json</span><span class="sxs-lookup"><span data-stu-id="02e89-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02e89-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02e89-125">Request body</span></span>
<span data-ttu-id="02e89-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="02e89-126">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="02e89-127">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="02e89-127">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="02e89-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02e89-128">Property</span></span>|<span data-ttu-id="02e89-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="02e89-129">Type</span></span>|<span data-ttu-id="02e89-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="02e89-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02e89-131">id</span><span class="sxs-lookup"><span data-stu-id="02e89-131">id</span></span>|<span data-ttu-id="02e89-132">String</span><span class="sxs-lookup"><span data-stu-id="02e89-132">String</span></span>|<span data-ttu-id="02e89-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="02e89-133">Not yet documented</span></span>|
|<span data-ttu-id="02e89-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="02e89-134">lastSyncDateTime</span></span>|<span data-ttu-id="02e89-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02e89-135">DateTimeOffset</span></span>|<span data-ttu-id="02e89-136">Hora da última sincronização do Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="02e89-136">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="02e89-137">status</span><span class="sxs-lookup"><span data-stu-id="02e89-137">status</span></span>|[<span data-ttu-id="02e89-138">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="02e89-138">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="02e89-139">Status do Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="02e89-139">Exchange Connector Status.</span></span> <span data-ttu-id="02e89-140">Os valores possíveis são: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="02e89-140">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="02e89-141">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="02e89-141">primarySmtpAddress</span></span>|<span data-ttu-id="02e89-142">String</span><span class="sxs-lookup"><span data-stu-id="02e89-142">String</span></span>|<span data-ttu-id="02e89-143">Endereço de email usado para configurar o serviço a serviço do Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="02e89-143">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="02e89-144">serverName</span><span class="sxs-lookup"><span data-stu-id="02e89-144">serverName</span></span>|<span data-ttu-id="02e89-145">String</span><span class="sxs-lookup"><span data-stu-id="02e89-145">String</span></span>|<span data-ttu-id="02e89-146">O nome do servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="02e89-146">The name of the Exchange server.</span></span>|
|<span data-ttu-id="02e89-147">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="02e89-147">connectorServerName</span></span>|<span data-ttu-id="02e89-148">String</span><span class="sxs-lookup"><span data-stu-id="02e89-148">String</span></span>|<span data-ttu-id="02e89-149">O nome do servidor que hospeda o Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="02e89-149">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="02e89-150">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="02e89-150">exchangeConnectorType</span></span>|[<span data-ttu-id="02e89-151">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="02e89-151">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="02e89-152">O tipo de Exchange Connector configurado.</span><span class="sxs-lookup"><span data-stu-id="02e89-152">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="02e89-153">Os valores possíveis são: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="02e89-153">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="02e89-154">version</span><span class="sxs-lookup"><span data-stu-id="02e89-154">version</span></span>|<span data-ttu-id="02e89-155">String</span><span class="sxs-lookup"><span data-stu-id="02e89-155">String</span></span>|<span data-ttu-id="02e89-156">A versão do ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="02e89-156">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="02e89-157">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="02e89-157">exchangeAlias</span></span>|<span data-ttu-id="02e89-158">String</span><span class="sxs-lookup"><span data-stu-id="02e89-158">String</span></span>|<span data-ttu-id="02e89-159">Um alias atribuído a um servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="02e89-159">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="02e89-160">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="02e89-160">exchangeOrganization</span></span>|<span data-ttu-id="02e89-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02e89-161">String</span></span>|<span data-ttu-id="02e89-162">Organização do Exchange no servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="02e89-162">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="02e89-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="02e89-163">Response</span></span>
<span data-ttu-id="02e89-164">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02e89-164">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02e89-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02e89-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="02e89-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02e89-166">Request</span></span>
<span data-ttu-id="02e89-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02e89-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="02e89-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="02e89-168">Response</span></span>
<span data-ttu-id="02e89-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02e89-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



