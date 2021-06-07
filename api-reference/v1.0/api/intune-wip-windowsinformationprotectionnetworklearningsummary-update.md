---
title: Atualizar windowsInformationProtectionNetworkLearningSummary
description: Atualizar as propriedades de um objeto windowsInformationProtectionNetworkLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 54a0e5b33cd8897f6b0b243baca2ebb7bb91f0f4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751423"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="b9200-103">Atualizar windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="b9200-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

<span data-ttu-id="b9200-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9200-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9200-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9200-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9200-106">Atualizar as propriedades de um objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="b9200-106">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9200-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b9200-107">Prerequisites</span></span>
<span data-ttu-id="b9200-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9200-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9200-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9200-110">Permission type</span></span>|<span data-ttu-id="b9200-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9200-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9200-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9200-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b9200-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9200-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b9200-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9200-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9200-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9200-115">Not supported.</span></span>|
|<span data-ttu-id="b9200-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9200-116">Application</span></span>|<span data-ttu-id="b9200-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9200-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9200-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9200-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="b9200-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9200-119">Request headers</span></span>
|<span data-ttu-id="b9200-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9200-120">Header</span></span>|<span data-ttu-id="b9200-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b9200-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9200-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9200-122">Authorization</span></span>|<span data-ttu-id="b9200-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9200-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9200-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b9200-124">Accept</span></span>|<span data-ttu-id="b9200-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b9200-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9200-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9200-126">Request body</span></span>
<span data-ttu-id="b9200-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="b9200-127">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="b9200-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="b9200-128">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="b9200-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9200-129">Property</span></span>|<span data-ttu-id="b9200-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9200-130">Type</span></span>|<span data-ttu-id="b9200-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9200-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9200-132">id</span><span class="sxs-lookup"><span data-stu-id="b9200-132">id</span></span>|<span data-ttu-id="b9200-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9200-133">String</span></span>|<span data-ttu-id="b9200-134">Identificador exclusivo de WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="b9200-134">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="b9200-135">url</span><span class="sxs-lookup"><span data-stu-id="b9200-135">url</span></span>|<span data-ttu-id="b9200-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9200-136">String</span></span>|<span data-ttu-id="b9200-137">Url do site</span><span class="sxs-lookup"><span data-stu-id="b9200-137">Website url</span></span>|
|<span data-ttu-id="b9200-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="b9200-138">deviceCount</span></span>|<span data-ttu-id="b9200-139">Int32</span><span class="sxs-lookup"><span data-stu-id="b9200-139">Int32</span></span>|<span data-ttu-id="b9200-140">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="b9200-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="b9200-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9200-141">Response</span></span>
<span data-ttu-id="b9200-142">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9200-142">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9200-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9200-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9200-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9200-144">Request</span></span>
<span data-ttu-id="b9200-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9200-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="b9200-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9200-146">Response</span></span>
<span data-ttu-id="b9200-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9200-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




