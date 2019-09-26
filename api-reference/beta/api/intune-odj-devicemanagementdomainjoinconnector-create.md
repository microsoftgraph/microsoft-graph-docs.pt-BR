---
title: Criar deviceManagementDomainJoinConnector
description: Criar um novo objeto deviceManagementDomainJoinConnector.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 178d43f041058f4380c7b179d56d7f91d1923a6a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191096"
---
# <a name="create-devicemanagementdomainjoinconnector"></a><span data-ttu-id="be4cd-103">Criar deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="be4cd-103">Create deviceManagementDomainJoinConnector</span></span>

> <span data-ttu-id="be4cd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="be4cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be4cd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="be4cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be4cd-106">Criar um novo objeto [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="be4cd-106">Create a new [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be4cd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="be4cd-107">Prerequisites</span></span>
<span data-ttu-id="be4cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be4cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be4cd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be4cd-110">Permission type</span></span>|<span data-ttu-id="be4cd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="be4cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be4cd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be4cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="be4cd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4cd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="be4cd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be4cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be4cd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be4cd-115">Not supported.</span></span>|
|<span data-ttu-id="be4cd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be4cd-116">Application</span></span>|<span data-ttu-id="be4cd-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4cd-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="be4cd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be4cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/domainJoinConnectors
```

## <a name="request-headers"></a><span data-ttu-id="be4cd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be4cd-119">Request headers</span></span>
|<span data-ttu-id="be4cd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="be4cd-120">Header</span></span>|<span data-ttu-id="be4cd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="be4cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be4cd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="be4cd-122">Authorization</span></span>|<span data-ttu-id="be4cd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be4cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be4cd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="be4cd-124">Accept</span></span>|<span data-ttu-id="be4cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="be4cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be4cd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be4cd-126">Request body</span></span>
<span data-ttu-id="be4cd-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementDomainJoinConnector.</span><span class="sxs-lookup"><span data-stu-id="be4cd-127">In the request body, supply a JSON representation for the deviceManagementDomainJoinConnector object.</span></span>

<span data-ttu-id="be4cd-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementDomainJoinConnector.</span><span class="sxs-lookup"><span data-stu-id="be4cd-128">The following table shows the properties that are required when you create the deviceManagementDomainJoinConnector.</span></span>

|<span data-ttu-id="be4cd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be4cd-129">Property</span></span>|<span data-ttu-id="be4cd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="be4cd-130">Type</span></span>|<span data-ttu-id="be4cd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="be4cd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be4cd-132">id</span><span class="sxs-lookup"><span data-stu-id="be4cd-132">id</span></span>|<span data-ttu-id="be4cd-133">String</span><span class="sxs-lookup"><span data-stu-id="be4cd-133">String</span></span>|<span data-ttu-id="be4cd-134">Identificador exclusivo para representar um conector.</span><span class="sxs-lookup"><span data-stu-id="be4cd-134">Unique identifier to represent a connector.</span></span>|
|<span data-ttu-id="be4cd-135">displayName</span><span class="sxs-lookup"><span data-stu-id="be4cd-135">displayName</span></span>|<span data-ttu-id="be4cd-136">String</span><span class="sxs-lookup"><span data-stu-id="be4cd-136">String</span></span>|<span data-ttu-id="be4cd-137">O nome de exibição do conector.</span><span class="sxs-lookup"><span data-stu-id="be4cd-137">The connector display name.</span></span>|
|<span data-ttu-id="be4cd-138">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="be4cd-138">lastConnectionDateTime</span></span>|<span data-ttu-id="be4cd-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be4cd-139">DateTimeOffset</span></span>|<span data-ttu-id="be4cd-140">Último conector de horário contatado o Intune.</span><span class="sxs-lookup"><span data-stu-id="be4cd-140">Last time connector contacted Intune.</span></span>|
|<span data-ttu-id="be4cd-141">estado</span><span class="sxs-lookup"><span data-stu-id="be4cd-141">state</span></span>|[<span data-ttu-id="be4cd-142">deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="be4cd-142">deviceManagementDomainJoinConnectorState</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|<span data-ttu-id="be4cd-143">O estado do conector.</span><span class="sxs-lookup"><span data-stu-id="be4cd-143">The connector state.</span></span> <span data-ttu-id="be4cd-144">Os valores possíveis são: `active`, `error`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="be4cd-144">Possible values are: `active`, `error`, `inactive`.</span></span>|
|<span data-ttu-id="be4cd-145">versão</span><span class="sxs-lookup"><span data-stu-id="be4cd-145">version</span></span>|<span data-ttu-id="be4cd-146">String</span><span class="sxs-lookup"><span data-stu-id="be4cd-146">String</span></span>|<span data-ttu-id="be4cd-147">A versão do conector.</span><span class="sxs-lookup"><span data-stu-id="be4cd-147">The version of the connector.</span></span>|



## <a name="response"></a><span data-ttu-id="be4cd-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="be4cd-148">Response</span></span>
<span data-ttu-id="be4cd-149">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be4cd-149">If successful, this method returns a `201 Created` response code and a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be4cd-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be4cd-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="be4cd-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be4cd-151">Request</span></span>
<span data-ttu-id="be4cd-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be4cd-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="be4cd-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="be4cd-153">Response</span></span>
<span data-ttu-id="be4cd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be4cd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




