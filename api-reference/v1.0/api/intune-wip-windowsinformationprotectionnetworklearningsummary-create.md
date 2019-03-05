---
title: Criar windowsInformationProtectionNetworkLearningSummary
description: Criar um novo objeto windowsInformationProtectionNetworkLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dc9ffe06e2438510a5301caa09dca2f20c27c293
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257796"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="423dd-103">Criar windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="423dd-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="423dd-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="423dd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="423dd-105">Criar um novo objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="423dd-105">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="423dd-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="423dd-106">Prerequisites</span></span>
<span data-ttu-id="423dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="423dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="423dd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="423dd-109">Permission type</span></span>|<span data-ttu-id="423dd-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="423dd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="423dd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="423dd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="423dd-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="423dd-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="423dd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="423dd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="423dd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="423dd-114">Not supported.</span></span>|
|<span data-ttu-id="423dd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="423dd-115">Application</span></span>|<span data-ttu-id="423dd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="423dd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="423dd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="423dd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="423dd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="423dd-118">Request headers</span></span>
|<span data-ttu-id="423dd-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="423dd-119">Header</span></span>|<span data-ttu-id="423dd-120">Valor</span><span class="sxs-lookup"><span data-stu-id="423dd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="423dd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="423dd-121">Authorization</span></span>|<span data-ttu-id="423dd-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="423dd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="423dd-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="423dd-123">Accept</span></span>|<span data-ttu-id="423dd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="423dd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="423dd-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="423dd-125">Request body</span></span>
<span data-ttu-id="423dd-126">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="423dd-126">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="423dd-127">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="423dd-127">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="423dd-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="423dd-128">Property</span></span>|<span data-ttu-id="423dd-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="423dd-129">Type</span></span>|<span data-ttu-id="423dd-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="423dd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="423dd-131">id</span><span class="sxs-lookup"><span data-stu-id="423dd-131">id</span></span>|<span data-ttu-id="423dd-132">String</span><span class="sxs-lookup"><span data-stu-id="423dd-132">String</span></span>|<span data-ttu-id="423dd-133">Identificador exclusivo de WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="423dd-133">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="423dd-134">url</span><span class="sxs-lookup"><span data-stu-id="423dd-134">url</span></span>|<span data-ttu-id="423dd-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="423dd-135">String</span></span>|<span data-ttu-id="423dd-136">Url do site</span><span class="sxs-lookup"><span data-stu-id="423dd-136">Website url</span></span>|
|<span data-ttu-id="423dd-137">deviceCount</span><span class="sxs-lookup"><span data-stu-id="423dd-137">deviceCount</span></span>|<span data-ttu-id="423dd-138">Int32</span><span class="sxs-lookup"><span data-stu-id="423dd-138">Int32</span></span>|<span data-ttu-id="423dd-139">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="423dd-139">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="423dd-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="423dd-140">Response</span></span>
<span data-ttu-id="423dd-141">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="423dd-141">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="423dd-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="423dd-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="423dd-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="423dd-143">Request</span></span>
<span data-ttu-id="423dd-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="423dd-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="423dd-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="423dd-145">Response</span></span>
<span data-ttu-id="423dd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="423dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



