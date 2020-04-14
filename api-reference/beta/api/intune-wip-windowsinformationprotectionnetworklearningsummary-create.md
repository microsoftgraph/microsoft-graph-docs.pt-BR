---
title: Criar windowsInformationProtectionNetworkLearningSummary
description: Criar um novo objeto windowsInformationProtectionNetworkLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 49230a41ab866c6f0f7c03bf02917f924d8ec23a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451923"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="e2ecc-103">Criar windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="e2ecc-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

<span data-ttu-id="e2ecc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2ecc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2ecc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e2ecc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2ecc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e2ecc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2ecc-107">Criar um novo objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="e2ecc-107">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2ecc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e2ecc-108">Prerequisites</span></span>
<span data-ttu-id="e2ecc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2ecc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2ecc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2ecc-111">Permission type</span></span>|<span data-ttu-id="e2ecc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e2ecc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2ecc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2ecc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2ecc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2ecc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e2ecc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2ecc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2ecc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2ecc-116">Not supported.</span></span>|
|<span data-ttu-id="e2ecc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2ecc-117">Application</span></span>|<span data-ttu-id="e2ecc-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2ecc-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2ecc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2ecc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="e2ecc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2ecc-120">Request headers</span></span>
|<span data-ttu-id="e2ecc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e2ecc-121">Header</span></span>|<span data-ttu-id="e2ecc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e2ecc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2ecc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2ecc-123">Authorization</span></span>|<span data-ttu-id="e2ecc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2ecc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2ecc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e2ecc-125">Accept</span></span>|<span data-ttu-id="e2ecc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2ecc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2ecc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2ecc-127">Request body</span></span>
<span data-ttu-id="e2ecc-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="e2ecc-128">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="e2ecc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="e2ecc-129">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="e2ecc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2ecc-130">Property</span></span>|<span data-ttu-id="e2ecc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2ecc-131">Type</span></span>|<span data-ttu-id="e2ecc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2ecc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2ecc-133">id</span><span class="sxs-lookup"><span data-stu-id="e2ecc-133">id</span></span>|<span data-ttu-id="e2ecc-134">String</span><span class="sxs-lookup"><span data-stu-id="e2ecc-134">String</span></span>|<span data-ttu-id="e2ecc-135">Identificador exclusivo de WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="e2ecc-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="e2ecc-136">url</span><span class="sxs-lookup"><span data-stu-id="e2ecc-136">url</span></span>|<span data-ttu-id="e2ecc-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2ecc-137">String</span></span>|<span data-ttu-id="e2ecc-138">Url do site</span><span class="sxs-lookup"><span data-stu-id="e2ecc-138">Website url</span></span>|
|<span data-ttu-id="e2ecc-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="e2ecc-139">deviceCount</span></span>|<span data-ttu-id="e2ecc-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e2ecc-140">Int32</span></span>|<span data-ttu-id="e2ecc-141">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="e2ecc-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="e2ecc-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2ecc-142">Response</span></span>
<span data-ttu-id="e2ecc-143">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2ecc-143">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2ecc-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2ecc-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2ecc-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2ecc-145">Request</span></span>
<span data-ttu-id="e2ecc-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2ecc-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="e2ecc-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2ecc-147">Response</span></span>
<span data-ttu-id="e2ecc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2ecc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



