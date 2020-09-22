---
title: Criar windowsInformationProtectionNetworkLearningSummary
description: Criar um novo objeto windowsInformationProtectionNetworkLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 37677e12f1ed68a565e5a1c6f57f8d3e4224a392
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028641"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="b3474-103">Criar windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="b3474-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

<span data-ttu-id="b3474-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3474-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3474-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b3474-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3474-106">Criar um novo objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="b3474-106">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3474-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b3474-107">Prerequisites</span></span>
<span data-ttu-id="b3474-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3474-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3474-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3474-110">Permission type</span></span>|<span data-ttu-id="b3474-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b3474-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3474-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3474-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3474-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3474-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b3474-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3474-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3474-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3474-115">Not supported.</span></span>|
|<span data-ttu-id="b3474-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3474-116">Application</span></span>|<span data-ttu-id="b3474-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3474-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3474-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3474-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="b3474-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3474-119">Request headers</span></span>
|<span data-ttu-id="b3474-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3474-120">Header</span></span>|<span data-ttu-id="b3474-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b3474-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3474-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3474-122">Authorization</span></span>|<span data-ttu-id="b3474-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3474-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3474-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b3474-124">Accept</span></span>|<span data-ttu-id="b3474-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b3474-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3474-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3474-126">Request body</span></span>
<span data-ttu-id="b3474-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="b3474-127">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="b3474-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="b3474-128">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="b3474-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3474-129">Property</span></span>|<span data-ttu-id="b3474-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3474-130">Type</span></span>|<span data-ttu-id="b3474-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3474-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3474-132">id</span><span class="sxs-lookup"><span data-stu-id="b3474-132">id</span></span>|<span data-ttu-id="b3474-133">String</span><span class="sxs-lookup"><span data-stu-id="b3474-133">String</span></span>|<span data-ttu-id="b3474-134">Identificador exclusivo de WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="b3474-134">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="b3474-135">url</span><span class="sxs-lookup"><span data-stu-id="b3474-135">url</span></span>|<span data-ttu-id="b3474-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3474-136">String</span></span>|<span data-ttu-id="b3474-137">Url do site</span><span class="sxs-lookup"><span data-stu-id="b3474-137">Website url</span></span>|
|<span data-ttu-id="b3474-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="b3474-138">deviceCount</span></span>|<span data-ttu-id="b3474-139">Int32</span><span class="sxs-lookup"><span data-stu-id="b3474-139">Int32</span></span>|<span data-ttu-id="b3474-140">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="b3474-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="b3474-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3474-141">Response</span></span>
<span data-ttu-id="b3474-142">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3474-142">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3474-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3474-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3474-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3474-144">Request</span></span>
<span data-ttu-id="b3474-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3474-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="b3474-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3474-146">Response</span></span>
<span data-ttu-id="b3474-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3474-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```









