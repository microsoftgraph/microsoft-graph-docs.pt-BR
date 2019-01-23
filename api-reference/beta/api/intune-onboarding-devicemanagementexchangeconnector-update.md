---
title: Atualizar deviceManagementExchangeConnector
description: Atualizar as propriedades de um objeto deviceManagementExchangeConnector.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ba75d306c302f8f2fca760b3fb6075e340342088
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425012"
---
# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="fe47f-103">Atualizar deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="fe47f-103">Update deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="fe47f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="fe47f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fe47f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fe47f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe47f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="fe47f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe47f-107">Atualizar as propriedades de um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="fe47f-107">Update the properties of a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe47f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fe47f-108">Prerequisites</span></span>
<span data-ttu-id="fe47f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fe47f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fe47f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe47f-111">Permission type</span></span>|<span data-ttu-id="fe47f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fe47f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe47f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe47f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe47f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe47f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fe47f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe47f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe47f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe47f-116">Not supported.</span></span>|
|<span data-ttu-id="fe47f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe47f-117">Application</span></span>|<span data-ttu-id="fe47f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe47f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe47f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe47f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="fe47f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe47f-120">Request headers</span></span>
|<span data-ttu-id="fe47f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe47f-121">Header</span></span>|<span data-ttu-id="fe47f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fe47f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe47f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe47f-123">Authorization</span></span>|<span data-ttu-id="fe47f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe47f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe47f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fe47f-125">Accept</span></span>|<span data-ttu-id="fe47f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe47f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe47f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe47f-127">Request body</span></span>
<span data-ttu-id="fe47f-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="fe47f-128">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="fe47f-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="fe47f-129">The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>

|<span data-ttu-id="fe47f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe47f-130">Property</span></span>|<span data-ttu-id="fe47f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe47f-131">Type</span></span>|<span data-ttu-id="fe47f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe47f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe47f-133">id</span><span class="sxs-lookup"><span data-stu-id="fe47f-133">id</span></span>|<span data-ttu-id="fe47f-134">String</span><span class="sxs-lookup"><span data-stu-id="fe47f-134">String</span></span>|<span data-ttu-id="fe47f-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fe47f-135">Not yet documented</span></span>|
|<span data-ttu-id="fe47f-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="fe47f-136">lastSyncDateTime</span></span>|<span data-ttu-id="fe47f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe47f-137">DateTimeOffset</span></span>|<span data-ttu-id="fe47f-138">Hora da última sincronização do Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="fe47f-138">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="fe47f-139">status</span><span class="sxs-lookup"><span data-stu-id="fe47f-139">status</span></span>|[<span data-ttu-id="fe47f-140">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="fe47f-140">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="fe47f-141">Status de conector do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fe47f-141">Exchange Connector Status.</span></span> <span data-ttu-id="fe47f-142">Os valores possíveis são: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="fe47f-142">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="fe47f-143">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="fe47f-143">primarySmtpAddress</span></span>|<span data-ttu-id="fe47f-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe47f-144">String</span></span>|<span data-ttu-id="fe47f-145">Endereço de email usado para configurar o serviço a serviço do Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="fe47f-145">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="fe47f-146">serverName</span><span class="sxs-lookup"><span data-stu-id="fe47f-146">serverName</span></span>|<span data-ttu-id="fe47f-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe47f-147">String</span></span>|<span data-ttu-id="fe47f-148">O nome do servidor do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fe47f-148">The name of the Exchange server.</span></span>|
|<span data-ttu-id="fe47f-149">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="fe47f-149">connectorServerName</span></span>|<span data-ttu-id="fe47f-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe47f-150">String</span></span>|<span data-ttu-id="fe47f-151">O nome do servidor que hospeda o Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="fe47f-151">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="fe47f-152">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="fe47f-152">exchangeConnectorType</span></span>|[<span data-ttu-id="fe47f-153">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="fe47f-153">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="fe47f-154">O tipo de Exchange Connector configurado.</span><span class="sxs-lookup"><span data-stu-id="fe47f-154">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="fe47f-155">Os valores possíveis são: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="fe47f-155">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="fe47f-156">version</span><span class="sxs-lookup"><span data-stu-id="fe47f-156">version</span></span>|<span data-ttu-id="fe47f-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe47f-157">String</span></span>|<span data-ttu-id="fe47f-158">A versão do ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="fe47f-158">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="fe47f-159">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="fe47f-159">exchangeAlias</span></span>|<span data-ttu-id="fe47f-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe47f-160">String</span></span>|<span data-ttu-id="fe47f-161">Um alias atribuído a um servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="fe47f-161">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="fe47f-162">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="fe47f-162">exchangeOrganization</span></span>|<span data-ttu-id="fe47f-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe47f-163">String</span></span>|<span data-ttu-id="fe47f-164">Organização do Exchange no servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="fe47f-164">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="fe47f-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe47f-165">Response</span></span>
<span data-ttu-id="fe47f-166">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe47f-166">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe47f-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe47f-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe47f-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe47f-168">Request</span></span>
<span data-ttu-id="fe47f-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe47f-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fe47f-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe47f-170">Response</span></span>
<span data-ttu-id="fe47f-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe47f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




