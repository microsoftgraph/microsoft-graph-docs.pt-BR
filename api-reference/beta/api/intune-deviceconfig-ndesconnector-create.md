---
title: Criar ndesConnector
description: Crie um novo objeto ndesConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0d5d1fdcadc99034f1f02044d02dc32de1dc1a0f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155124"
---
# <a name="create-ndesconnector"></a><span data-ttu-id="525ab-103">Criar ndesConnector</span><span class="sxs-lookup"><span data-stu-id="525ab-103">Create ndesConnector</span></span>

<span data-ttu-id="525ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="525ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="525ab-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="525ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="525ab-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="525ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="525ab-107">Crie um novo [objeto ndesConnector.](../resources/intune-deviceconfig-ndesconnector.md)</span><span class="sxs-lookup"><span data-stu-id="525ab-107">Create a new [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="525ab-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="525ab-108">Prerequisites</span></span>
<span data-ttu-id="525ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="525ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="525ab-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="525ab-111">Permission type</span></span>|<span data-ttu-id="525ab-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="525ab-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="525ab-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="525ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="525ab-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="525ab-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="525ab-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="525ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="525ab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="525ab-116">Not supported.</span></span>|
|<span data-ttu-id="525ab-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="525ab-117">Application</span></span>|<span data-ttu-id="525ab-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="525ab-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="525ab-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="525ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/ndesConnectors
```

## <a name="request-headers"></a><span data-ttu-id="525ab-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="525ab-120">Request headers</span></span>
|<span data-ttu-id="525ab-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="525ab-121">Header</span></span>|<span data-ttu-id="525ab-122">Valor</span><span class="sxs-lookup"><span data-stu-id="525ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="525ab-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="525ab-123">Authorization</span></span>|<span data-ttu-id="525ab-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="525ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="525ab-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="525ab-125">Accept</span></span>|<span data-ttu-id="525ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="525ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="525ab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="525ab-127">Request body</span></span>
<span data-ttu-id="525ab-128">No corpo da solicitação, fornece uma representação JSON para o objeto ndesConnector.</span><span class="sxs-lookup"><span data-stu-id="525ab-128">In the request body, supply a JSON representation for the ndesConnector object.</span></span>

<span data-ttu-id="525ab-129">A tabela a seguir mostra as propriedades necessárias ao criar o ndesConnector.</span><span class="sxs-lookup"><span data-stu-id="525ab-129">The following table shows the properties that are required when you create the ndesConnector.</span></span>

|<span data-ttu-id="525ab-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="525ab-130">Property</span></span>|<span data-ttu-id="525ab-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="525ab-131">Type</span></span>|<span data-ttu-id="525ab-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="525ab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="525ab-133">id</span><span class="sxs-lookup"><span data-stu-id="525ab-133">id</span></span>|<span data-ttu-id="525ab-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="525ab-134">String</span></span>|<span data-ttu-id="525ab-135">A chave do Conector NDES.</span><span class="sxs-lookup"><span data-stu-id="525ab-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="525ab-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="525ab-136">lastConnectionDateTime</span></span>|<span data-ttu-id="525ab-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="525ab-137">DateTimeOffset</span></span>|<span data-ttu-id="525ab-138">Última hora de conexão para o Conector do Ndes</span><span class="sxs-lookup"><span data-stu-id="525ab-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="525ab-139">state</span><span class="sxs-lookup"><span data-stu-id="525ab-139">state</span></span>|[<span data-ttu-id="525ab-140">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="525ab-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="525ab-141">Status do Conector do Ndes.</span><span class="sxs-lookup"><span data-stu-id="525ab-141">Ndes Connector Status.</span></span> <span data-ttu-id="525ab-142">Os valores possíveis são: `none`, `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="525ab-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="525ab-143">displayName</span><span class="sxs-lookup"><span data-stu-id="525ab-143">displayName</span></span>|<span data-ttu-id="525ab-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="525ab-144">String</span></span>|<span data-ttu-id="525ab-145">O nome amigável do Conector do Ndes.</span><span class="sxs-lookup"><span data-stu-id="525ab-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="525ab-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="525ab-146">Response</span></span>
<span data-ttu-id="525ab-147">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="525ab-147">If successful, this method returns a `201 Created` response code and a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="525ab-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="525ab-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="525ab-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="525ab-149">Request</span></span>
<span data-ttu-id="525ab-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="525ab-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="525ab-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="525ab-151">Response</span></span>
<span data-ttu-id="525ab-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="525ab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




