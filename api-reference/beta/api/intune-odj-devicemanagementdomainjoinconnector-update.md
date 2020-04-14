---
title: Atualizar deviceManagementDomainJoinConnector
description: Atualiza as propriedades de um objeto deviceManagementDomainJoinConnector.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 28204a3f8fd81ffe526edbfb19a3e4af5851852f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461041"
---
# <a name="update-devicemanagementdomainjoinconnector"></a><span data-ttu-id="d1652-103">Atualizar deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="d1652-103">Update deviceManagementDomainJoinConnector</span></span>

<span data-ttu-id="d1652-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1652-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1652-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d1652-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1652-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d1652-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1652-107">Atualiza as propriedades de um objeto [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="d1652-107">Update the properties of a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1652-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d1652-108">Prerequisites</span></span>
<span data-ttu-id="d1652-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1652-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1652-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1652-111">Permission type</span></span>|<span data-ttu-id="d1652-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d1652-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1652-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1652-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1652-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1652-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d1652-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1652-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1652-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1652-116">Not supported.</span></span>|
|<span data-ttu-id="d1652-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1652-117">Application</span></span>|<span data-ttu-id="d1652-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1652-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1652-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1652-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/domainJoinConnectors/{deviceManagementDomainJoinConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="d1652-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1652-120">Request headers</span></span>
|<span data-ttu-id="d1652-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d1652-121">Header</span></span>|<span data-ttu-id="d1652-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d1652-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1652-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1652-123">Authorization</span></span>|<span data-ttu-id="d1652-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1652-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1652-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d1652-125">Accept</span></span>|<span data-ttu-id="d1652-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1652-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1652-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1652-127">Request body</span></span>
<span data-ttu-id="d1652-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="d1652-128">In the request body, supply a JSON representation for the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

<span data-ttu-id="d1652-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md).</span><span class="sxs-lookup"><span data-stu-id="d1652-129">The following table shows the properties that are required when you create the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md).</span></span>

|<span data-ttu-id="d1652-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1652-130">Property</span></span>|<span data-ttu-id="d1652-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1652-131">Type</span></span>|<span data-ttu-id="d1652-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1652-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1652-133">id</span><span class="sxs-lookup"><span data-stu-id="d1652-133">id</span></span>|<span data-ttu-id="d1652-134">String</span><span class="sxs-lookup"><span data-stu-id="d1652-134">String</span></span>|<span data-ttu-id="d1652-135">Identificador exclusivo para representar um conector.</span><span class="sxs-lookup"><span data-stu-id="d1652-135">Unique identifier to represent a connector.</span></span>|
|<span data-ttu-id="d1652-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d1652-136">displayName</span></span>|<span data-ttu-id="d1652-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1652-137">String</span></span>|<span data-ttu-id="d1652-138">O nome de exibição do conector.</span><span class="sxs-lookup"><span data-stu-id="d1652-138">The connector display name.</span></span>|
|<span data-ttu-id="d1652-139">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="d1652-139">lastConnectionDateTime</span></span>|<span data-ttu-id="d1652-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1652-140">DateTimeOffset</span></span>|<span data-ttu-id="d1652-141">Último conector de horário contatado o Intune.</span><span class="sxs-lookup"><span data-stu-id="d1652-141">Last time connector contacted Intune.</span></span>|
|<span data-ttu-id="d1652-142">state</span><span class="sxs-lookup"><span data-stu-id="d1652-142">state</span></span>|[<span data-ttu-id="d1652-143">deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="d1652-143">deviceManagementDomainJoinConnectorState</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|<span data-ttu-id="d1652-144">O estado do conector.</span><span class="sxs-lookup"><span data-stu-id="d1652-144">The connector state.</span></span> <span data-ttu-id="d1652-145">Os valores possíveis são: `active`, `error`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="d1652-145">Possible values are: `active`, `error`, `inactive`.</span></span>|
|<span data-ttu-id="d1652-146">versão</span><span class="sxs-lookup"><span data-stu-id="d1652-146">version</span></span>|<span data-ttu-id="d1652-147">String</span><span class="sxs-lookup"><span data-stu-id="d1652-147">String</span></span>|<span data-ttu-id="d1652-148">A versão do conector.</span><span class="sxs-lookup"><span data-stu-id="d1652-148">The version of the connector.</span></span>|



## <a name="response"></a><span data-ttu-id="d1652-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1652-149">Response</span></span>
<span data-ttu-id="d1652-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1652-150">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1652-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1652-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1652-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1652-152">Request</span></span>
<span data-ttu-id="d1652-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1652-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d1652-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1652-154">Response</span></span>
<span data-ttu-id="d1652-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1652-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



