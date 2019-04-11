---
title: Atualizar windowsInformationProtectionNetworkLearningSummary
description: Atualizar as propriedades de um objeto windowsInformationProtectionNetworkLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e22260808237797c14d8cf77f14ed07ff0add8e2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802405"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="2e9fd-103">Atualizar windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="2e9fd-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="2e9fd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2e9fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e9fd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2e9fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e9fd-106">Atualizar as propriedades de um objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2e9fd-106">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e9fd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2e9fd-107">Prerequisites</span></span>
<span data-ttu-id="2e9fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e9fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e9fd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e9fd-110">Permission type</span></span>|<span data-ttu-id="2e9fd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2e9fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e9fd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e9fd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2e9fd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e9fd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2e9fd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e9fd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e9fd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e9fd-115">Not supported.</span></span>|
|<span data-ttu-id="2e9fd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e9fd-116">Application</span></span>|<span data-ttu-id="2e9fd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e9fd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e9fd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e9fd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="2e9fd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e9fd-119">Request headers</span></span>
|<span data-ttu-id="2e9fd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2e9fd-120">Header</span></span>|<span data-ttu-id="2e9fd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2e9fd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e9fd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e9fd-122">Authorization</span></span>|<span data-ttu-id="2e9fd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e9fd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e9fd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2e9fd-124">Accept</span></span>|<span data-ttu-id="2e9fd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2e9fd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e9fd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e9fd-126">Request body</span></span>
<span data-ttu-id="2e9fd-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2e9fd-127">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="2e9fd-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2e9fd-128">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="2e9fd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e9fd-129">Property</span></span>|<span data-ttu-id="2e9fd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e9fd-130">Type</span></span>|<span data-ttu-id="2e9fd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e9fd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e9fd-132">id</span><span class="sxs-lookup"><span data-stu-id="2e9fd-132">id</span></span>|<span data-ttu-id="2e9fd-133">String</span><span class="sxs-lookup"><span data-stu-id="2e9fd-133">String</span></span>|<span data-ttu-id="2e9fd-134">Identificador exclusivo de WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="2e9fd-134">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="2e9fd-135">url</span><span class="sxs-lookup"><span data-stu-id="2e9fd-135">url</span></span>|<span data-ttu-id="2e9fd-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e9fd-136">String</span></span>|<span data-ttu-id="2e9fd-137">Url do site</span><span class="sxs-lookup"><span data-stu-id="2e9fd-137">Website url</span></span>|
|<span data-ttu-id="2e9fd-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="2e9fd-138">deviceCount</span></span>|<span data-ttu-id="2e9fd-139">Int32</span><span class="sxs-lookup"><span data-stu-id="2e9fd-139">Int32</span></span>|<span data-ttu-id="2e9fd-140">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="2e9fd-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="2e9fd-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e9fd-141">Response</span></span>
<span data-ttu-id="2e9fd-142">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e9fd-142">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e9fd-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e9fd-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e9fd-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e9fd-144">Request</span></span>
<span data-ttu-id="2e9fd-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e9fd-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2e9fd-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e9fd-146">Response</span></span>
<span data-ttu-id="2e9fd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e9fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





