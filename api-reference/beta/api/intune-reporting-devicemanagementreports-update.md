---
title: Atualizar deviceManagementReports
description: Atualiza as propriedades de um objeto deviceManagementReports.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a4b49f49962da7cf17392e0fa9f0ee21aca3deac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044827"
---
# <a name="update-devicemanagementreports"></a><span data-ttu-id="31068-103">Atualizar deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="31068-103">Update deviceManagementReports</span></span>

<span data-ttu-id="31068-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31068-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31068-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="31068-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31068-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="31068-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31068-107">Atualiza as propriedades de um objeto [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) .</span><span class="sxs-lookup"><span data-stu-id="31068-107">Update the properties of a [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31068-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="31068-108">Prerequisites</span></span>
<span data-ttu-id="31068-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31068-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31068-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31068-111">Permission type</span></span>|<span data-ttu-id="31068-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="31068-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31068-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31068-113">Delegated (work or school account)</span></span>|<span data-ttu-id="31068-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="31068-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="31068-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31068-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31068-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31068-116">Not supported.</span></span>|
|<span data-ttu-id="31068-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31068-117">Application</span></span>|<span data-ttu-id="31068-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="31068-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31068-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31068-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports
```

## <a name="request-headers"></a><span data-ttu-id="31068-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31068-120">Request headers</span></span>
|<span data-ttu-id="31068-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="31068-121">Header</span></span>|<span data-ttu-id="31068-122">Valor</span><span class="sxs-lookup"><span data-stu-id="31068-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31068-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="31068-123">Authorization</span></span>|<span data-ttu-id="31068-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31068-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31068-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="31068-125">Accept</span></span>|<span data-ttu-id="31068-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31068-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31068-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31068-127">Request body</span></span>
<span data-ttu-id="31068-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) .</span><span class="sxs-lookup"><span data-stu-id="31068-128">In the request body, supply a JSON representation for the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

<span data-ttu-id="31068-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md).</span><span class="sxs-lookup"><span data-stu-id="31068-129">The following table shows the properties that are required when you create the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md).</span></span>

|<span data-ttu-id="31068-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31068-130">Property</span></span>|<span data-ttu-id="31068-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="31068-131">Type</span></span>|<span data-ttu-id="31068-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="31068-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31068-133">id</span><span class="sxs-lookup"><span data-stu-id="31068-133">id</span></span>|<span data-ttu-id="31068-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31068-134">String</span></span>|<span data-ttu-id="31068-135">Identificador exclusivo para esta entidade</span><span class="sxs-lookup"><span data-stu-id="31068-135">Unique identifier for this entity</span></span>|



## <a name="response"></a><span data-ttu-id="31068-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="31068-136">Response</span></span>
<span data-ttu-id="31068-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31068-137">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31068-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31068-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="31068-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31068-139">Request</span></span>
<span data-ttu-id="31068-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31068-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.deviceManagementReports"
}
```

### <a name="response"></a><span data-ttu-id="31068-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="31068-141">Response</span></span>
<span data-ttu-id="31068-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31068-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "d6a697d3-97d3-d6a6-d397-a6d6d397a6d6"
}
```






