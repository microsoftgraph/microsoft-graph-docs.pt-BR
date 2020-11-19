---
title: Criar ndesConnector
description: Criar um novo objeto ndesConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c6e7d4af96843416e63bcaa500e087b27d108ab8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49282871"
---
# <a name="create-ndesconnector"></a><span data-ttu-id="ae3f5-103">Criar ndesConnector</span><span class="sxs-lookup"><span data-stu-id="ae3f5-103">Create ndesConnector</span></span>

<span data-ttu-id="ae3f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae3f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae3f5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ae3f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae3f5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae3f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae3f5-107">Criar um novo objeto [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="ae3f5-107">Create a new [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae3f5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ae3f5-108">Prerequisites</span></span>
<span data-ttu-id="ae3f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae3f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae3f5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae3f5-111">Permission type</span></span>|<span data-ttu-id="ae3f5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ae3f5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae3f5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae3f5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae3f5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae3f5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae3f5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae3f5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae3f5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae3f5-116">Not supported.</span></span>|
|<span data-ttu-id="ae3f5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae3f5-117">Application</span></span>|<span data-ttu-id="ae3f5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae3f5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae3f5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae3f5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/ndesConnectors
```

## <a name="request-headers"></a><span data-ttu-id="ae3f5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae3f5-120">Request headers</span></span>
|<span data-ttu-id="ae3f5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae3f5-121">Header</span></span>|<span data-ttu-id="ae3f5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ae3f5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae3f5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae3f5-123">Authorization</span></span>|<span data-ttu-id="ae3f5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae3f5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae3f5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ae3f5-125">Accept</span></span>|<span data-ttu-id="ae3f5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae3f5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae3f5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae3f5-127">Request body</span></span>
<span data-ttu-id="ae3f5-128">No corpo da solicitação, forneça uma representação JSON do objeto ndesConnector.</span><span class="sxs-lookup"><span data-stu-id="ae3f5-128">In the request body, supply a JSON representation for the ndesConnector object.</span></span>

<span data-ttu-id="ae3f5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar ndesConnector.</span><span class="sxs-lookup"><span data-stu-id="ae3f5-129">The following table shows the properties that are required when you create the ndesConnector.</span></span>

|<span data-ttu-id="ae3f5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae3f5-130">Property</span></span>|<span data-ttu-id="ae3f5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae3f5-131">Type</span></span>|<span data-ttu-id="ae3f5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae3f5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae3f5-133">id</span><span class="sxs-lookup"><span data-stu-id="ae3f5-133">id</span></span>|<span data-ttu-id="ae3f5-134">String</span><span class="sxs-lookup"><span data-stu-id="ae3f5-134">String</span></span>|<span data-ttu-id="ae3f5-135">A chave do conector NDES.</span><span class="sxs-lookup"><span data-stu-id="ae3f5-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="ae3f5-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="ae3f5-136">lastConnectionDateTime</span></span>|<span data-ttu-id="ae3f5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae3f5-137">DateTimeOffset</span></span>|<span data-ttu-id="ae3f5-138">Hora da última conexão para o conector NDES</span><span class="sxs-lookup"><span data-stu-id="ae3f5-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="ae3f5-139">state</span><span class="sxs-lookup"><span data-stu-id="ae3f5-139">state</span></span>|[<span data-ttu-id="ae3f5-140">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="ae3f5-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="ae3f5-141">Status do conector NDES.</span><span class="sxs-lookup"><span data-stu-id="ae3f5-141">Ndes Connector Status.</span></span> <span data-ttu-id="ae3f5-142">Os valores possíveis são: `none`, `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="ae3f5-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="ae3f5-143">displayName</span><span class="sxs-lookup"><span data-stu-id="ae3f5-143">displayName</span></span>|<span data-ttu-id="ae3f5-144">String</span><span class="sxs-lookup"><span data-stu-id="ae3f5-144">String</span></span>|<span data-ttu-id="ae3f5-145">O nome amigável do conector NDES.</span><span class="sxs-lookup"><span data-stu-id="ae3f5-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="ae3f5-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae3f5-146">Response</span></span>
<span data-ttu-id="ae3f5-147">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae3f5-147">If successful, this method returns a `201 Created` response code and a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae3f5-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae3f5-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae3f5-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae3f5-149">Request</span></span>
<span data-ttu-id="ae3f5-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae3f5-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/ndesConnectors
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="ae3f5-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae3f5-151">Response</span></span>
<span data-ttu-id="ae3f5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae3f5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "id": "e71fa706-a706-e71f-06a7-1fe706a71fe7",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```




