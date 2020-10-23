---
title: Atualizar ndesConnector
description: Atualiza as propriedades de um objeto ndesConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2fe297bbb7c530f5a4cef7afd7c17ad6ca8c6e25
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708295"
---
# <a name="update-ndesconnector"></a><span data-ttu-id="891f8-103">Atualizar ndesConnector</span><span class="sxs-lookup"><span data-stu-id="891f8-103">Update ndesConnector</span></span>

<span data-ttu-id="891f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="891f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="891f8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="891f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="891f8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="891f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="891f8-107">Atualiza as propriedades de um objeto [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="891f8-107">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="891f8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="891f8-108">Prerequisites</span></span>
<span data-ttu-id="891f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="891f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="891f8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="891f8-111">Permission type</span></span>|<span data-ttu-id="891f8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="891f8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="891f8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="891f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="891f8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="891f8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="891f8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="891f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="891f8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="891f8-116">Not supported.</span></span>|
|<span data-ttu-id="891f8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="891f8-117">Application</span></span>|<span data-ttu-id="891f8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="891f8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="891f8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="891f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="891f8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="891f8-120">Request headers</span></span>
|<span data-ttu-id="891f8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="891f8-121">Header</span></span>|<span data-ttu-id="891f8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="891f8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="891f8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="891f8-123">Authorization</span></span>|<span data-ttu-id="891f8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="891f8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="891f8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="891f8-125">Accept</span></span>|<span data-ttu-id="891f8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="891f8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="891f8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="891f8-127">Request body</span></span>
<span data-ttu-id="891f8-128">No corpo da solicitação, forneça uma representação JSON do objeto [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="891f8-128">In the request body, supply a JSON representation for the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

<span data-ttu-id="891f8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span><span class="sxs-lookup"><span data-stu-id="891f8-129">The following table shows the properties that are required when you create the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>

|<span data-ttu-id="891f8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="891f8-130">Property</span></span>|<span data-ttu-id="891f8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="891f8-131">Type</span></span>|<span data-ttu-id="891f8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="891f8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="891f8-133">id</span><span class="sxs-lookup"><span data-stu-id="891f8-133">id</span></span>|<span data-ttu-id="891f8-134">String</span><span class="sxs-lookup"><span data-stu-id="891f8-134">String</span></span>|<span data-ttu-id="891f8-135">A chave do conector NDES.</span><span class="sxs-lookup"><span data-stu-id="891f8-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="891f8-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="891f8-136">lastConnectionDateTime</span></span>|<span data-ttu-id="891f8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="891f8-137">DateTimeOffset</span></span>|<span data-ttu-id="891f8-138">Hora da última conexão para o conector NDES</span><span class="sxs-lookup"><span data-stu-id="891f8-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="891f8-139">state</span><span class="sxs-lookup"><span data-stu-id="891f8-139">state</span></span>|[<span data-ttu-id="891f8-140">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="891f8-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="891f8-141">Status do conector NDES.</span><span class="sxs-lookup"><span data-stu-id="891f8-141">Ndes Connector Status.</span></span> <span data-ttu-id="891f8-142">Os valores possíveis são: `none`, `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="891f8-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="891f8-143">displayName</span><span class="sxs-lookup"><span data-stu-id="891f8-143">displayName</span></span>|<span data-ttu-id="891f8-144">String</span><span class="sxs-lookup"><span data-stu-id="891f8-144">String</span></span>|<span data-ttu-id="891f8-145">O nome amigável do conector NDES.</span><span class="sxs-lookup"><span data-stu-id="891f8-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="891f8-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="891f8-146">Response</span></span>
<span data-ttu-id="891f8-147">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="891f8-147">If successful, this method returns a `200 OK` response code and an updated [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="891f8-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="891f8-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="891f8-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="891f8-149">Request</span></span>
<span data-ttu-id="891f8-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="891f8-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="891f8-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="891f8-151">Response</span></span>
<span data-ttu-id="891f8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="891f8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





