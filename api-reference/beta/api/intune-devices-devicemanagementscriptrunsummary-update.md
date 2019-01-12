---
title: Atualizar deviceManagementScriptRunSummary
description: Atualize as propriedades de um objeto deviceManagementScriptRunSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d2a0ba2a7dfbd44cd5e756010239caee285fe090
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954698"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="b5a94-103">Atualizar deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="b5a94-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="b5a94-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b5a94-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5a94-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b5a94-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5a94-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b5a94-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5a94-107">Atualize as propriedades de um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="b5a94-107">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b5a94-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b5a94-108">Prerequisites</span></span>
<span data-ttu-id="b5a94-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5a94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5a94-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5a94-111">Permission type</span></span>|<span data-ttu-id="b5a94-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b5a94-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5a94-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5a94-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5a94-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5a94-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b5a94-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5a94-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5a94-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5a94-116">Not supported.</span></span>|
|<span data-ttu-id="b5a94-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5a94-117">Application</span></span>|<span data-ttu-id="b5a94-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5a94-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5a94-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5a94-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="b5a94-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5a94-120">Request headers</span></span>
|<span data-ttu-id="b5a94-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b5a94-121">Header</span></span>|<span data-ttu-id="b5a94-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b5a94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5a94-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5a94-123">Authorization</span></span>|<span data-ttu-id="b5a94-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5a94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5a94-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b5a94-125">Accept</span></span>|<span data-ttu-id="b5a94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b5a94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5a94-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5a94-127">Request body</span></span>
<span data-ttu-id="b5a94-128">No corpo da solicitação, fornece uma representação JSON para o objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="b5a94-128">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="b5a94-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="b5a94-129">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="b5a94-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5a94-130">Property</span></span>|<span data-ttu-id="b5a94-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5a94-131">Type</span></span>|<span data-ttu-id="b5a94-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5a94-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5a94-133">id</span><span class="sxs-lookup"><span data-stu-id="b5a94-133">id</span></span>|<span data-ttu-id="b5a94-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5a94-134">String</span></span>|<span data-ttu-id="b5a94-135">Chave do script de gerenciamento de dispositivo execute entidade resumida.</span><span class="sxs-lookup"><span data-stu-id="b5a94-135">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="b5a94-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b5a94-136">successDeviceCount</span></span>|<span data-ttu-id="b5a94-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b5a94-137">Int32</span></span>|<span data-ttu-id="b5a94-138">Contagem de sucesso do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b5a94-138">Success device count.</span></span>|
|<span data-ttu-id="b5a94-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b5a94-139">errorDeviceCount</span></span>|<span data-ttu-id="b5a94-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b5a94-140">Int32</span></span>|<span data-ttu-id="b5a94-141">Contagem de erros de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b5a94-141">Error device count.</span></span>|
|<span data-ttu-id="b5a94-142">successUserCount</span><span class="sxs-lookup"><span data-stu-id="b5a94-142">successUserCount</span></span>|<span data-ttu-id="b5a94-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b5a94-143">Int32</span></span>|<span data-ttu-id="b5a94-144">Contagem de usuário de sucesso.</span><span class="sxs-lookup"><span data-stu-id="b5a94-144">Success user count.</span></span>|
|<span data-ttu-id="b5a94-145">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="b5a94-145">errorUserCount</span></span>|<span data-ttu-id="b5a94-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b5a94-146">Int32</span></span>|<span data-ttu-id="b5a94-147">Contagem de erros de usuário.</span><span class="sxs-lookup"><span data-stu-id="b5a94-147">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="b5a94-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5a94-148">Response</span></span>
<span data-ttu-id="b5a94-149">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5a94-149">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5a94-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5a94-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="b5a94-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5a94-151">Request</span></span>
<span data-ttu-id="b5a94-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5a94-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b5a94-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5a94-153">Response</span></span>
<span data-ttu-id="b5a94-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5a94-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





