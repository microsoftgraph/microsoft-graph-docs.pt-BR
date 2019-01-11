---
title: Atualizar windowsInformationProtectionAppLearningSummary
description: Atualizar as propriedades de um objeto windowsInformationProtectionAppLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 052a18270aab27603969d8abaeec88f86f0bc5e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882905"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="bafa9-103">Atualizar windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="bafa9-103">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="bafa9-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bafa9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bafa9-105">Atualizar as propriedades de um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="bafa9-105">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bafa9-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bafa9-106">Prerequisites</span></span>
<span data-ttu-id="bafa9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bafa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bafa9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bafa9-109">Permission type</span></span>|<span data-ttu-id="bafa9-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bafa9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bafa9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bafa9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bafa9-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bafa9-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bafa9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bafa9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bafa9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bafa9-114">Not supported.</span></span>|
|<span data-ttu-id="bafa9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bafa9-115">Application</span></span>|<span data-ttu-id="bafa9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bafa9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bafa9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bafa9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="bafa9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bafa9-118">Request headers</span></span>
|<span data-ttu-id="bafa9-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bafa9-119">Header</span></span>|<span data-ttu-id="bafa9-120">Valor</span><span class="sxs-lookup"><span data-stu-id="bafa9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bafa9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bafa9-121">Authorization</span></span>|<span data-ttu-id="bafa9-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bafa9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bafa9-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bafa9-123">Accept</span></span>|<span data-ttu-id="bafa9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bafa9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bafa9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bafa9-125">Request body</span></span>
<span data-ttu-id="bafa9-126">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="bafa9-126">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="bafa9-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="bafa9-127">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="bafa9-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bafa9-128">Property</span></span>|<span data-ttu-id="bafa9-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="bafa9-129">Type</span></span>|<span data-ttu-id="bafa9-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="bafa9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bafa9-131">id</span><span class="sxs-lookup"><span data-stu-id="bafa9-131">id</span></span>|<span data-ttu-id="bafa9-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bafa9-132">String</span></span>|<span data-ttu-id="bafa9-133">Identificador exclusivo do WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="bafa9-133">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="bafa9-134">applicationName</span><span class="sxs-lookup"><span data-stu-id="bafa9-134">applicationName</span></span>|<span data-ttu-id="bafa9-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bafa9-135">String</span></span>|<span data-ttu-id="bafa9-136">Nome do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bafa9-136">Application Name</span></span>|
|<span data-ttu-id="bafa9-137">applicationType</span><span class="sxs-lookup"><span data-stu-id="bafa9-137">applicationType</span></span>|[<span data-ttu-id="bafa9-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="bafa9-138">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="bafa9-139">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bafa9-139">Application Type.</span></span> <span data-ttu-id="bafa9-140">Os valores possíveis são: `universal` e `desktop`.</span><span class="sxs-lookup"><span data-stu-id="bafa9-140">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="bafa9-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="bafa9-141">deviceCount</span></span>|<span data-ttu-id="bafa9-142">Int32</span><span class="sxs-lookup"><span data-stu-id="bafa9-142">Int32</span></span>|<span data-ttu-id="bafa9-143">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="bafa9-143">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="bafa9-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="bafa9-144">Response</span></span>
<span data-ttu-id="bafa9-145">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bafa9-145">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bafa9-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bafa9-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="bafa9-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bafa9-147">Request</span></span>
<span data-ttu-id="bafa9-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bafa9-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bafa9-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="bafa9-149">Response</span></span>
<span data-ttu-id="bafa9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bafa9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



