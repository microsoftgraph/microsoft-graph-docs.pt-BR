---
title: Atualizar windowsInformationProtectionAppLearningSummary
description: Atualizar as propriedades de um objeto windowsInformationProtectionAppLearningSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 20c86caed48499fc5df3a1c84254aec1ef5a4216
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360920"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="50a9a-103">Atualizar windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="50a9a-103">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="50a9a-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50a9a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50a9a-105">Atualizar as propriedades de um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="50a9a-105">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50a9a-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50a9a-106">Prerequisites</span></span>
<span data-ttu-id="50a9a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50a9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50a9a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50a9a-109">Permission type</span></span>|<span data-ttu-id="50a9a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50a9a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50a9a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50a9a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="50a9a-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50a9a-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="50a9a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50a9a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50a9a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50a9a-114">Not supported.</span></span>|
|<span data-ttu-id="50a9a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50a9a-115">Application</span></span>|<span data-ttu-id="50a9a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50a9a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50a9a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50a9a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="50a9a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50a9a-118">Request headers</span></span>
|<span data-ttu-id="50a9a-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50a9a-119">Header</span></span>|<span data-ttu-id="50a9a-120">Valor</span><span class="sxs-lookup"><span data-stu-id="50a9a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50a9a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="50a9a-121">Authorization</span></span>|<span data-ttu-id="50a9a-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50a9a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50a9a-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50a9a-123">Accept</span></span>|<span data-ttu-id="50a9a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="50a9a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50a9a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50a9a-125">Request body</span></span>
<span data-ttu-id="50a9a-126">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="50a9a-126">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="50a9a-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="50a9a-127">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="50a9a-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50a9a-128">Property</span></span>|<span data-ttu-id="50a9a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="50a9a-129">Type</span></span>|<span data-ttu-id="50a9a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="50a9a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50a9a-131">id</span><span class="sxs-lookup"><span data-stu-id="50a9a-131">id</span></span>|<span data-ttu-id="50a9a-132">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-132">String</span></span>|<span data-ttu-id="50a9a-133">Identificador exclusivo do WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="50a9a-133">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="50a9a-134">applicationName</span><span class="sxs-lookup"><span data-stu-id="50a9a-134">applicationName</span></span>|<span data-ttu-id="50a9a-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50a9a-135">String</span></span>|<span data-ttu-id="50a9a-136">Nome do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50a9a-136">Application Name</span></span>|
|<span data-ttu-id="50a9a-137">applicationType</span><span class="sxs-lookup"><span data-stu-id="50a9a-137">applicationType</span></span>|[<span data-ttu-id="50a9a-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="50a9a-138">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="50a9a-139">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="50a9a-139">Application Type.</span></span> <span data-ttu-id="50a9a-140">Os valores possíveis são: `universal` e `desktop`.</span><span class="sxs-lookup"><span data-stu-id="50a9a-140">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="50a9a-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="50a9a-141">deviceCount</span></span>|<span data-ttu-id="50a9a-142">Int32</span><span class="sxs-lookup"><span data-stu-id="50a9a-142">Int32</span></span>|<span data-ttu-id="50a9a-143">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="50a9a-143">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="50a9a-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="50a9a-144">Response</span></span>
<span data-ttu-id="50a9a-145">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50a9a-145">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50a9a-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50a9a-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="50a9a-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50a9a-147">Request</span></span>
<span data-ttu-id="50a9a-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50a9a-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="50a9a-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="50a9a-149">Response</span></span>
<span data-ttu-id="50a9a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50a9a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "063baf50-af50-063b-50af-3b0650af3b06",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```




