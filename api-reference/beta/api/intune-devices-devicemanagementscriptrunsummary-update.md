---
title: Atualizar deviceManagementScriptRunSummary
description: Atualize as propriedades de um objeto deviceManagementScriptRunSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c7a82b01ccae7e3f5ca1e8c3b3b784791fe08df3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858321"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="ed43e-103">Atualizar deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="ed43e-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="ed43e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ed43e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed43e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ed43e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed43e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ed43e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed43e-107">Atualize as propriedades de um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="ed43e-107">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed43e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ed43e-108">Prerequisites</span></span>
<span data-ttu-id="ed43e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed43e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed43e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed43e-111">Permission type</span></span>|<span data-ttu-id="ed43e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ed43e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed43e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed43e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed43e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed43e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ed43e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed43e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed43e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed43e-116">Not supported.</span></span>|
|<span data-ttu-id="ed43e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed43e-117">Application</span></span>|<span data-ttu-id="ed43e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed43e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed43e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed43e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="ed43e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed43e-120">Request headers</span></span>
|<span data-ttu-id="ed43e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed43e-121">Header</span></span>|<span data-ttu-id="ed43e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ed43e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed43e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed43e-123">Authorization</span></span>|<span data-ttu-id="ed43e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed43e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed43e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ed43e-125">Accept</span></span>|<span data-ttu-id="ed43e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed43e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed43e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed43e-127">Request body</span></span>
<span data-ttu-id="ed43e-128">No corpo da solicitação, fornece uma representação JSON para o objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="ed43e-128">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="ed43e-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="ed43e-129">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="ed43e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed43e-130">Property</span></span>|<span data-ttu-id="ed43e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed43e-131">Type</span></span>|<span data-ttu-id="ed43e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed43e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed43e-133">id</span><span class="sxs-lookup"><span data-stu-id="ed43e-133">id</span></span>|<span data-ttu-id="ed43e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed43e-134">String</span></span>|<span data-ttu-id="ed43e-135">Chave do script de gerenciamento de dispositivo execute entidade resumida.</span><span class="sxs-lookup"><span data-stu-id="ed43e-135">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="ed43e-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed43e-136">successDeviceCount</span></span>|<span data-ttu-id="ed43e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ed43e-137">Int32</span></span>|<span data-ttu-id="ed43e-138">Contagem de sucesso do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ed43e-138">Success device count.</span></span>|
|<span data-ttu-id="ed43e-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed43e-139">errorDeviceCount</span></span>|<span data-ttu-id="ed43e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ed43e-140">Int32</span></span>|<span data-ttu-id="ed43e-141">Contagem de erros de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ed43e-141">Error device count.</span></span>|
|<span data-ttu-id="ed43e-142">successUserCount</span><span class="sxs-lookup"><span data-stu-id="ed43e-142">successUserCount</span></span>|<span data-ttu-id="ed43e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ed43e-143">Int32</span></span>|<span data-ttu-id="ed43e-144">Contagem de usuário de sucesso.</span><span class="sxs-lookup"><span data-stu-id="ed43e-144">Success user count.</span></span>|
|<span data-ttu-id="ed43e-145">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="ed43e-145">errorUserCount</span></span>|<span data-ttu-id="ed43e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ed43e-146">Int32</span></span>|<span data-ttu-id="ed43e-147">Contagem de erros de usuário.</span><span class="sxs-lookup"><span data-stu-id="ed43e-147">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="ed43e-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed43e-148">Response</span></span>
<span data-ttu-id="ed43e-149">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed43e-149">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed43e-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed43e-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed43e-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed43e-151">Request</span></span>
<span data-ttu-id="ed43e-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed43e-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
Content-type: application/json
Content-length: 108

{
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```

### <a name="response"></a><span data-ttu-id="ed43e-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed43e-153">Response</span></span>
<span data-ttu-id="ed43e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed43e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "514d5d38-5d38-514d-385d-4d51385d4d51",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```





