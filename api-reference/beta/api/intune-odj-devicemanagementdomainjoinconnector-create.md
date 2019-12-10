---
title: Criar deviceManagementDomainJoinConnector
description: Criar um novo objeto deviceManagementDomainJoinConnector.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fa7818b71b608aca546e277e035b87e54005a01f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941950"
---
# <a name="create-devicemanagementdomainjoinconnector"></a><span data-ttu-id="1e31d-103">Criar deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="1e31d-103">Create deviceManagementDomainJoinConnector</span></span>

> <span data-ttu-id="1e31d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1e31d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e31d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1e31d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e31d-106">Criar um novo objeto [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="1e31d-106">Create a new [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e31d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e31d-107">Prerequisites</span></span>
<span data-ttu-id="1e31d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e31d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e31d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e31d-110">Permission type</span></span>|<span data-ttu-id="1e31d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1e31d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e31d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e31d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e31d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e31d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1e31d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e31d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e31d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e31d-115">Not supported.</span></span>|
|<span data-ttu-id="1e31d-116">Application</span><span class="sxs-lookup"><span data-stu-id="1e31d-116">Application</span></span>|<span data-ttu-id="1e31d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e31d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e31d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e31d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/domainJoinConnectors
```

## <a name="request-headers"></a><span data-ttu-id="1e31d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e31d-119">Request headers</span></span>
|<span data-ttu-id="1e31d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e31d-120">Header</span></span>|<span data-ttu-id="1e31d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1e31d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e31d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e31d-122">Authorization</span></span>|<span data-ttu-id="1e31d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e31d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e31d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1e31d-124">Accept</span></span>|<span data-ttu-id="1e31d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1e31d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e31d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e31d-126">Request body</span></span>
<span data-ttu-id="1e31d-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementDomainJoinConnector.</span><span class="sxs-lookup"><span data-stu-id="1e31d-127">In the request body, supply a JSON representation for the deviceManagementDomainJoinConnector object.</span></span>

<span data-ttu-id="1e31d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementDomainJoinConnector.</span><span class="sxs-lookup"><span data-stu-id="1e31d-128">The following table shows the properties that are required when you create the deviceManagementDomainJoinConnector.</span></span>

|<span data-ttu-id="1e31d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e31d-129">Property</span></span>|<span data-ttu-id="1e31d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e31d-130">Type</span></span>|<span data-ttu-id="1e31d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e31d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e31d-132">id</span><span class="sxs-lookup"><span data-stu-id="1e31d-132">id</span></span>|<span data-ttu-id="1e31d-133">String</span><span class="sxs-lookup"><span data-stu-id="1e31d-133">String</span></span>|<span data-ttu-id="1e31d-134">Identificador exclusivo para representar um conector.</span><span class="sxs-lookup"><span data-stu-id="1e31d-134">Unique identifier to represent a connector.</span></span>|
|<span data-ttu-id="1e31d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1e31d-135">displayName</span></span>|<span data-ttu-id="1e31d-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e31d-136">String</span></span>|<span data-ttu-id="1e31d-137">O nome de exibição do conector.</span><span class="sxs-lookup"><span data-stu-id="1e31d-137">The connector display name.</span></span>|
|<span data-ttu-id="1e31d-138">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="1e31d-138">lastConnectionDateTime</span></span>|<span data-ttu-id="1e31d-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e31d-139">DateTimeOffset</span></span>|<span data-ttu-id="1e31d-140">Último conector de horário contatado o Intune.</span><span class="sxs-lookup"><span data-stu-id="1e31d-140">Last time connector contacted Intune.</span></span>|
|<span data-ttu-id="1e31d-141">state</span><span class="sxs-lookup"><span data-stu-id="1e31d-141">state</span></span>|[<span data-ttu-id="1e31d-142">deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="1e31d-142">deviceManagementDomainJoinConnectorState</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|<span data-ttu-id="1e31d-143">O estado do conector.</span><span class="sxs-lookup"><span data-stu-id="1e31d-143">The connector state.</span></span> <span data-ttu-id="1e31d-144">Os valores possíveis são: `active`, `error`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="1e31d-144">Possible values are: `active`, `error`, `inactive`.</span></span>|
|<span data-ttu-id="1e31d-145">versão</span><span class="sxs-lookup"><span data-stu-id="1e31d-145">version</span></span>|<span data-ttu-id="1e31d-146">String</span><span class="sxs-lookup"><span data-stu-id="1e31d-146">String</span></span>|<span data-ttu-id="1e31d-147">A versão do conector.</span><span class="sxs-lookup"><span data-stu-id="1e31d-147">The version of the connector.</span></span>|



## <a name="response"></a><span data-ttu-id="1e31d-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e31d-148">Response</span></span>
<span data-ttu-id="1e31d-149">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e31d-149">If successful, this method returns a `201 Created` response code and a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e31d-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e31d-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e31d-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e31d-151">Request</span></span>
<span data-ttu-id="1e31d-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e31d-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1e31d-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e31d-153">Response</span></span>
<span data-ttu-id="1e31d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e31d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





