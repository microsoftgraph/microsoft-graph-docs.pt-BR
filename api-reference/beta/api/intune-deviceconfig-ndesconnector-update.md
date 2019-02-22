---
title: Atualizar ndesConnector
description: Atualiza as propriedades de um objeto ndesConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4d51f22c71ef43784ec45e521f0e1900abdb9c0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140275"
---
# <a name="update-ndesconnector"></a><span data-ttu-id="88f4b-103">Atualizar ndesConnector</span><span class="sxs-lookup"><span data-stu-id="88f4b-103">Update ndesConnector</span></span>

> <span data-ttu-id="88f4b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="88f4b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88f4b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88f4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88f4b-106">Atualiza as propriedades de um objeto [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="88f4b-106">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88f4b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="88f4b-107">Prerequisites</span></span>
<span data-ttu-id="88f4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="88f4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="88f4b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88f4b-110">Permission type</span></span>|<span data-ttu-id="88f4b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="88f4b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88f4b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88f4b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="88f4b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88f4b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="88f4b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88f4b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88f4b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88f4b-115">Not supported.</span></span>|
|<span data-ttu-id="88f4b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88f4b-116">Application</span></span>|<span data-ttu-id="88f4b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88f4b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88f4b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88f4b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="88f4b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88f4b-119">Request headers</span></span>
|<span data-ttu-id="88f4b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88f4b-120">Header</span></span>|<span data-ttu-id="88f4b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="88f4b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88f4b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="88f4b-122">Authorization</span></span>|<span data-ttu-id="88f4b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88f4b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88f4b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="88f4b-124">Accept</span></span>|<span data-ttu-id="88f4b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="88f4b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88f4b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88f4b-126">Request body</span></span>
<span data-ttu-id="88f4b-127">No corpo da solicitação, forneça uma representação JSON do objeto [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="88f4b-127">In the request body, supply a JSON representation for the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

<span data-ttu-id="88f4b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span><span class="sxs-lookup"><span data-stu-id="88f4b-128">The following table shows the properties that are required when you create the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>

|<span data-ttu-id="88f4b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88f4b-129">Property</span></span>|<span data-ttu-id="88f4b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="88f4b-130">Type</span></span>|<span data-ttu-id="88f4b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="88f4b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88f4b-132">id</span><span class="sxs-lookup"><span data-stu-id="88f4b-132">id</span></span>|<span data-ttu-id="88f4b-133">String</span><span class="sxs-lookup"><span data-stu-id="88f4b-133">String</span></span>|<span data-ttu-id="88f4b-134">A chave do conector NDES.</span><span class="sxs-lookup"><span data-stu-id="88f4b-134">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="88f4b-135">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="88f4b-135">lastConnectionDateTime</span></span>|<span data-ttu-id="88f4b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88f4b-136">DateTimeOffset</span></span>|<span data-ttu-id="88f4b-137">Hora da última conexão para o conector NDES</span><span class="sxs-lookup"><span data-stu-id="88f4b-137">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="88f4b-138">state</span><span class="sxs-lookup"><span data-stu-id="88f4b-138">state</span></span>|[<span data-ttu-id="88f4b-139">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="88f4b-139">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="88f4b-140">Status do conector NDES.</span><span class="sxs-lookup"><span data-stu-id="88f4b-140">Ndes Connector Status.</span></span> <span data-ttu-id="88f4b-141">Os valores possíveis são: `none`, `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="88f4b-141">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="88f4b-142">displayName</span><span class="sxs-lookup"><span data-stu-id="88f4b-142">displayName</span></span>|<span data-ttu-id="88f4b-143">String</span><span class="sxs-lookup"><span data-stu-id="88f4b-143">String</span></span>|<span data-ttu-id="88f4b-144">O nome amigável do conector NDES.</span><span class="sxs-lookup"><span data-stu-id="88f4b-144">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="88f4b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="88f4b-145">Response</span></span>
<span data-ttu-id="88f4b-146">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88f4b-146">If successful, this method returns a `200 OK` response code and an updated [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88f4b-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88f4b-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="88f4b-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88f4b-148">Request</span></span>
<span data-ttu-id="88f4b-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88f4b-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/ndesConnectors/{ndesConnectorId}
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="88f4b-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="88f4b-150">Response</span></span>
<span data-ttu-id="88f4b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88f4b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




