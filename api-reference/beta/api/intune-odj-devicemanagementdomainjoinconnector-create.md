---
title: Criar deviceManagementDomainJoinConnector
description: Criar um novo objeto deviceManagementDomainJoinConnector.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1272ca36d17683725971f66586a02182b58854a4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462625"
---
# <a name="create-devicemanagementdomainjoinconnector"></a><span data-ttu-id="03308-103">Criar deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="03308-103">Create deviceManagementDomainJoinConnector</span></span>

<span data-ttu-id="03308-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="03308-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03308-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="03308-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03308-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="03308-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03308-107">Criar um novo objeto [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="03308-107">Create a new [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03308-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="03308-108">Prerequisites</span></span>
<span data-ttu-id="03308-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03308-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03308-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03308-111">Permission type</span></span>|<span data-ttu-id="03308-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="03308-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03308-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03308-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03308-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03308-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03308-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03308-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03308-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03308-116">Not supported.</span></span>|
|<span data-ttu-id="03308-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03308-117">Application</span></span>|<span data-ttu-id="03308-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03308-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03308-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03308-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/domainJoinConnectors
```

## <a name="request-headers"></a><span data-ttu-id="03308-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03308-120">Request headers</span></span>
|<span data-ttu-id="03308-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="03308-121">Header</span></span>|<span data-ttu-id="03308-122">Valor</span><span class="sxs-lookup"><span data-stu-id="03308-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03308-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="03308-123">Authorization</span></span>|<span data-ttu-id="03308-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03308-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03308-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="03308-125">Accept</span></span>|<span data-ttu-id="03308-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03308-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03308-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03308-127">Request body</span></span>
<span data-ttu-id="03308-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementDomainJoinConnector.</span><span class="sxs-lookup"><span data-stu-id="03308-128">In the request body, supply a JSON representation for the deviceManagementDomainJoinConnector object.</span></span>

<span data-ttu-id="03308-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementDomainJoinConnector.</span><span class="sxs-lookup"><span data-stu-id="03308-129">The following table shows the properties that are required when you create the deviceManagementDomainJoinConnector.</span></span>

|<span data-ttu-id="03308-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03308-130">Property</span></span>|<span data-ttu-id="03308-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="03308-131">Type</span></span>|<span data-ttu-id="03308-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="03308-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03308-133">id</span><span class="sxs-lookup"><span data-stu-id="03308-133">id</span></span>|<span data-ttu-id="03308-134">String</span><span class="sxs-lookup"><span data-stu-id="03308-134">String</span></span>|<span data-ttu-id="03308-135">Identificador exclusivo para representar um conector.</span><span class="sxs-lookup"><span data-stu-id="03308-135">Unique identifier to represent a connector.</span></span>|
|<span data-ttu-id="03308-136">displayName</span><span class="sxs-lookup"><span data-stu-id="03308-136">displayName</span></span>|<span data-ttu-id="03308-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03308-137">String</span></span>|<span data-ttu-id="03308-138">O nome de exibição do conector.</span><span class="sxs-lookup"><span data-stu-id="03308-138">The connector display name.</span></span>|
|<span data-ttu-id="03308-139">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="03308-139">lastConnectionDateTime</span></span>|<span data-ttu-id="03308-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03308-140">DateTimeOffset</span></span>|<span data-ttu-id="03308-141">Último conector de horário contatado o Intune.</span><span class="sxs-lookup"><span data-stu-id="03308-141">Last time connector contacted Intune.</span></span>|
|<span data-ttu-id="03308-142">state</span><span class="sxs-lookup"><span data-stu-id="03308-142">state</span></span>|[<span data-ttu-id="03308-143">deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="03308-143">deviceManagementDomainJoinConnectorState</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|<span data-ttu-id="03308-144">O estado do conector.</span><span class="sxs-lookup"><span data-stu-id="03308-144">The connector state.</span></span> <span data-ttu-id="03308-145">Os valores possíveis são: `active`, `error`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="03308-145">Possible values are: `active`, `error`, `inactive`.</span></span>|
|<span data-ttu-id="03308-146">versão</span><span class="sxs-lookup"><span data-stu-id="03308-146">version</span></span>|<span data-ttu-id="03308-147">String</span><span class="sxs-lookup"><span data-stu-id="03308-147">String</span></span>|<span data-ttu-id="03308-148">A versão do conector.</span><span class="sxs-lookup"><span data-stu-id="03308-148">The version of the connector.</span></span>|



## <a name="response"></a><span data-ttu-id="03308-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="03308-149">Response</span></span>
<span data-ttu-id="03308-150">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03308-150">If successful, this method returns a `201 Created` response code and a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03308-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03308-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="03308-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03308-152">Request</span></span>
<span data-ttu-id="03308-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03308-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/domainJoinConnectors
Content-type: application/json
Content-length: 235

{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "displayName": "Display Name value",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "error",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="03308-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="03308-154">Response</span></span>
<span data-ttu-id="03308-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03308-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 284

{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "id": "77296cf7-6cf7-7729-f76c-2977f76c2977",
  "displayName": "Display Name value",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "error",
  "version": "Version value"
}
```





