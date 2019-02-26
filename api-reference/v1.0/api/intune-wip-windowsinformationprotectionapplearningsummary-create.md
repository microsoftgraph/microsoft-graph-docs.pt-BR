---
title: Criar windowsInformationProtectionAppLearningSummary
description: Criar um novo objeto windowsInformationProtectionAppLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 30cfe88f6e0a8a72e1a373b0f867357c63138f42
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260253"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="65a5c-103">Criar windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="65a5c-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="65a5c-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="65a5c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65a5c-105">Criar um novo objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="65a5c-105">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65a5c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="65a5c-106">Prerequisites</span></span>
<span data-ttu-id="65a5c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="65a5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="65a5c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65a5c-109">Permission type</span></span>|<span data-ttu-id="65a5c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="65a5c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65a5c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65a5c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="65a5c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65a5c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="65a5c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65a5c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65a5c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65a5c-114">Not supported.</span></span>|
|<span data-ttu-id="65a5c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65a5c-115">Application</span></span>|<span data-ttu-id="65a5c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65a5c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65a5c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65a5c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="65a5c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65a5c-118">Request headers</span></span>
|<span data-ttu-id="65a5c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="65a5c-119">Header</span></span>|<span data-ttu-id="65a5c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="65a5c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65a5c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="65a5c-121">Authorization</span></span>|<span data-ttu-id="65a5c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65a5c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65a5c-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="65a5c-123">Accept</span></span>|<span data-ttu-id="65a5c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="65a5c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65a5c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65a5c-125">Request body</span></span>
<span data-ttu-id="65a5c-126">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="65a5c-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="65a5c-127">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="65a5c-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="65a5c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65a5c-128">Property</span></span>|<span data-ttu-id="65a5c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="65a5c-129">Type</span></span>|<span data-ttu-id="65a5c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="65a5c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65a5c-131">id</span><span class="sxs-lookup"><span data-stu-id="65a5c-131">id</span></span>|<span data-ttu-id="65a5c-132">String</span><span class="sxs-lookup"><span data-stu-id="65a5c-132">String</span></span>|<span data-ttu-id="65a5c-133">Identificador exclusivo do WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="65a5c-133">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="65a5c-134">applicationName</span><span class="sxs-lookup"><span data-stu-id="65a5c-134">applicationName</span></span>|<span data-ttu-id="65a5c-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65a5c-135">String</span></span>|<span data-ttu-id="65a5c-136">Nome do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65a5c-136">Application Name</span></span>|
|<span data-ttu-id="65a5c-137">applicationType</span><span class="sxs-lookup"><span data-stu-id="65a5c-137">applicationType</span></span>|[<span data-ttu-id="65a5c-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="65a5c-138">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="65a5c-139">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="65a5c-139">Application Type.</span></span> <span data-ttu-id="65a5c-140">Os valores possíveis são: `universal` e `desktop`.</span><span class="sxs-lookup"><span data-stu-id="65a5c-140">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="65a5c-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="65a5c-141">deviceCount</span></span>|<span data-ttu-id="65a5c-142">Int32</span><span class="sxs-lookup"><span data-stu-id="65a5c-142">Int32</span></span>|<span data-ttu-id="65a5c-143">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="65a5c-143">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="65a5c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="65a5c-144">Response</span></span>
<span data-ttu-id="65a5c-145">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65a5c-145">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65a5c-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65a5c-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="65a5c-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65a5c-147">Request</span></span>
<span data-ttu-id="65a5c-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="65a5c-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="65a5c-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="65a5c-149">Response</span></span>
<span data-ttu-id="65a5c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65a5c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



