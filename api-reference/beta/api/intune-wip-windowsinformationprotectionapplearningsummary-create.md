---
title: Criar windowsInformationProtectionAppLearningSummary
description: Criar um novo objeto windowsInformationProtectionAppLearningSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 21d501e2edaf70bfc46ceeded315f7b65ac47634
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457381"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="063ff-103">Criar windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="063ff-103">Create windowsInformationProtectionAppLearningSummary</span></span>

<span data-ttu-id="063ff-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="063ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="063ff-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="063ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="063ff-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="063ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="063ff-107">Criar um novo objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="063ff-107">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="063ff-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="063ff-108">Prerequisites</span></span>
<span data-ttu-id="063ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="063ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="063ff-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="063ff-111">Permission type</span></span>|<span data-ttu-id="063ff-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="063ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="063ff-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="063ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="063ff-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="063ff-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="063ff-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="063ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="063ff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="063ff-116">Not supported.</span></span>|
|<span data-ttu-id="063ff-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="063ff-117">Application</span></span>|<span data-ttu-id="063ff-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="063ff-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="063ff-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="063ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="063ff-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="063ff-120">Request headers</span></span>
|<span data-ttu-id="063ff-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="063ff-121">Header</span></span>|<span data-ttu-id="063ff-122">Valor</span><span class="sxs-lookup"><span data-stu-id="063ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="063ff-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="063ff-123">Authorization</span></span>|<span data-ttu-id="063ff-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="063ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="063ff-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="063ff-125">Accept</span></span>|<span data-ttu-id="063ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="063ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="063ff-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="063ff-127">Request body</span></span>
<span data-ttu-id="063ff-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="063ff-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="063ff-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="063ff-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="063ff-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="063ff-130">Property</span></span>|<span data-ttu-id="063ff-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="063ff-131">Type</span></span>|<span data-ttu-id="063ff-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="063ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="063ff-133">id</span><span class="sxs-lookup"><span data-stu-id="063ff-133">id</span></span>|<span data-ttu-id="063ff-134">String</span><span class="sxs-lookup"><span data-stu-id="063ff-134">String</span></span>|<span data-ttu-id="063ff-135">Identificador exclusivo do WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="063ff-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="063ff-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="063ff-136">applicationName</span></span>|<span data-ttu-id="063ff-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="063ff-137">String</span></span>|<span data-ttu-id="063ff-138">Nome do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="063ff-138">Application Name</span></span>|
|<span data-ttu-id="063ff-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="063ff-139">applicationType</span></span>|[<span data-ttu-id="063ff-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="063ff-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="063ff-141">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="063ff-141">Application Type.</span></span> <span data-ttu-id="063ff-142">Os valores possíveis são: `universal` e `desktop`.</span><span class="sxs-lookup"><span data-stu-id="063ff-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="063ff-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="063ff-143">deviceCount</span></span>|<span data-ttu-id="063ff-144">Int32</span><span class="sxs-lookup"><span data-stu-id="063ff-144">Int32</span></span>|<span data-ttu-id="063ff-145">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="063ff-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="063ff-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="063ff-146">Response</span></span>
<span data-ttu-id="063ff-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="063ff-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="063ff-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="063ff-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="063ff-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="063ff-149">Request</span></span>
<span data-ttu-id="063ff-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="063ff-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="063ff-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="063ff-151">Response</span></span>
<span data-ttu-id="063ff-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="063ff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





