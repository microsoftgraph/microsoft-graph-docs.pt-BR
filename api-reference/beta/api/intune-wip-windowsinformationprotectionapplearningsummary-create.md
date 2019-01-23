---
title: Criar windowsInformationProtectionAppLearningSummary
description: Criar um novo objeto windowsInformationProtectionAppLearningSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3c39303154cbf09d6aedb1080d0560885e91133e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407757"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="e7c14-103">Criar windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="e7c14-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="e7c14-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e7c14-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e7c14-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e7c14-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7c14-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e7c14-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7c14-107">Criar um novo objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="e7c14-107">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7c14-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7c14-108">Prerequisites</span></span>
<span data-ttu-id="e7c14-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e7c14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e7c14-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7c14-111">Permission type</span></span>|<span data-ttu-id="e7c14-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e7c14-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7c14-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7c14-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7c14-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7c14-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e7c14-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7c14-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7c14-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7c14-116">Not supported.</span></span>|
|<span data-ttu-id="e7c14-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7c14-117">Application</span></span>|<span data-ttu-id="e7c14-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7c14-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7c14-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7c14-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="e7c14-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7c14-120">Request headers</span></span>
|<span data-ttu-id="e7c14-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7c14-121">Header</span></span>|<span data-ttu-id="e7c14-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e7c14-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7c14-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7c14-123">Authorization</span></span>|<span data-ttu-id="e7c14-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7c14-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7c14-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e7c14-125">Accept</span></span>|<span data-ttu-id="e7c14-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7c14-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7c14-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7c14-127">Request body</span></span>
<span data-ttu-id="e7c14-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="e7c14-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="e7c14-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="e7c14-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="e7c14-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7c14-130">Property</span></span>|<span data-ttu-id="e7c14-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7c14-131">Type</span></span>|<span data-ttu-id="e7c14-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7c14-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7c14-133">id</span><span class="sxs-lookup"><span data-stu-id="e7c14-133">id</span></span>|<span data-ttu-id="e7c14-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7c14-134">String</span></span>|<span data-ttu-id="e7c14-135">Identificador exclusivo do WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="e7c14-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="e7c14-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="e7c14-136">applicationName</span></span>|<span data-ttu-id="e7c14-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7c14-137">String</span></span>|<span data-ttu-id="e7c14-138">Nome do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7c14-138">Application Name</span></span>|
|<span data-ttu-id="e7c14-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="e7c14-139">applicationType</span></span>|[<span data-ttu-id="e7c14-140">applicationType</span><span class="sxs-lookup"><span data-stu-id="e7c14-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="e7c14-141">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e7c14-141">Application Type.</span></span> <span data-ttu-id="e7c14-142">Os valores possíveis são: `universal` e `desktop`.</span><span class="sxs-lookup"><span data-stu-id="e7c14-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="e7c14-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="e7c14-143">deviceCount</span></span>|<span data-ttu-id="e7c14-144">Int32</span><span class="sxs-lookup"><span data-stu-id="e7c14-144">Int32</span></span>|<span data-ttu-id="e7c14-145">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="e7c14-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="e7c14-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7c14-146">Response</span></span>
<span data-ttu-id="e7c14-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7c14-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7c14-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7c14-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7c14-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7c14-149">Request</span></span>
<span data-ttu-id="e7c14-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7c14-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e7c14-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7c14-151">Response</span></span>
<span data-ttu-id="e7c14-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7c14-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




