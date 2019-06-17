---
title: Atualizar deviceManagementDomainJoinConnector
description: Atualiza as propriedades de um objeto deviceManagementDomainJoinConnector.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 760683b2b837ac8bcfab40a12b3bf4f84214d2c2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002151"
---
# <a name="update-devicemanagementdomainjoinconnector"></a><span data-ttu-id="4bd66-103">Atualizar deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="4bd66-103">Update deviceManagementDomainJoinConnector</span></span>

> <span data-ttu-id="4bd66-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4bd66-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4bd66-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4bd66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bd66-106">Atualiza as propriedades de um objeto [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="4bd66-106">Update the properties of a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4bd66-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4bd66-107">Prerequisites</span></span>
<span data-ttu-id="4bd66-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bd66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bd66-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4bd66-110">Permission type</span></span>|<span data-ttu-id="4bd66-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4bd66-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bd66-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4bd66-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4bd66-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bd66-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4bd66-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4bd66-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bd66-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bd66-115">Not supported.</span></span>|
|<span data-ttu-id="4bd66-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bd66-116">Application</span></span>|<span data-ttu-id="4bd66-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bd66-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bd66-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4bd66-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/domainJoinConnectors/{deviceManagementDomainJoinConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="4bd66-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4bd66-119">Request headers</span></span>
|<span data-ttu-id="4bd66-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4bd66-120">Header</span></span>|<span data-ttu-id="4bd66-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4bd66-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bd66-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4bd66-122">Authorization</span></span>|<span data-ttu-id="4bd66-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4bd66-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bd66-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4bd66-124">Accept</span></span>|<span data-ttu-id="4bd66-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4bd66-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bd66-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4bd66-126">Request body</span></span>
<span data-ttu-id="4bd66-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="4bd66-127">In the request body, supply a JSON representation for the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

<span data-ttu-id="4bd66-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md).</span><span class="sxs-lookup"><span data-stu-id="4bd66-128">The following table shows the properties that are required when you create the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md).</span></span>

|<span data-ttu-id="4bd66-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4bd66-129">Property</span></span>|<span data-ttu-id="4bd66-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bd66-130">Type</span></span>|<span data-ttu-id="4bd66-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bd66-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bd66-132">id</span><span class="sxs-lookup"><span data-stu-id="4bd66-132">id</span></span>|<span data-ttu-id="4bd66-133">String</span><span class="sxs-lookup"><span data-stu-id="4bd66-133">String</span></span>|<span data-ttu-id="4bd66-134">Identificador exclusivo para representar um conector.</span><span class="sxs-lookup"><span data-stu-id="4bd66-134">Unique identifier to represent a connector.</span></span>|
|<span data-ttu-id="4bd66-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4bd66-135">displayName</span></span>|<span data-ttu-id="4bd66-136">String</span><span class="sxs-lookup"><span data-stu-id="4bd66-136">String</span></span>|<span data-ttu-id="4bd66-137">O nome de exibição do conector.</span><span class="sxs-lookup"><span data-stu-id="4bd66-137">The connector display name.</span></span>|
|<span data-ttu-id="4bd66-138">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="4bd66-138">lastConnectionDateTime</span></span>|<span data-ttu-id="4bd66-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bd66-139">DateTimeOffset</span></span>|<span data-ttu-id="4bd66-140">Último conector de horário contatado o Intune.</span><span class="sxs-lookup"><span data-stu-id="4bd66-140">Last time connector contacted Intune.</span></span>|
|<span data-ttu-id="4bd66-141">estado</span><span class="sxs-lookup"><span data-stu-id="4bd66-141">state</span></span>|[<span data-ttu-id="4bd66-142">deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="4bd66-142">deviceManagementDomainJoinConnectorState</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|<span data-ttu-id="4bd66-143">O estado do conector.</span><span class="sxs-lookup"><span data-stu-id="4bd66-143">The connector state.</span></span> <span data-ttu-id="4bd66-144">Os valores possíveis são: `active`, `error`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="4bd66-144">Possible values are: `active`, `error`, `inactive`.</span></span>|
|<span data-ttu-id="4bd66-145">versão</span><span class="sxs-lookup"><span data-stu-id="4bd66-145">version</span></span>|<span data-ttu-id="4bd66-146">String</span><span class="sxs-lookup"><span data-stu-id="4bd66-146">String</span></span>|<span data-ttu-id="4bd66-147">A versão do conector.</span><span class="sxs-lookup"><span data-stu-id="4bd66-147">The version of the connector.</span></span>|



## <a name="response"></a><span data-ttu-id="4bd66-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bd66-148">Response</span></span>
<span data-ttu-id="4bd66-149">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bd66-149">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bd66-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4bd66-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="4bd66-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bd66-151">Request</span></span>
<span data-ttu-id="4bd66-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bd66-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/domainJoinConnectors/{deviceManagementDomainJoinConnectorId}
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

### <a name="response"></a><span data-ttu-id="4bd66-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bd66-153">Response</span></span>
<span data-ttu-id="4bd66-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4bd66-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





