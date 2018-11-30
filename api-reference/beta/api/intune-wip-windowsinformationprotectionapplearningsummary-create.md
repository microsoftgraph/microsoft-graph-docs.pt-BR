---
title: Criar windowsInformationProtectionAppLearningSummary
description: Criar um novo objeto windowsInformationProtectionAppLearningSummary.
ms.openlocfilehash: 671ab1efd631541871623fd1687639dd3d8d95ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040031"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="d3f90-103">Criar windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="d3f90-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="d3f90-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d3f90-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3f90-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d3f90-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d3f90-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d3f90-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3f90-107">Criar um novo objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="d3f90-107">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d3f90-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3f90-108">Prerequisites</span></span>
<span data-ttu-id="d3f90-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3f90-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3f90-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3f90-111">Permission type</span></span>|<span data-ttu-id="d3f90-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3f90-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3f90-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3f90-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3f90-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3f90-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d3f90-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3f90-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3f90-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3f90-116">Not supported.</span></span>|
|<span data-ttu-id="d3f90-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3f90-117">Application</span></span>|<span data-ttu-id="d3f90-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3f90-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3f90-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3f90-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="d3f90-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3f90-120">Request headers</span></span>
|<span data-ttu-id="d3f90-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3f90-121">Header</span></span>|<span data-ttu-id="d3f90-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d3f90-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3f90-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3f90-123">Authorization</span></span>|<span data-ttu-id="d3f90-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3f90-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3f90-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d3f90-125">Accept</span></span>|<span data-ttu-id="d3f90-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3f90-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3f90-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3f90-127">Request body</span></span>
<span data-ttu-id="d3f90-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="d3f90-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="d3f90-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="d3f90-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="d3f90-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3f90-130">Property</span></span>|<span data-ttu-id="d3f90-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3f90-131">Type</span></span>|<span data-ttu-id="d3f90-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3f90-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3f90-133">id</span><span class="sxs-lookup"><span data-stu-id="d3f90-133">id</span></span>|<span data-ttu-id="d3f90-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3f90-134">String</span></span>|<span data-ttu-id="d3f90-135">Identificador exclusivo do WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="d3f90-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="d3f90-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="d3f90-136">applicationName</span></span>|<span data-ttu-id="d3f90-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3f90-137">String</span></span>|<span data-ttu-id="d3f90-138">Nome do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3f90-138">Application Name</span></span>|
|<span data-ttu-id="d3f90-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="d3f90-139">applicationType</span></span>|[<span data-ttu-id="d3f90-140">applicationType</span><span class="sxs-lookup"><span data-stu-id="d3f90-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="d3f90-141">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3f90-141">Application Type.</span></span> <span data-ttu-id="d3f90-142">Os valores possíveis são: `universal` e `desktop`.</span><span class="sxs-lookup"><span data-stu-id="d3f90-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="d3f90-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="d3f90-143">deviceCount</span></span>|<span data-ttu-id="d3f90-144">Int32</span><span class="sxs-lookup"><span data-stu-id="d3f90-144">Int32</span></span>|<span data-ttu-id="d3f90-145">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="d3f90-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="d3f90-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3f90-146">Response</span></span>
<span data-ttu-id="d3f90-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3f90-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3f90-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3f90-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="d3f90-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3f90-149">Request</span></span>
<span data-ttu-id="d3f90-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3f90-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d3f90-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3f90-151">Response</span></span>
<span data-ttu-id="d3f90-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3f90-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





