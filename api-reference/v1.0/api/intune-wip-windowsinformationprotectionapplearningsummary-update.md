---
title: Atualizar windowsInformationProtectionAppLearningSummary
description: Atualizar as propriedades de um objeto windowsInformationProtectionAppLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9df0f1893c17ae39649ff1ebd554059648f80ed4
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253117"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="98381-103">Atualizar windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="98381-103">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="98381-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="98381-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98381-105">Atualizar as propriedades de um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="98381-105">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98381-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="98381-106">Prerequisites</span></span>
<span data-ttu-id="98381-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="98381-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="98381-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98381-109">Permission type</span></span>|<span data-ttu-id="98381-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="98381-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98381-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98381-111">Delegated (work or school account)</span></span>|<span data-ttu-id="98381-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98381-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="98381-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98381-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98381-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98381-114">Not supported.</span></span>|
|<span data-ttu-id="98381-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98381-115">Application</span></span>|<span data-ttu-id="98381-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98381-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98381-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98381-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="98381-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98381-118">Request headers</span></span>
|<span data-ttu-id="98381-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="98381-119">Header</span></span>|<span data-ttu-id="98381-120">Valor</span><span class="sxs-lookup"><span data-stu-id="98381-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98381-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="98381-121">Authorization</span></span>|<span data-ttu-id="98381-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98381-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98381-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="98381-123">Accept</span></span>|<span data-ttu-id="98381-124">application/json</span><span class="sxs-lookup"><span data-stu-id="98381-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98381-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98381-125">Request body</span></span>
<span data-ttu-id="98381-126">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="98381-126">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="98381-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="98381-127">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="98381-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98381-128">Property</span></span>|<span data-ttu-id="98381-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="98381-129">Type</span></span>|<span data-ttu-id="98381-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="98381-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98381-131">id</span><span class="sxs-lookup"><span data-stu-id="98381-131">id</span></span>|<span data-ttu-id="98381-132">String</span><span class="sxs-lookup"><span data-stu-id="98381-132">String</span></span>|<span data-ttu-id="98381-133">Identificador exclusivo do WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="98381-133">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="98381-134">applicationName</span><span class="sxs-lookup"><span data-stu-id="98381-134">applicationName</span></span>|<span data-ttu-id="98381-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98381-135">String</span></span>|<span data-ttu-id="98381-136">Nome do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98381-136">Application Name</span></span>|
|<span data-ttu-id="98381-137">applicationType</span><span class="sxs-lookup"><span data-stu-id="98381-137">applicationType</span></span>|[<span data-ttu-id="98381-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="98381-138">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="98381-139">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="98381-139">Application Type.</span></span> <span data-ttu-id="98381-140">Os valores possíveis são: `universal` e `desktop`.</span><span class="sxs-lookup"><span data-stu-id="98381-140">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="98381-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="98381-141">deviceCount</span></span>|<span data-ttu-id="98381-142">Int32</span><span class="sxs-lookup"><span data-stu-id="98381-142">Int32</span></span>|<span data-ttu-id="98381-143">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="98381-143">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="98381-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="98381-144">Response</span></span>
<span data-ttu-id="98381-145">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98381-145">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98381-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98381-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="98381-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98381-147">Request</span></span>
<span data-ttu-id="98381-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98381-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="98381-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="98381-149">Response</span></span>
<span data-ttu-id="98381-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98381-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



