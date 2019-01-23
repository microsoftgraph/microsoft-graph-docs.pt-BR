---
title: Atualizar deviceConfigurationDeviceStateSummary
description: Atualizar as propriedades de um objeto deviceConfigurationDeviceStateSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 41b092aa651d8526618f8287c7a90ff9673c7508
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408548"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="01c9b-103">Atualizar deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="01c9b-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="01c9b-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="01c9b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="01c9b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="01c9b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01c9b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="01c9b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01c9b-107">Atualizar as propriedades de um objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="01c9b-107">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01c9b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="01c9b-108">Prerequisites</span></span>
<span data-ttu-id="01c9b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="01c9b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="01c9b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01c9b-111">Permission type</span></span>|<span data-ttu-id="01c9b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="01c9b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01c9b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01c9b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01c9b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01c9b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01c9b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01c9b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01c9b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01c9b-116">Not supported.</span></span>|
|<span data-ttu-id="01c9b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01c9b-117">Application</span></span>|<span data-ttu-id="01c9b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01c9b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01c9b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01c9b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="01c9b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01c9b-120">Request headers</span></span>
|<span data-ttu-id="01c9b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01c9b-121">Header</span></span>|<span data-ttu-id="01c9b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="01c9b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01c9b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="01c9b-123">Authorization</span></span>|<span data-ttu-id="01c9b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01c9b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01c9b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="01c9b-125">Accept</span></span>|<span data-ttu-id="01c9b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01c9b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01c9b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01c9b-127">Request body</span></span>
<span data-ttu-id="01c9b-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="01c9b-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="01c9b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="01c9b-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="01c9b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01c9b-130">Property</span></span>|<span data-ttu-id="01c9b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="01c9b-131">Type</span></span>|<span data-ttu-id="01c9b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="01c9b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01c9b-133">id</span><span class="sxs-lookup"><span data-stu-id="01c9b-133">id</span></span>|<span data-ttu-id="01c9b-134">String</span><span class="sxs-lookup"><span data-stu-id="01c9b-134">String</span></span>|<span data-ttu-id="01c9b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="01c9b-135">Key of the entity.</span></span>|
|<span data-ttu-id="01c9b-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="01c9b-136">unknownDeviceCount</span></span>|<span data-ttu-id="01c9b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="01c9b-137">Int32</span></span>|<span data-ttu-id="01c9b-138">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="01c9b-138">Number of unknown devices</span></span>|
|<span data-ttu-id="01c9b-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="01c9b-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="01c9b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="01c9b-140">Int32</span></span>|<span data-ttu-id="01c9b-141">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="01c9b-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="01c9b-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="01c9b-142">compliantDeviceCount</span></span>|<span data-ttu-id="01c9b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="01c9b-143">Int32</span></span>|<span data-ttu-id="01c9b-144">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="01c9b-144">Number of compliant devices</span></span>|
|<span data-ttu-id="01c9b-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="01c9b-145">remediatedDeviceCount</span></span>|<span data-ttu-id="01c9b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="01c9b-146">Int32</span></span>|<span data-ttu-id="01c9b-147">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="01c9b-147">Number of remediated devices</span></span>|
|<span data-ttu-id="01c9b-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="01c9b-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="01c9b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="01c9b-149">Int32</span></span>|<span data-ttu-id="01c9b-150">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="01c9b-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="01c9b-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="01c9b-151">errorDeviceCount</span></span>|<span data-ttu-id="01c9b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="01c9b-152">Int32</span></span>|<span data-ttu-id="01c9b-153">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="01c9b-153">Number of error devices</span></span>|
|<span data-ttu-id="01c9b-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="01c9b-154">conflictDeviceCount</span></span>|<span data-ttu-id="01c9b-155">Int32</span><span class="sxs-lookup"><span data-stu-id="01c9b-155">Int32</span></span>|<span data-ttu-id="01c9b-156">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="01c9b-156">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="01c9b-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="01c9b-157">Response</span></span>
<span data-ttu-id="01c9b-158">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01c9b-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01c9b-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01c9b-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="01c9b-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01c9b-160">Request</span></span>
<span data-ttu-id="01c9b-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01c9b-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="01c9b-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="01c9b-162">Response</span></span>
<span data-ttu-id="01c9b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01c9b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




