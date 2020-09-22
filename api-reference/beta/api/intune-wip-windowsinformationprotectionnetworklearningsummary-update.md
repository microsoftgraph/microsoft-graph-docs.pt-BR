---
title: Atualizar windowsInformationProtectionNetworkLearningSummary
description: Atualizar as propriedades de um objeto windowsInformationProtectionNetworkLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ee4b9e2f6a1c0ec29c41d7073737a9448ebb9f72
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47980103"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="362a0-103">Atualizar windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="362a0-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

<span data-ttu-id="362a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="362a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="362a0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="362a0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="362a0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="362a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="362a0-107">Atualizar as propriedades de um objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="362a0-107">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="362a0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="362a0-108">Prerequisites</span></span>
<span data-ttu-id="362a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="362a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="362a0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="362a0-111">Permission type</span></span>|<span data-ttu-id="362a0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="362a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="362a0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="362a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="362a0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="362a0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="362a0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="362a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="362a0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="362a0-116">Not supported.</span></span>|
|<span data-ttu-id="362a0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="362a0-117">Application</span></span>|<span data-ttu-id="362a0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="362a0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="362a0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="362a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="362a0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="362a0-120">Request headers</span></span>
|<span data-ttu-id="362a0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="362a0-121">Header</span></span>|<span data-ttu-id="362a0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="362a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="362a0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="362a0-123">Authorization</span></span>|<span data-ttu-id="362a0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="362a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="362a0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="362a0-125">Accept</span></span>|<span data-ttu-id="362a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="362a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="362a0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="362a0-127">Request body</span></span>
<span data-ttu-id="362a0-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="362a0-128">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="362a0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="362a0-129">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="362a0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="362a0-130">Property</span></span>|<span data-ttu-id="362a0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="362a0-131">Type</span></span>|<span data-ttu-id="362a0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="362a0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="362a0-133">id</span><span class="sxs-lookup"><span data-stu-id="362a0-133">id</span></span>|<span data-ttu-id="362a0-134">String</span><span class="sxs-lookup"><span data-stu-id="362a0-134">String</span></span>|<span data-ttu-id="362a0-135">Identificador exclusivo de WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="362a0-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="362a0-136">url</span><span class="sxs-lookup"><span data-stu-id="362a0-136">url</span></span>|<span data-ttu-id="362a0-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="362a0-137">String</span></span>|<span data-ttu-id="362a0-138">Url do site</span><span class="sxs-lookup"><span data-stu-id="362a0-138">Website url</span></span>|
|<span data-ttu-id="362a0-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="362a0-139">deviceCount</span></span>|<span data-ttu-id="362a0-140">Int32</span><span class="sxs-lookup"><span data-stu-id="362a0-140">Int32</span></span>|<span data-ttu-id="362a0-141">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="362a0-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="362a0-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="362a0-142">Response</span></span>
<span data-ttu-id="362a0-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="362a0-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="362a0-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="362a0-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="362a0-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="362a0-145">Request</span></span>
<span data-ttu-id="362a0-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="362a0-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="362a0-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="362a0-147">Response</span></span>
<span data-ttu-id="362a0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="362a0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```






