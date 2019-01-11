---
title: Criar windowsInformationProtectionAppLearningSummary
description: Criar um novo objeto windowsInformationProtectionAppLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9823b3006cdecd787990869ffb58ee0ff3ad97c1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862731"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="4d80b-103">Criar windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="4d80b-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="4d80b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4d80b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d80b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4d80b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d80b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4d80b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d80b-107">Criar um novo objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="4d80b-107">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4d80b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4d80b-108">Prerequisites</span></span>
<span data-ttu-id="4d80b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d80b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d80b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d80b-111">Permission type</span></span>|<span data-ttu-id="4d80b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4d80b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d80b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d80b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4d80b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d80b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4d80b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d80b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d80b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d80b-116">Not supported.</span></span>|
|<span data-ttu-id="4d80b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d80b-117">Application</span></span>|<span data-ttu-id="4d80b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d80b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d80b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d80b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="4d80b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d80b-120">Request headers</span></span>
|<span data-ttu-id="4d80b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4d80b-121">Header</span></span>|<span data-ttu-id="4d80b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4d80b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d80b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d80b-123">Authorization</span></span>|<span data-ttu-id="4d80b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d80b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d80b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4d80b-125">Accept</span></span>|<span data-ttu-id="4d80b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d80b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d80b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d80b-127">Request body</span></span>
<span data-ttu-id="4d80b-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="4d80b-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="4d80b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="4d80b-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="4d80b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d80b-130">Property</span></span>|<span data-ttu-id="4d80b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d80b-131">Type</span></span>|<span data-ttu-id="4d80b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d80b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d80b-133">id</span><span class="sxs-lookup"><span data-stu-id="4d80b-133">id</span></span>|<span data-ttu-id="4d80b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d80b-134">String</span></span>|<span data-ttu-id="4d80b-135">Identificador exclusivo do WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="4d80b-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="4d80b-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="4d80b-136">applicationName</span></span>|<span data-ttu-id="4d80b-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d80b-137">String</span></span>|<span data-ttu-id="4d80b-138">Nome do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d80b-138">Application Name</span></span>|
|<span data-ttu-id="4d80b-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="4d80b-139">applicationType</span></span>|[<span data-ttu-id="4d80b-140">applicationType</span><span class="sxs-lookup"><span data-stu-id="4d80b-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="4d80b-141">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4d80b-141">Application Type.</span></span> <span data-ttu-id="4d80b-142">Os valores possíveis são: `universal` e `desktop`.</span><span class="sxs-lookup"><span data-stu-id="4d80b-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="4d80b-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="4d80b-143">deviceCount</span></span>|<span data-ttu-id="4d80b-144">Int32</span><span class="sxs-lookup"><span data-stu-id="4d80b-144">Int32</span></span>|<span data-ttu-id="4d80b-145">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="4d80b-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="4d80b-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d80b-146">Response</span></span>
<span data-ttu-id="4d80b-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d80b-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d80b-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d80b-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="4d80b-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d80b-149">Request</span></span>
<span data-ttu-id="4d80b-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d80b-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4d80b-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d80b-151">Response</span></span>
<span data-ttu-id="4d80b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d80b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





