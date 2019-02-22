---
title: Criar windowsInformationProtectionAppLearningSummary
description: Criar um novo objeto windowsInformationProtectionAppLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 165664c3977ede205c406da712d5a331ff9de7c7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174654"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="24911-103">Criar windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="24911-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="24911-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="24911-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24911-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="24911-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24911-106">Criar um novo objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="24911-106">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24911-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="24911-107">Prerequisites</span></span>
<span data-ttu-id="24911-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="24911-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="24911-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24911-110">Permission type</span></span>|<span data-ttu-id="24911-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="24911-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24911-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24911-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24911-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24911-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="24911-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24911-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24911-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24911-115">Not supported.</span></span>|
|<span data-ttu-id="24911-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24911-116">Application</span></span>|<span data-ttu-id="24911-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24911-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24911-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24911-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="24911-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24911-119">Request headers</span></span>
|<span data-ttu-id="24911-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="24911-120">Header</span></span>|<span data-ttu-id="24911-121">Valor</span><span class="sxs-lookup"><span data-stu-id="24911-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24911-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="24911-122">Authorization</span></span>|<span data-ttu-id="24911-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24911-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24911-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="24911-124">Accept</span></span>|<span data-ttu-id="24911-125">application/json</span><span class="sxs-lookup"><span data-stu-id="24911-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24911-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24911-126">Request body</span></span>
<span data-ttu-id="24911-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="24911-127">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="24911-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="24911-128">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="24911-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24911-129">Property</span></span>|<span data-ttu-id="24911-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="24911-130">Type</span></span>|<span data-ttu-id="24911-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="24911-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24911-132">id</span><span class="sxs-lookup"><span data-stu-id="24911-132">id</span></span>|<span data-ttu-id="24911-133">String</span><span class="sxs-lookup"><span data-stu-id="24911-133">String</span></span>|<span data-ttu-id="24911-134">Identificador exclusivo do WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="24911-134">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="24911-135">applicationName</span><span class="sxs-lookup"><span data-stu-id="24911-135">applicationName</span></span>|<span data-ttu-id="24911-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="24911-136">String</span></span>|<span data-ttu-id="24911-137">Nome do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24911-137">Application Name</span></span>|
|<span data-ttu-id="24911-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="24911-138">applicationType</span></span>|[<span data-ttu-id="24911-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="24911-139">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="24911-140">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="24911-140">Application Type.</span></span> <span data-ttu-id="24911-141">Os valores possíveis são: `universal` e `desktop`.</span><span class="sxs-lookup"><span data-stu-id="24911-141">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="24911-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="24911-142">deviceCount</span></span>|<span data-ttu-id="24911-143">Int32</span><span class="sxs-lookup"><span data-stu-id="24911-143">Int32</span></span>|<span data-ttu-id="24911-144">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="24911-144">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="24911-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="24911-145">Response</span></span>
<span data-ttu-id="24911-146">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24911-146">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24911-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24911-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="24911-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24911-148">Request</span></span>
<span data-ttu-id="24911-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24911-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="24911-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="24911-150">Response</span></span>
<span data-ttu-id="24911-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24911-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




