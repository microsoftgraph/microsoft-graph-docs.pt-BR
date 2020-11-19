---
title: Criar windowsInformationProtectionAppLearningSummary
description: Criar um novo objeto windowsInformationProtectionAppLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b353fec8d74d3b1208e0385f1dc2c5195ebfb9f1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49217274"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="30e34-103">Criar windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="30e34-103">Create windowsInformationProtectionAppLearningSummary</span></span>

<span data-ttu-id="30e34-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30e34-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30e34-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="30e34-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30e34-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30e34-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30e34-107">Criar um novo objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="30e34-107">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30e34-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="30e34-108">Prerequisites</span></span>
<span data-ttu-id="30e34-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30e34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30e34-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30e34-111">Permission type</span></span>|<span data-ttu-id="30e34-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="30e34-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30e34-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30e34-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30e34-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30e34-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="30e34-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30e34-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30e34-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30e34-116">Not supported.</span></span>|
|<span data-ttu-id="30e34-117">Application</span><span class="sxs-lookup"><span data-stu-id="30e34-117">Application</span></span>|<span data-ttu-id="30e34-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30e34-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30e34-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30e34-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="30e34-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30e34-120">Request headers</span></span>
|<span data-ttu-id="30e34-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30e34-121">Header</span></span>|<span data-ttu-id="30e34-122">Valor</span><span class="sxs-lookup"><span data-stu-id="30e34-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30e34-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="30e34-123">Authorization</span></span>|<span data-ttu-id="30e34-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30e34-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30e34-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="30e34-125">Accept</span></span>|<span data-ttu-id="30e34-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30e34-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30e34-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30e34-127">Request body</span></span>
<span data-ttu-id="30e34-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="30e34-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="30e34-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="30e34-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="30e34-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30e34-130">Property</span></span>|<span data-ttu-id="30e34-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="30e34-131">Type</span></span>|<span data-ttu-id="30e34-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="30e34-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30e34-133">id</span><span class="sxs-lookup"><span data-stu-id="30e34-133">id</span></span>|<span data-ttu-id="30e34-134">String</span><span class="sxs-lookup"><span data-stu-id="30e34-134">String</span></span>|<span data-ttu-id="30e34-135">Identificador exclusivo do WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="30e34-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="30e34-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="30e34-136">applicationName</span></span>|<span data-ttu-id="30e34-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="30e34-137">String</span></span>|<span data-ttu-id="30e34-138">Nome do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30e34-138">Application Name</span></span>|
|<span data-ttu-id="30e34-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="30e34-139">applicationType</span></span>|[<span data-ttu-id="30e34-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="30e34-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="30e34-141">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30e34-141">Application Type.</span></span> <span data-ttu-id="30e34-142">Os valores possíveis são: `universal` e `desktop`.</span><span class="sxs-lookup"><span data-stu-id="30e34-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="30e34-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="30e34-143">deviceCount</span></span>|<span data-ttu-id="30e34-144">Int32</span><span class="sxs-lookup"><span data-stu-id="30e34-144">Int32</span></span>|<span data-ttu-id="30e34-145">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="30e34-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="30e34-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="30e34-146">Response</span></span>
<span data-ttu-id="30e34-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30e34-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30e34-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30e34-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="30e34-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30e34-149">Request</span></span>
<span data-ttu-id="30e34-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30e34-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="30e34-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="30e34-151">Response</span></span>
<span data-ttu-id="30e34-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30e34-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




