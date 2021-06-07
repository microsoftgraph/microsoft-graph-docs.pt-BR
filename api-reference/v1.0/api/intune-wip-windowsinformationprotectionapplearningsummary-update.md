---
title: Atualizar windowsInformationProtectionAppLearningSummary
description: Atualizar as propriedades de um objeto windowsInformationProtectionAppLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ffbdaaf7b56ce93c7380660dc425147057f02aa4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752466"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="9e05e-103">Atualizar windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="9e05e-103">Update windowsInformationProtectionAppLearningSummary</span></span>

<span data-ttu-id="9e05e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e05e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e05e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e05e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e05e-106">Atualizar as propriedades de um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="9e05e-106">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e05e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9e05e-107">Prerequisites</span></span>
<span data-ttu-id="9e05e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e05e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e05e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e05e-110">Permission type</span></span>|<span data-ttu-id="9e05e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e05e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e05e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e05e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e05e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e05e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9e05e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e05e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e05e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e05e-115">Not supported.</span></span>|
|<span data-ttu-id="9e05e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e05e-116">Application</span></span>|<span data-ttu-id="9e05e-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e05e-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e05e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e05e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="9e05e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e05e-119">Request headers</span></span>
|<span data-ttu-id="9e05e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e05e-120">Header</span></span>|<span data-ttu-id="9e05e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9e05e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e05e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e05e-122">Authorization</span></span>|<span data-ttu-id="9e05e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e05e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e05e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9e05e-124">Accept</span></span>|<span data-ttu-id="9e05e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9e05e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e05e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e05e-126">Request body</span></span>
<span data-ttu-id="9e05e-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="9e05e-127">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="9e05e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="9e05e-128">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="9e05e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e05e-129">Property</span></span>|<span data-ttu-id="9e05e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e05e-130">Type</span></span>|<span data-ttu-id="9e05e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e05e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e05e-132">id</span><span class="sxs-lookup"><span data-stu-id="9e05e-132">id</span></span>|<span data-ttu-id="9e05e-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e05e-133">String</span></span>|<span data-ttu-id="9e05e-134">Identificador exclusivo do WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="9e05e-134">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="9e05e-135">applicationName</span><span class="sxs-lookup"><span data-stu-id="9e05e-135">applicationName</span></span>|<span data-ttu-id="9e05e-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e05e-136">String</span></span>|<span data-ttu-id="9e05e-137">Nome do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e05e-137">Application Name</span></span>|
|<span data-ttu-id="9e05e-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="9e05e-138">applicationType</span></span>|[<span data-ttu-id="9e05e-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="9e05e-139">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="9e05e-140">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e05e-140">Application Type.</span></span> <span data-ttu-id="9e05e-141">Os valores possíveis são: `universal` e `desktop`.</span><span class="sxs-lookup"><span data-stu-id="9e05e-141">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="9e05e-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="9e05e-142">deviceCount</span></span>|<span data-ttu-id="9e05e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9e05e-143">Int32</span></span>|<span data-ttu-id="9e05e-144">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="9e05e-144">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="9e05e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e05e-145">Response</span></span>
<span data-ttu-id="9e05e-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e05e-146">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e05e-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e05e-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e05e-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e05e-148">Request</span></span>
<span data-ttu-id="9e05e-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e05e-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9e05e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e05e-150">Response</span></span>
<span data-ttu-id="9e05e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e05e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




