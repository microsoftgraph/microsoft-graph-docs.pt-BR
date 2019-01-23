---
title: Atualizar windowsManagementAppHealthSummary
description: Atualize as propriedades de um objeto windowsManagementAppHealthSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d7e8c077b8f06b9647e34a18fd5aa92987272e77
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394163"
---
# <a name="update-windowsmanagementapphealthsummary"></a><span data-ttu-id="03683-103">Atualizar windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="03683-103">Update windowsManagementAppHealthSummary</span></span>

> <span data-ttu-id="03683-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="03683-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="03683-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="03683-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03683-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="03683-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03683-107">Atualize as propriedades de um objeto [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="03683-107">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03683-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="03683-108">Prerequisites</span></span>
<span data-ttu-id="03683-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="03683-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="03683-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03683-111">Permission type</span></span>|<span data-ttu-id="03683-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="03683-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03683-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03683-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03683-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03683-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="03683-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03683-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03683-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03683-116">Not supported.</span></span>|
|<span data-ttu-id="03683-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03683-117">Application</span></span>|<span data-ttu-id="03683-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03683-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03683-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03683-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthSummary
```

## <a name="request-headers"></a><span data-ttu-id="03683-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03683-120">Request headers</span></span>
|<span data-ttu-id="03683-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="03683-121">Header</span></span>|<span data-ttu-id="03683-122">Valor</span><span class="sxs-lookup"><span data-stu-id="03683-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03683-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="03683-123">Authorization</span></span>|<span data-ttu-id="03683-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03683-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03683-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="03683-125">Accept</span></span>|<span data-ttu-id="03683-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03683-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03683-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03683-127">Request body</span></span>
<span data-ttu-id="03683-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="03683-128">In the request body, supply a JSON representation for the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

<span data-ttu-id="03683-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span><span class="sxs-lookup"><span data-stu-id="03683-129">The following table shows the properties that are required when you create the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span></span>

|<span data-ttu-id="03683-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03683-130">Property</span></span>|<span data-ttu-id="03683-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="03683-131">Type</span></span>|<span data-ttu-id="03683-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="03683-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03683-133">id</span><span class="sxs-lookup"><span data-stu-id="03683-133">id</span></span>|<span data-ttu-id="03683-134">String</span><span class="sxs-lookup"><span data-stu-id="03683-134">String</span></span>|<span data-ttu-id="03683-135">Chave da entidade Windows management app integridade resumida.</span><span class="sxs-lookup"><span data-stu-id="03683-135">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="03683-136">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="03683-136">healthyDeviceCount</span></span>|<span data-ttu-id="03683-137">Int32</span><span class="sxs-lookup"><span data-stu-id="03683-137">Int32</span></span>|<span data-ttu-id="03683-138">Contagem de dispositivo íntegro.</span><span class="sxs-lookup"><span data-stu-id="03683-138">Healthy device count.</span></span>|
|<span data-ttu-id="03683-139">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="03683-139">unhealthyDeviceCount</span></span>|<span data-ttu-id="03683-140">Int32</span><span class="sxs-lookup"><span data-stu-id="03683-140">Int32</span></span>|<span data-ttu-id="03683-141">Contagem de dispositivo não íntegros.</span><span class="sxs-lookup"><span data-stu-id="03683-141">Unhealthy device count.</span></span>|
|<span data-ttu-id="03683-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="03683-142">unknownDeviceCount</span></span>|<span data-ttu-id="03683-143">Int32</span><span class="sxs-lookup"><span data-stu-id="03683-143">Int32</span></span>|<span data-ttu-id="03683-144">Contagem de dispositivo desconhecido.</span><span class="sxs-lookup"><span data-stu-id="03683-144">Unknown device count.</span></span>|



## <a name="response"></a><span data-ttu-id="03683-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="03683-145">Response</span></span>
<span data-ttu-id="03683-146">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03683-146">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03683-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03683-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="03683-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03683-148">Request</span></span>
<span data-ttu-id="03683-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03683-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="03683-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="03683-150">Response</span></span>
<span data-ttu-id="03683-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03683-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




