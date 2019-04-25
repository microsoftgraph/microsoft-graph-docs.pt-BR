---
title: Atualizar windowsInformationProtectionAppLearningSummary
description: Atualizar as propriedades de um objeto windowsInformationProtectionAppLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 86d8ab048b81401fd3d4378000af89d06a7fcb5f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541154"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="60141-103">Atualizar windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="60141-103">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="60141-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="60141-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60141-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="60141-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60141-106">Atualizar as propriedades de um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="60141-106">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60141-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="60141-107">Prerequisites</span></span>
<span data-ttu-id="60141-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60141-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60141-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60141-110">Permission type</span></span>|<span data-ttu-id="60141-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="60141-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60141-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60141-112">Delegated (work or school account)</span></span>|<span data-ttu-id="60141-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60141-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="60141-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60141-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60141-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60141-115">Not supported.</span></span>|
|<span data-ttu-id="60141-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60141-116">Application</span></span>|<span data-ttu-id="60141-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60141-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60141-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60141-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="60141-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60141-119">Request headers</span></span>
|<span data-ttu-id="60141-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60141-120">Header</span></span>|<span data-ttu-id="60141-121">Valor</span><span class="sxs-lookup"><span data-stu-id="60141-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60141-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="60141-122">Authorization</span></span>|<span data-ttu-id="60141-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60141-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60141-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="60141-124">Accept</span></span>|<span data-ttu-id="60141-125">application/json</span><span class="sxs-lookup"><span data-stu-id="60141-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60141-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60141-126">Request body</span></span>
<span data-ttu-id="60141-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="60141-127">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="60141-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="60141-128">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="60141-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60141-129">Property</span></span>|<span data-ttu-id="60141-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="60141-130">Type</span></span>|<span data-ttu-id="60141-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="60141-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60141-132">id</span><span class="sxs-lookup"><span data-stu-id="60141-132">id</span></span>|<span data-ttu-id="60141-133">String</span><span class="sxs-lookup"><span data-stu-id="60141-133">String</span></span>|<span data-ttu-id="60141-134">Identificador exclusivo do WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="60141-134">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="60141-135">applicationName</span><span class="sxs-lookup"><span data-stu-id="60141-135">applicationName</span></span>|<span data-ttu-id="60141-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="60141-136">String</span></span>|<span data-ttu-id="60141-137">Nome do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60141-137">Application Name</span></span>|
|<span data-ttu-id="60141-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="60141-138">applicationType</span></span>|[<span data-ttu-id="60141-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="60141-139">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="60141-140">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="60141-140">Application Type.</span></span> <span data-ttu-id="60141-141">Os valores possíveis são: `universal` e `desktop`.</span><span class="sxs-lookup"><span data-stu-id="60141-141">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="60141-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="60141-142">deviceCount</span></span>|<span data-ttu-id="60141-143">Int32</span><span class="sxs-lookup"><span data-stu-id="60141-143">Int32</span></span>|<span data-ttu-id="60141-144">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="60141-144">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="60141-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="60141-145">Response</span></span>
<span data-ttu-id="60141-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60141-146">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60141-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60141-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="60141-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60141-148">Request</span></span>
<span data-ttu-id="60141-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60141-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="60141-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="60141-150">Response</span></span>
<span data-ttu-id="60141-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60141-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





