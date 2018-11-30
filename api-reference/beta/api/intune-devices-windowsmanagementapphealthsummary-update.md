---
title: Atualizar windowsManagementAppHealthSummary
description: Atualize as propriedades de um objeto windowsManagementAppHealthSummary.
ms.openlocfilehash: e0f02a49b6585398d95d096aeb0b592438dbe68a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036711"
---
# <a name="update-windowsmanagementapphealthsummary"></a><span data-ttu-id="5ea71-103">Atualizar windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="5ea71-103">Update windowsManagementAppHealthSummary</span></span>

> <span data-ttu-id="5ea71-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5ea71-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ea71-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5ea71-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5ea71-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5ea71-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5ea71-107">Atualize as propriedades de um objeto [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="5ea71-107">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5ea71-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ea71-108">Prerequisites</span></span>
<span data-ttu-id="5ea71-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ea71-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ea71-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ea71-111">Permission type</span></span>|<span data-ttu-id="5ea71-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ea71-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ea71-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ea71-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ea71-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ea71-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5ea71-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ea71-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ea71-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ea71-116">Not supported.</span></span>|
|<span data-ttu-id="5ea71-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ea71-117">Application</span></span>|<span data-ttu-id="5ea71-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ea71-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ea71-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ea71-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthSummary
```

## <a name="request-headers"></a><span data-ttu-id="5ea71-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ea71-120">Request headers</span></span>
|<span data-ttu-id="5ea71-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ea71-121">Header</span></span>|<span data-ttu-id="5ea71-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5ea71-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ea71-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ea71-123">Authorization</span></span>|<span data-ttu-id="5ea71-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ea71-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ea71-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5ea71-125">Accept</span></span>|<span data-ttu-id="5ea71-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ea71-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ea71-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ea71-127">Request body</span></span>
<span data-ttu-id="5ea71-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="5ea71-128">In the request body, supply a JSON representation for the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

<span data-ttu-id="5ea71-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span><span class="sxs-lookup"><span data-stu-id="5ea71-129">The following table shows the properties that are required when you create the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span></span>

|<span data-ttu-id="5ea71-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ea71-130">Property</span></span>|<span data-ttu-id="5ea71-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ea71-131">Type</span></span>|<span data-ttu-id="5ea71-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ea71-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ea71-133">id</span><span class="sxs-lookup"><span data-stu-id="5ea71-133">id</span></span>|<span data-ttu-id="5ea71-134">String</span><span class="sxs-lookup"><span data-stu-id="5ea71-134">String</span></span>|<span data-ttu-id="5ea71-135">Chave da entidade Windows management app integridade resumida.</span><span class="sxs-lookup"><span data-stu-id="5ea71-135">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="5ea71-136">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ea71-136">healthyDeviceCount</span></span>|<span data-ttu-id="5ea71-137">Int32</span><span class="sxs-lookup"><span data-stu-id="5ea71-137">Int32</span></span>|<span data-ttu-id="5ea71-138">Contagem de dispositivo íntegro.</span><span class="sxs-lookup"><span data-stu-id="5ea71-138">Healthy device count.</span></span>|
|<span data-ttu-id="5ea71-139">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ea71-139">unhealthyDeviceCount</span></span>|<span data-ttu-id="5ea71-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5ea71-140">Int32</span></span>|<span data-ttu-id="5ea71-141">Contagem de dispositivo não íntegros.</span><span class="sxs-lookup"><span data-stu-id="5ea71-141">Unhealthy device count.</span></span>|
|<span data-ttu-id="5ea71-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ea71-142">unknownDeviceCount</span></span>|<span data-ttu-id="5ea71-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5ea71-143">Int32</span></span>|<span data-ttu-id="5ea71-144">Contagem de dispositivo desconhecido.</span><span class="sxs-lookup"><span data-stu-id="5ea71-144">Unknown device count.</span></span>|



## <a name="response"></a><span data-ttu-id="5ea71-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ea71-145">Response</span></span>
<span data-ttu-id="5ea71-146">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ea71-146">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ea71-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ea71-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="5ea71-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ea71-148">Request</span></span>
<span data-ttu-id="5ea71-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ea71-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthSummary
Content-type: application/json
Content-length: 89

{
  "healthyDeviceCount": 2,
  "unhealthyDeviceCount": 4,
  "unknownDeviceCount": 2
}
```

### <a name="response"></a><span data-ttu-id="5ea71-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ea71-150">Response</span></span>
<span data-ttu-id="5ea71-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ea71-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





