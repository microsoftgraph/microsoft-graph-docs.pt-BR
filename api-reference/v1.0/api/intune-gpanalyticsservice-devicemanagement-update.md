---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ee1c2892047fcff1e304e0dc01e67be831116718
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752853"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="9c4b9-103">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="9c4b9-103">Update deviceManagement</span></span>

<span data-ttu-id="9c4b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c4b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c4b9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9c4b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c4b9-106">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-gpanalyticsservice-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="9c4b9-106">Update the properties of a [deviceManagement](../resources/intune-gpanalyticsservice-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c4b9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9c4b9-107">Prerequisites</span></span>
<span data-ttu-id="9c4b9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c4b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c4b9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c4b9-110">Permission type</span></span>|<span data-ttu-id="9c4b9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9c4b9-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c4b9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c4b9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9c4b9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c4b9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9c4b9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c4b9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c4b9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c4b9-115">Not supported.</span></span>|
|<span data-ttu-id="9c4b9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c4b9-116">Application</span></span>|<span data-ttu-id="9c4b9-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c4b9-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c4b9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c4b9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="9c4b9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c4b9-119">Request headers</span></span>
|<span data-ttu-id="9c4b9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9c4b9-120">Header</span></span>|<span data-ttu-id="9c4b9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9c4b9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c4b9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c4b9-122">Authorization</span></span>|<span data-ttu-id="9c4b9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c4b9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c4b9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9c4b9-124">Accept</span></span>|<span data-ttu-id="9c4b9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9c4b9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c4b9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c4b9-126">Request body</span></span>
<span data-ttu-id="9c4b9-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune-gpanalyticsservice-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="9c4b9-127">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-gpanalyticsservice-devicemanagement.md) object.</span></span>

<span data-ttu-id="9c4b9-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune-gpanalyticsservice-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="9c4b9-128">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-gpanalyticsservice-devicemanagement.md).</span></span>

|<span data-ttu-id="9c4b9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c4b9-129">Property</span></span>|<span data-ttu-id="9c4b9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c4b9-130">Type</span></span>|<span data-ttu-id="9c4b9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c4b9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c4b9-132">id</span><span class="sxs-lookup"><span data-stu-id="9c4b9-132">id</span></span>|<span data-ttu-id="9c4b9-133">String</span><span class="sxs-lookup"><span data-stu-id="9c4b9-133">String</span></span>|<span data-ttu-id="9c4b9-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9c4b9-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9c4b9-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c4b9-135">Response</span></span>
<span data-ttu-id="9c4b9-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-gpanalyticsservice-devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c4b9-136">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-gpanalyticsservice-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c4b9-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c4b9-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c4b9-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c4b9-138">Request</span></span>
<span data-ttu-id="9c4b9-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c4b9-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.deviceManagement"
}
```

### <a name="response"></a><span data-ttu-id="9c4b9-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c4b9-140">Response</span></span>
<span data-ttu-id="9c4b9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9c4b9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b"
}
```




