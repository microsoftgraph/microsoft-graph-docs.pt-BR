---
title: Atualizar deviceManagementExchangeConnector
description: Atualizar as propriedades de um objeto deviceManagementExchangeConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c3e8784796577f08bf8c1f30a748513ff5e081c9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957420"
---
# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="0f7eb-103">Atualizar deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="0f7eb-103">Update deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="0f7eb-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f7eb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f7eb-105">Atualizar as propriedades de um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="0f7eb-105">Update the properties of a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f7eb-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0f7eb-106">Prerequisites</span></span>
<span data-ttu-id="0f7eb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f7eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f7eb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f7eb-109">Permission type</span></span>|<span data-ttu-id="0f7eb-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0f7eb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f7eb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f7eb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0f7eb-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f7eb-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0f7eb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f7eb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f7eb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f7eb-114">Not supported.</span></span>|
|<span data-ttu-id="0f7eb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f7eb-115">Application</span></span>|<span data-ttu-id="0f7eb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f7eb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f7eb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f7eb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="0f7eb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f7eb-118">Request headers</span></span>
|<span data-ttu-id="0f7eb-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0f7eb-119">Header</span></span>|<span data-ttu-id="0f7eb-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0f7eb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f7eb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f7eb-121">Authorization</span></span>|<span data-ttu-id="0f7eb-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f7eb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f7eb-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0f7eb-123">Accept</span></span>|<span data-ttu-id="0f7eb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0f7eb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f7eb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f7eb-125">Request body</span></span>
<span data-ttu-id="0f7eb-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="0f7eb-126">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="0f7eb-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="0f7eb-127">The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>

|<span data-ttu-id="0f7eb-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f7eb-128">Property</span></span>|<span data-ttu-id="0f7eb-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f7eb-129">Type</span></span>|<span data-ttu-id="0f7eb-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f7eb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f7eb-131">id</span><span class="sxs-lookup"><span data-stu-id="0f7eb-131">id</span></span>|<span data-ttu-id="0f7eb-132">String</span><span class="sxs-lookup"><span data-stu-id="0f7eb-132">String</span></span>|<span data-ttu-id="0f7eb-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0f7eb-133">Not yet documented</span></span>|
|<span data-ttu-id="0f7eb-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0f7eb-134">lastSyncDateTime</span></span>|<span data-ttu-id="0f7eb-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f7eb-135">DateTimeOffset</span></span>|<span data-ttu-id="0f7eb-136">Hora da última sincronização do Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="0f7eb-136">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="0f7eb-137">status</span><span class="sxs-lookup"><span data-stu-id="0f7eb-137">status</span></span>|[<span data-ttu-id="0f7eb-138">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="0f7eb-138">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="0f7eb-139">Status do Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="0f7eb-139">Exchange Connector Status.</span></span> <span data-ttu-id="0f7eb-140">Os valores possíveis são: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="0f7eb-140">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="0f7eb-141">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="0f7eb-141">primarySmtpAddress</span></span>|<span data-ttu-id="0f7eb-142">String</span><span class="sxs-lookup"><span data-stu-id="0f7eb-142">String</span></span>|<span data-ttu-id="0f7eb-143">Endereço de email usado para configurar o serviço a serviço do Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="0f7eb-143">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="0f7eb-144">serverName</span><span class="sxs-lookup"><span data-stu-id="0f7eb-144">serverName</span></span>|<span data-ttu-id="0f7eb-145">String</span><span class="sxs-lookup"><span data-stu-id="0f7eb-145">String</span></span>|<span data-ttu-id="0f7eb-146">O nome do servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f7eb-146">The name of the Exchange server.</span></span>|
|<span data-ttu-id="0f7eb-147">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="0f7eb-147">connectorServerName</span></span>|<span data-ttu-id="0f7eb-148">String</span><span class="sxs-lookup"><span data-stu-id="0f7eb-148">String</span></span>|<span data-ttu-id="0f7eb-149">O nome do servidor que hospeda o Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="0f7eb-149">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="0f7eb-150">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="0f7eb-150">exchangeConnectorType</span></span>|[<span data-ttu-id="0f7eb-151">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="0f7eb-151">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="0f7eb-152">O tipo de Exchange Connector configurado.</span><span class="sxs-lookup"><span data-stu-id="0f7eb-152">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="0f7eb-153">Os valores possíveis são: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="0f7eb-153">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="0f7eb-154">versão</span><span class="sxs-lookup"><span data-stu-id="0f7eb-154">version</span></span>|<span data-ttu-id="0f7eb-155">String</span><span class="sxs-lookup"><span data-stu-id="0f7eb-155">String</span></span>|<span data-ttu-id="0f7eb-156">A versão do ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="0f7eb-156">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="0f7eb-157">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="0f7eb-157">exchangeAlias</span></span>|<span data-ttu-id="0f7eb-158">String</span><span class="sxs-lookup"><span data-stu-id="0f7eb-158">String</span></span>|<span data-ttu-id="0f7eb-159">Um alias atribuído a um servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="0f7eb-159">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="0f7eb-160">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="0f7eb-160">exchangeOrganization</span></span>|<span data-ttu-id="0f7eb-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f7eb-161">String</span></span>|<span data-ttu-id="0f7eb-162">Organização do Exchange no servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="0f7eb-162">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="0f7eb-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f7eb-163">Response</span></span>
<span data-ttu-id="0f7eb-164">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f7eb-164">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f7eb-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f7eb-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f7eb-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f7eb-166">Request</span></span>
<span data-ttu-id="0f7eb-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f7eb-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0f7eb-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f7eb-168">Response</span></span>
<span data-ttu-id="0f7eb-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f7eb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



