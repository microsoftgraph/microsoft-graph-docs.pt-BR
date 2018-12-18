---
title: Criar windowsInformationProtectionAppLearningSummary
description: Criar um novo objeto windowsInformationProtectionAppLearningSummary.
author: tfitzmac
ms.openlocfilehash: fdcf4be10f26036c06f4cfd0a67f98601c296ec7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354296"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="e44ad-103">Criar windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="e44ad-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="e44ad-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e44ad-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e44ad-105">Criar um novo objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="e44ad-105">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e44ad-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e44ad-106">Prerequisites</span></span>
<span data-ttu-id="e44ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e44ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e44ad-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e44ad-109">Permission type</span></span>|<span data-ttu-id="e44ad-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e44ad-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e44ad-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e44ad-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e44ad-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e44ad-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e44ad-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e44ad-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e44ad-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e44ad-114">Not supported.</span></span>|
|<span data-ttu-id="e44ad-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e44ad-115">Application</span></span>|<span data-ttu-id="e44ad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e44ad-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e44ad-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e44ad-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="e44ad-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e44ad-118">Request headers</span></span>
|<span data-ttu-id="e44ad-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e44ad-119">Header</span></span>|<span data-ttu-id="e44ad-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e44ad-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e44ad-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e44ad-121">Authorization</span></span>|<span data-ttu-id="e44ad-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e44ad-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e44ad-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e44ad-123">Accept</span></span>|<span data-ttu-id="e44ad-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e44ad-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e44ad-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e44ad-125">Request body</span></span>
<span data-ttu-id="e44ad-126">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="e44ad-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="e44ad-127">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="e44ad-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="e44ad-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e44ad-128">Property</span></span>|<span data-ttu-id="e44ad-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e44ad-129">Type</span></span>|<span data-ttu-id="e44ad-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e44ad-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e44ad-131">id</span><span class="sxs-lookup"><span data-stu-id="e44ad-131">id</span></span>|<span data-ttu-id="e44ad-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e44ad-132">String</span></span>|<span data-ttu-id="e44ad-133">Identificador exclusivo do WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="e44ad-133">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="e44ad-134">applicationName</span><span class="sxs-lookup"><span data-stu-id="e44ad-134">applicationName</span></span>|<span data-ttu-id="e44ad-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e44ad-135">String</span></span>|<span data-ttu-id="e44ad-136">Nome do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e44ad-136">Application Name</span></span>|
|<span data-ttu-id="e44ad-137">applicationType</span><span class="sxs-lookup"><span data-stu-id="e44ad-137">applicationType</span></span>|[<span data-ttu-id="e44ad-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="e44ad-138">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="e44ad-139">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e44ad-139">Application Type.</span></span> <span data-ttu-id="e44ad-140">Os valores possíveis são: `universal` e `desktop`.</span><span class="sxs-lookup"><span data-stu-id="e44ad-140">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="e44ad-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="e44ad-141">deviceCount</span></span>|<span data-ttu-id="e44ad-142">Int32</span><span class="sxs-lookup"><span data-stu-id="e44ad-142">Int32</span></span>|<span data-ttu-id="e44ad-143">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="e44ad-143">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="e44ad-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="e44ad-144">Response</span></span>
<span data-ttu-id="e44ad-145">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e44ad-145">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e44ad-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e44ad-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="e44ad-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e44ad-147">Request</span></span>
<span data-ttu-id="e44ad-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e44ad-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e44ad-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="e44ad-149">Response</span></span>
<span data-ttu-id="e44ad-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e44ad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



