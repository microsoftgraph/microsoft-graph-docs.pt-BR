---
title: Criar windowsInformationProtectionAppLearningSummary
description: Criar um novo objeto windowsInformationProtectionAppLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1a85aaf4b6ab81b025927038d5620a9c6010aa43
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144862"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="6d1b1-103">Criar windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="6d1b1-103">Create windowsInformationProtectionAppLearningSummary</span></span>

<span data-ttu-id="6d1b1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d1b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d1b1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6d1b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d1b1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d1b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d1b1-107">Criar um novo objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="6d1b1-107">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d1b1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6d1b1-108">Prerequisites</span></span>
<span data-ttu-id="6d1b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d1b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d1b1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d1b1-111">Permission type</span></span>|<span data-ttu-id="6d1b1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d1b1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d1b1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d1b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6d1b1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d1b1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6d1b1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d1b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d1b1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d1b1-116">Not supported.</span></span>|
|<span data-ttu-id="6d1b1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d1b1-117">Application</span></span>|<span data-ttu-id="6d1b1-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d1b1-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d1b1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d1b1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="6d1b1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d1b1-120">Request headers</span></span>
|<span data-ttu-id="6d1b1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6d1b1-121">Header</span></span>|<span data-ttu-id="6d1b1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6d1b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d1b1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d1b1-123">Authorization</span></span>|<span data-ttu-id="6d1b1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d1b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d1b1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6d1b1-125">Accept</span></span>|<span data-ttu-id="6d1b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d1b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d1b1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d1b1-127">Request body</span></span>
<span data-ttu-id="6d1b1-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="6d1b1-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="6d1b1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="6d1b1-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="6d1b1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d1b1-130">Property</span></span>|<span data-ttu-id="6d1b1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d1b1-131">Type</span></span>|<span data-ttu-id="6d1b1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d1b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d1b1-133">id</span><span class="sxs-lookup"><span data-stu-id="6d1b1-133">id</span></span>|<span data-ttu-id="6d1b1-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d1b1-134">String</span></span>|<span data-ttu-id="6d1b1-135">Identificador exclusivo do WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="6d1b1-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="6d1b1-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="6d1b1-136">applicationName</span></span>|<span data-ttu-id="6d1b1-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d1b1-137">String</span></span>|<span data-ttu-id="6d1b1-138">Nome do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d1b1-138">Application Name</span></span>|
|<span data-ttu-id="6d1b1-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="6d1b1-139">applicationType</span></span>|[<span data-ttu-id="6d1b1-140">applicationType</span><span class="sxs-lookup"><span data-stu-id="6d1b1-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="6d1b1-141">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6d1b1-141">Application Type.</span></span> <span data-ttu-id="6d1b1-142">Os valores possíveis são: `universal` e `desktop`.</span><span class="sxs-lookup"><span data-stu-id="6d1b1-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="6d1b1-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="6d1b1-143">deviceCount</span></span>|<span data-ttu-id="6d1b1-144">Int32</span><span class="sxs-lookup"><span data-stu-id="6d1b1-144">Int32</span></span>|<span data-ttu-id="6d1b1-145">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="6d1b1-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="6d1b1-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d1b1-146">Response</span></span>
<span data-ttu-id="6d1b1-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d1b1-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d1b1-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d1b1-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d1b1-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d1b1-149">Request</span></span>
<span data-ttu-id="6d1b1-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d1b1-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6d1b1-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d1b1-151">Response</span></span>
<span data-ttu-id="6d1b1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d1b1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




