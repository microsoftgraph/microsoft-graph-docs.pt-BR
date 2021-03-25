---
title: Criar deviceManagementDomainJoinConnector
description: Crie um novo objeto deviceManagementDomainJoinConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 30d14586705ece2bde2c18ab09aef4bd1196dbdc
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152793"
---
# <a name="create-devicemanagementdomainjoinconnector"></a><span data-ttu-id="0c19b-103">Criar deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="0c19b-103">Create deviceManagementDomainJoinConnector</span></span>

<span data-ttu-id="0c19b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c19b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c19b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0c19b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c19b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c19b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c19b-107">Crie um novo [objeto deviceManagementDomainJoinConnector.](../resources/intune-odj-devicemanagementdomainjoinconnector.md)</span><span class="sxs-lookup"><span data-stu-id="0c19b-107">Create a new [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c19b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c19b-108">Prerequisites</span></span>
<span data-ttu-id="0c19b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c19b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c19b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c19b-111">Permission type</span></span>|<span data-ttu-id="0c19b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c19b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c19b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c19b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c19b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c19b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c19b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c19b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c19b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c19b-116">Not supported.</span></span>|
|<span data-ttu-id="0c19b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c19b-117">Application</span></span>|<span data-ttu-id="0c19b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c19b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c19b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c19b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/domainJoinConnectors
```

## <a name="request-headers"></a><span data-ttu-id="0c19b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c19b-120">Request headers</span></span>
|<span data-ttu-id="0c19b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c19b-121">Header</span></span>|<span data-ttu-id="0c19b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0c19b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c19b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c19b-123">Authorization</span></span>|<span data-ttu-id="0c19b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c19b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c19b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0c19b-125">Accept</span></span>|<span data-ttu-id="0c19b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c19b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c19b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c19b-127">Request body</span></span>
<span data-ttu-id="0c19b-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementDomainJoinConnector.</span><span class="sxs-lookup"><span data-stu-id="0c19b-128">In the request body, supply a JSON representation for the deviceManagementDomainJoinConnector object.</span></span>

<span data-ttu-id="0c19b-129">A tabela a seguir mostra as propriedades necessárias ao criar deviceManagementDomainJoinConnector.</span><span class="sxs-lookup"><span data-stu-id="0c19b-129">The following table shows the properties that are required when you create the deviceManagementDomainJoinConnector.</span></span>

|<span data-ttu-id="0c19b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c19b-130">Property</span></span>|<span data-ttu-id="0c19b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c19b-131">Type</span></span>|<span data-ttu-id="0c19b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c19b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c19b-133">id</span><span class="sxs-lookup"><span data-stu-id="0c19b-133">id</span></span>|<span data-ttu-id="0c19b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c19b-134">String</span></span>|<span data-ttu-id="0c19b-135">Identificador exclusivo para representar um conector.</span><span class="sxs-lookup"><span data-stu-id="0c19b-135">Unique identifier to represent a connector.</span></span>|
|<span data-ttu-id="0c19b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0c19b-136">displayName</span></span>|<span data-ttu-id="0c19b-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c19b-137">String</span></span>|<span data-ttu-id="0c19b-138">O nome de exibição do conector.</span><span class="sxs-lookup"><span data-stu-id="0c19b-138">The connector display name.</span></span>|
|<span data-ttu-id="0c19b-139">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="0c19b-139">lastConnectionDateTime</span></span>|<span data-ttu-id="0c19b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c19b-140">DateTimeOffset</span></span>|<span data-ttu-id="0c19b-141">Última vez que o conector entrou em contato com o Intune.</span><span class="sxs-lookup"><span data-stu-id="0c19b-141">Last time connector contacted Intune.</span></span>|
|<span data-ttu-id="0c19b-142">state</span><span class="sxs-lookup"><span data-stu-id="0c19b-142">state</span></span>|[<span data-ttu-id="0c19b-143">deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="0c19b-143">deviceManagementDomainJoinConnectorState</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|<span data-ttu-id="0c19b-144">O estado do conector.</span><span class="sxs-lookup"><span data-stu-id="0c19b-144">The connector state.</span></span> <span data-ttu-id="0c19b-145">Os valores possíveis são: `active`, `error`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="0c19b-145">Possible values are: `active`, `error`, `inactive`.</span></span>|
|<span data-ttu-id="0c19b-146">versão</span><span class="sxs-lookup"><span data-stu-id="0c19b-146">version</span></span>|<span data-ttu-id="0c19b-147">String</span><span class="sxs-lookup"><span data-stu-id="0c19b-147">String</span></span>|<span data-ttu-id="0c19b-148">A versão do conector.</span><span class="sxs-lookup"><span data-stu-id="0c19b-148">The version of the connector.</span></span>|



## <a name="response"></a><span data-ttu-id="0c19b-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c19b-149">Response</span></span>
<span data-ttu-id="0c19b-150">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c19b-150">If successful, this method returns a `201 Created` response code and a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c19b-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c19b-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c19b-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c19b-152">Request</span></span>
<span data-ttu-id="0c19b-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c19b-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0c19b-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c19b-154">Response</span></span>
<span data-ttu-id="0c19b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c19b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




