---
title: Criar windowsInformationProtectionAppLearningSummary
description: Criar um novo objeto windowsInformationProtectionAppLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 530851bda5175cc488232051c51b395d0cd5a910
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455302"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="01891-103">Criar windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="01891-103">Create windowsInformationProtectionAppLearningSummary</span></span>

<span data-ttu-id="01891-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01891-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01891-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="01891-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01891-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="01891-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01891-107">Criar um novo objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="01891-107">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01891-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="01891-108">Prerequisites</span></span>
<span data-ttu-id="01891-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01891-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01891-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01891-111">Permission type</span></span>|<span data-ttu-id="01891-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="01891-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01891-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01891-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01891-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01891-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="01891-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01891-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01891-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01891-116">Not supported.</span></span>|
|<span data-ttu-id="01891-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01891-117">Application</span></span>|<span data-ttu-id="01891-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01891-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01891-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01891-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="01891-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01891-120">Request headers</span></span>
|<span data-ttu-id="01891-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01891-121">Header</span></span>|<span data-ttu-id="01891-122">Valor</span><span class="sxs-lookup"><span data-stu-id="01891-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01891-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="01891-123">Authorization</span></span>|<span data-ttu-id="01891-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01891-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01891-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="01891-125">Accept</span></span>|<span data-ttu-id="01891-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01891-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01891-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01891-127">Request body</span></span>
<span data-ttu-id="01891-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="01891-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="01891-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="01891-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="01891-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01891-130">Property</span></span>|<span data-ttu-id="01891-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="01891-131">Type</span></span>|<span data-ttu-id="01891-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="01891-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01891-133">id</span><span class="sxs-lookup"><span data-stu-id="01891-133">id</span></span>|<span data-ttu-id="01891-134">String</span><span class="sxs-lookup"><span data-stu-id="01891-134">String</span></span>|<span data-ttu-id="01891-135">Identificador exclusivo do WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="01891-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="01891-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="01891-136">applicationName</span></span>|<span data-ttu-id="01891-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01891-137">String</span></span>|<span data-ttu-id="01891-138">Nome do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01891-138">Application Name</span></span>|
|<span data-ttu-id="01891-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="01891-139">applicationType</span></span>|[<span data-ttu-id="01891-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="01891-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="01891-141">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="01891-141">Application Type.</span></span> <span data-ttu-id="01891-142">Os valores possíveis são: `universal` e `desktop`.</span><span class="sxs-lookup"><span data-stu-id="01891-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="01891-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="01891-143">deviceCount</span></span>|<span data-ttu-id="01891-144">Int32</span><span class="sxs-lookup"><span data-stu-id="01891-144">Int32</span></span>|<span data-ttu-id="01891-145">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="01891-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="01891-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="01891-146">Response</span></span>
<span data-ttu-id="01891-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01891-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01891-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01891-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="01891-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01891-149">Request</span></span>
<span data-ttu-id="01891-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01891-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="01891-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="01891-151">Response</span></span>
<span data-ttu-id="01891-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01891-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



