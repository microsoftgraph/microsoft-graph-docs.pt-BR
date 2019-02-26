---
title: Atualizar windowsManagementAppHealthSummary
description: Atualiza as propriedades de um objeto windowsManagementAppHealthSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 764549ee57bc3ab3a2a1e0c2db9c6ac16309b85d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155962"
---
# <a name="update-windowsmanagementapphealthsummary"></a><span data-ttu-id="2d0f3-103">Atualizar windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="2d0f3-103">Update windowsManagementAppHealthSummary</span></span>

> <span data-ttu-id="2d0f3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2d0f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d0f3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2d0f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d0f3-106">Atualiza as propriedades de um objeto [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="2d0f3-106">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d0f3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2d0f3-107">Prerequisites</span></span>
<span data-ttu-id="2d0f3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2d0f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2d0f3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d0f3-110">Permission type</span></span>|<span data-ttu-id="2d0f3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2d0f3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d0f3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d0f3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d0f3-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d0f3-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2d0f3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d0f3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d0f3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d0f3-115">Not supported.</span></span>|
|<span data-ttu-id="2d0f3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d0f3-116">Application</span></span>|<span data-ttu-id="2d0f3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d0f3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d0f3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d0f3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthSummary
```

## <a name="request-headers"></a><span data-ttu-id="2d0f3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d0f3-119">Request headers</span></span>
|<span data-ttu-id="2d0f3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2d0f3-120">Header</span></span>|<span data-ttu-id="2d0f3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2d0f3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d0f3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d0f3-122">Authorization</span></span>|<span data-ttu-id="2d0f3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d0f3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d0f3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2d0f3-124">Accept</span></span>|<span data-ttu-id="2d0f3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d0f3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d0f3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d0f3-126">Request body</span></span>
<span data-ttu-id="2d0f3-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="2d0f3-127">In the request body, supply a JSON representation for the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

<span data-ttu-id="2d0f3-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2d0f3-128">The following table shows the properties that are required when you create the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span></span>

|<span data-ttu-id="2d0f3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d0f3-129">Property</span></span>|<span data-ttu-id="2d0f3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d0f3-130">Type</span></span>|<span data-ttu-id="2d0f3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d0f3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d0f3-132">id</span><span class="sxs-lookup"><span data-stu-id="2d0f3-132">id</span></span>|<span data-ttu-id="2d0f3-133">String</span><span class="sxs-lookup"><span data-stu-id="2d0f3-133">String</span></span>|<span data-ttu-id="2d0f3-134">Chave da entidade de Resumo de integridade do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="2d0f3-134">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="2d0f3-135">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d0f3-135">healthyDeviceCount</span></span>|<span data-ttu-id="2d0f3-136">Int32</span><span class="sxs-lookup"><span data-stu-id="2d0f3-136">Int32</span></span>|<span data-ttu-id="2d0f3-137">Contagem de dispositivos íntegros.</span><span class="sxs-lookup"><span data-stu-id="2d0f3-137">Healthy device count.</span></span>|
|<span data-ttu-id="2d0f3-138">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d0f3-138">unhealthyDeviceCount</span></span>|<span data-ttu-id="2d0f3-139">Int32</span><span class="sxs-lookup"><span data-stu-id="2d0f3-139">Int32</span></span>|<span data-ttu-id="2d0f3-140">Contagem de dispositivos não íntegros.</span><span class="sxs-lookup"><span data-stu-id="2d0f3-140">Unhealthy device count.</span></span>|
|<span data-ttu-id="2d0f3-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d0f3-141">unknownDeviceCount</span></span>|<span data-ttu-id="2d0f3-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2d0f3-142">Int32</span></span>|<span data-ttu-id="2d0f3-143">Contagem desconhecida de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="2d0f3-143">Unknown device count.</span></span>|



## <a name="response"></a><span data-ttu-id="2d0f3-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d0f3-144">Response</span></span>
<span data-ttu-id="2d0f3-145">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d0f3-145">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d0f3-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d0f3-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d0f3-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d0f3-147">Request</span></span>
<span data-ttu-id="2d0f3-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d0f3-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthSummary
Content-type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "healthyDeviceCount": 2,
  "unhealthyDeviceCount": 4,
  "unknownDeviceCount": 2
}
```

### <a name="response"></a><span data-ttu-id="2d0f3-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d0f3-149">Response</span></span>
<span data-ttu-id="2d0f3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d0f3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 210

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "id": "a9d38a9e-8a9e-a9d3-9e8a-d3a99e8ad3a9",
  "healthyDeviceCount": 2,
  "unhealthyDeviceCount": 4,
  "unknownDeviceCount": 2
}
```




