---
title: Atualizar deviceConfigurationUserStatus
description: Atualizar as propriedades de um objeto deviceConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fb2be54a7abe5f398148ddef5ddea01d3a97fbca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875716"
---
# <a name="update-deviceconfigurationuserstatus"></a><span data-ttu-id="85c50-103">Atualizar deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="85c50-103">Update deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="85c50-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="85c50-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85c50-105">Atualizar as propriedades de um objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="85c50-105">Update the properties of a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="85c50-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="85c50-106">Prerequisites</span></span>
<span data-ttu-id="85c50-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85c50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85c50-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85c50-109">Permission type</span></span>|<span data-ttu-id="85c50-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="85c50-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85c50-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85c50-111">Delegated (work or school account)</span></span>|<span data-ttu-id="85c50-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85c50-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="85c50-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85c50-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85c50-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85c50-114">Not supported.</span></span>|
|<span data-ttu-id="85c50-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85c50-115">Application</span></span>|<span data-ttu-id="85c50-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85c50-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85c50-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85c50-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="85c50-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85c50-118">Request headers</span></span>
|<span data-ttu-id="85c50-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="85c50-119">Header</span></span>|<span data-ttu-id="85c50-120">Valor</span><span class="sxs-lookup"><span data-stu-id="85c50-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85c50-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="85c50-121">Authorization</span></span>|<span data-ttu-id="85c50-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85c50-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85c50-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="85c50-123">Accept</span></span>|<span data-ttu-id="85c50-124">application/json</span><span class="sxs-lookup"><span data-stu-id="85c50-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85c50-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85c50-125">Request body</span></span>
<span data-ttu-id="85c50-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="85c50-126">In the request body, supply a JSON representation for the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="85c50-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="85c50-127">The following table shows the properties that are required when you create the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="85c50-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85c50-128">Property</span></span>|<span data-ttu-id="85c50-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="85c50-129">Type</span></span>|<span data-ttu-id="85c50-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="85c50-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85c50-131">id</span><span class="sxs-lookup"><span data-stu-id="85c50-131">id</span></span>|<span data-ttu-id="85c50-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85c50-132">String</span></span>|<span data-ttu-id="85c50-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="85c50-133">Key of the entity.</span></span>|
|<span data-ttu-id="85c50-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="85c50-134">userDisplayName</span></span>|<span data-ttu-id="85c50-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85c50-135">String</span></span>|<span data-ttu-id="85c50-136">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="85c50-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="85c50-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="85c50-137">devicesCount</span></span>|<span data-ttu-id="85c50-138">Int32</span><span class="sxs-lookup"><span data-stu-id="85c50-138">Int32</span></span>|<span data-ttu-id="85c50-139">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="85c50-139">Devices count for that user.</span></span>|
|<span data-ttu-id="85c50-140">status</span><span class="sxs-lookup"><span data-stu-id="85c50-140">status</span></span>|[<span data-ttu-id="85c50-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="85c50-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="85c50-142">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="85c50-142">Compliance status of the policy report.</span></span> <span data-ttu-id="85c50-143">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="85c50-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="85c50-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="85c50-144">lastReportedDateTime</span></span>|<span data-ttu-id="85c50-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85c50-145">DateTimeOffset</span></span>|<span data-ttu-id="85c50-146">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="85c50-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="85c50-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="85c50-147">userPrincipalName</span></span>|<span data-ttu-id="85c50-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85c50-148">String</span></span>|<span data-ttu-id="85c50-149">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="85c50-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="85c50-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="85c50-150">Response</span></span>
<span data-ttu-id="85c50-151">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85c50-151">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85c50-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85c50-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="85c50-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85c50-153">Request</span></span>
<span data-ttu-id="85c50-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85c50-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="85c50-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="85c50-155">Response</span></span>
<span data-ttu-id="85c50-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85c50-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



