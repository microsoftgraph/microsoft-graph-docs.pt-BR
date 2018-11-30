---
title: Criar windowsInformationProtectionAppLearningSummary
description: Criar um novo objeto windowsInformationProtectionAppLearningSummary.
ms.openlocfilehash: 03a03e0e32115cd0f5b2f56e652c608073db7d94
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005356"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="45b52-103">Criar windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="45b52-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="45b52-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="45b52-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45b52-105">Criar um novo objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="45b52-105">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45b52-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45b52-106">Prerequisites</span></span>
<span data-ttu-id="45b52-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45b52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45b52-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45b52-109">Permission type</span></span>|<span data-ttu-id="45b52-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="45b52-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45b52-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45b52-111">Delegated (work or school account)</span></span>|<span data-ttu-id="45b52-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45b52-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="45b52-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45b52-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45b52-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45b52-114">Not supported.</span></span>|
|<span data-ttu-id="45b52-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45b52-115">Application</span></span>|<span data-ttu-id="45b52-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45b52-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45b52-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45b52-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="45b52-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45b52-118">Request headers</span></span>
|<span data-ttu-id="45b52-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45b52-119">Header</span></span>|<span data-ttu-id="45b52-120">Valor</span><span class="sxs-lookup"><span data-stu-id="45b52-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45b52-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="45b52-121">Authorization</span></span>|<span data-ttu-id="45b52-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45b52-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45b52-123">Accept</span><span class="sxs-lookup"><span data-stu-id="45b52-123">Accept</span></span>|<span data-ttu-id="45b52-124">application/json</span><span class="sxs-lookup"><span data-stu-id="45b52-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45b52-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45b52-125">Request body</span></span>
<span data-ttu-id="45b52-126">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="45b52-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="45b52-127">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="45b52-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="45b52-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45b52-128">Property</span></span>|<span data-ttu-id="45b52-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="45b52-129">Type</span></span>|<span data-ttu-id="45b52-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="45b52-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45b52-131">id</span><span class="sxs-lookup"><span data-stu-id="45b52-131">id</span></span>|<span data-ttu-id="45b52-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45b52-132">String</span></span>|<span data-ttu-id="45b52-133">Identificador exclusivo do WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="45b52-133">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="45b52-134">applicationName</span><span class="sxs-lookup"><span data-stu-id="45b52-134">applicationName</span></span>|<span data-ttu-id="45b52-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45b52-135">String</span></span>|<span data-ttu-id="45b52-136">Nome do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45b52-136">Application Name</span></span>|
|<span data-ttu-id="45b52-137">applicationType</span><span class="sxs-lookup"><span data-stu-id="45b52-137">applicationType</span></span>|[<span data-ttu-id="45b52-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="45b52-138">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="45b52-139">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="45b52-139">Application Type.</span></span> <span data-ttu-id="45b52-140">Os valores possíveis são: `universal` e `desktop`.</span><span class="sxs-lookup"><span data-stu-id="45b52-140">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="45b52-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="45b52-141">deviceCount</span></span>|<span data-ttu-id="45b52-142">Int32</span><span class="sxs-lookup"><span data-stu-id="45b52-142">Int32</span></span>|<span data-ttu-id="45b52-143">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="45b52-143">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="45b52-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="45b52-144">Response</span></span>
<span data-ttu-id="45b52-145">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45b52-145">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45b52-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45b52-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="45b52-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45b52-147">Request</span></span>
<span data-ttu-id="45b52-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45b52-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="45b52-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="45b52-149">Response</span></span>
<span data-ttu-id="45b52-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45b52-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



