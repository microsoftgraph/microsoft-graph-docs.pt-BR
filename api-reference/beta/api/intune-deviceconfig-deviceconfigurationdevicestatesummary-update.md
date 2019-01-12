---
title: Atualizar deviceConfigurationDeviceStateSummary
description: Atualizar as propriedades de um objeto deviceConfigurationDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 599411d60bc723e95297926c600359bda3c70fc1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924591"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="e3e2f-103">Atualizar deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e3e2f-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="e3e2f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e3e2f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3e2f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e3e2f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3e2f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e3e2f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3e2f-107">Atualizar as propriedades de um objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e3e2f-107">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3e2f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e3e2f-108">Prerequisites</span></span>
<span data-ttu-id="e3e2f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3e2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3e2f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3e2f-111">Permission type</span></span>|<span data-ttu-id="e3e2f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e3e2f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3e2f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3e2f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3e2f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3e2f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e3e2f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3e2f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3e2f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3e2f-116">Not supported.</span></span>|
|<span data-ttu-id="e3e2f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3e2f-117">Application</span></span>|<span data-ttu-id="e3e2f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3e2f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3e2f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3e2f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="e3e2f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3e2f-120">Request headers</span></span>
|<span data-ttu-id="e3e2f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e3e2f-121">Header</span></span>|<span data-ttu-id="e3e2f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e3e2f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3e2f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3e2f-123">Authorization</span></span>|<span data-ttu-id="e3e2f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3e2f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3e2f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e3e2f-125">Accept</span></span>|<span data-ttu-id="e3e2f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3e2f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3e2f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3e2f-127">Request body</span></span>
<span data-ttu-id="e3e2f-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e3e2f-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="e3e2f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e3e2f-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="e3e2f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3e2f-130">Property</span></span>|<span data-ttu-id="e3e2f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3e2f-131">Type</span></span>|<span data-ttu-id="e3e2f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3e2f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3e2f-133">id</span><span class="sxs-lookup"><span data-stu-id="e3e2f-133">id</span></span>|<span data-ttu-id="e3e2f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3e2f-134">String</span></span>|<span data-ttu-id="e3e2f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e3e2f-135">Key of the entity.</span></span>|
|<span data-ttu-id="e3e2f-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3e2f-136">unknownDeviceCount</span></span>|<span data-ttu-id="e3e2f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e2f-137">Int32</span></span>|<span data-ttu-id="e3e2f-138">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="e3e2f-138">Number of unknown devices</span></span>|
|<span data-ttu-id="e3e2f-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3e2f-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="e3e2f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e2f-140">Int32</span></span>|<span data-ttu-id="e3e2f-141">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="e3e2f-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="e3e2f-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3e2f-142">compliantDeviceCount</span></span>|<span data-ttu-id="e3e2f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e2f-143">Int32</span></span>|<span data-ttu-id="e3e2f-144">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="e3e2f-144">Number of compliant devices</span></span>|
|<span data-ttu-id="e3e2f-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3e2f-145">remediatedDeviceCount</span></span>|<span data-ttu-id="e3e2f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e2f-146">Int32</span></span>|<span data-ttu-id="e3e2f-147">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="e3e2f-147">Number of remediated devices</span></span>|
|<span data-ttu-id="e3e2f-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3e2f-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="e3e2f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e2f-149">Int32</span></span>|<span data-ttu-id="e3e2f-150">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="e3e2f-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="e3e2f-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3e2f-151">errorDeviceCount</span></span>|<span data-ttu-id="e3e2f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e2f-152">Int32</span></span>|<span data-ttu-id="e3e2f-153">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="e3e2f-153">Number of error devices</span></span>|
|<span data-ttu-id="e3e2f-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3e2f-154">conflictDeviceCount</span></span>|<span data-ttu-id="e3e2f-155">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e2f-155">Int32</span></span>|<span data-ttu-id="e3e2f-156">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="e3e2f-156">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="e3e2f-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3e2f-157">Response</span></span>
<span data-ttu-id="e3e2f-158">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3e2f-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3e2f-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3e2f-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3e2f-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3e2f-160">Request</span></span>
<span data-ttu-id="e3e2f-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3e2f-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 214

{
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="e3e2f-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3e2f-162">Response</span></span>
<span data-ttu-id="e3e2f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3e2f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```





