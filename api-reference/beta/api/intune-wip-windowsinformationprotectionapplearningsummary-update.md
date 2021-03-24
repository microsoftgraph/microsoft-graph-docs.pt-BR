---
title: Atualizar windowsInformationProtectionAppLearningSummary
description: Atualizar as propriedades de um objeto windowsInformationProtectionAppLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4cfd5b4f4d74957401028e5b1c5d7656a03853ff
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141453"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="85195-103">Atualizar windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="85195-103">Update windowsInformationProtectionAppLearningSummary</span></span>

<span data-ttu-id="85195-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85195-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85195-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="85195-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85195-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="85195-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85195-107">Atualizar as propriedades de um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="85195-107">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85195-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="85195-108">Prerequisites</span></span>
<span data-ttu-id="85195-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85195-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85195-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85195-111">Permission type</span></span>|<span data-ttu-id="85195-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85195-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85195-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85195-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85195-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85195-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="85195-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85195-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85195-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85195-116">Not supported.</span></span>|
|<span data-ttu-id="85195-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85195-117">Application</span></span>|<span data-ttu-id="85195-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85195-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85195-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85195-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="85195-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85195-120">Request headers</span></span>
|<span data-ttu-id="85195-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="85195-121">Header</span></span>|<span data-ttu-id="85195-122">Valor</span><span class="sxs-lookup"><span data-stu-id="85195-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85195-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="85195-123">Authorization</span></span>|<span data-ttu-id="85195-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85195-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85195-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="85195-125">Accept</span></span>|<span data-ttu-id="85195-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85195-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85195-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85195-127">Request body</span></span>
<span data-ttu-id="85195-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="85195-128">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="85195-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="85195-129">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="85195-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85195-130">Property</span></span>|<span data-ttu-id="85195-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="85195-131">Type</span></span>|<span data-ttu-id="85195-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="85195-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85195-133">id</span><span class="sxs-lookup"><span data-stu-id="85195-133">id</span></span>|<span data-ttu-id="85195-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85195-134">String</span></span>|<span data-ttu-id="85195-135">Identificador exclusivo do WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="85195-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="85195-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="85195-136">applicationName</span></span>|<span data-ttu-id="85195-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85195-137">String</span></span>|<span data-ttu-id="85195-138">Nome do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85195-138">Application Name</span></span>|
|<span data-ttu-id="85195-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="85195-139">applicationType</span></span>|[<span data-ttu-id="85195-140">applicationType</span><span class="sxs-lookup"><span data-stu-id="85195-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="85195-141">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="85195-141">Application Type.</span></span> <span data-ttu-id="85195-142">Os valores possíveis são: `universal` e `desktop`.</span><span class="sxs-lookup"><span data-stu-id="85195-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="85195-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="85195-143">deviceCount</span></span>|<span data-ttu-id="85195-144">Int32</span><span class="sxs-lookup"><span data-stu-id="85195-144">Int32</span></span>|<span data-ttu-id="85195-145">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="85195-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="85195-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="85195-146">Response</span></span>
<span data-ttu-id="85195-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85195-147">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85195-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85195-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="85195-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85195-149">Request</span></span>
<span data-ttu-id="85195-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85195-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="85195-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="85195-151">Response</span></span>
<span data-ttu-id="85195-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85195-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




