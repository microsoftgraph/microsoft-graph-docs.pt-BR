---
title: Atualizar deviceComplianceUserOverview
description: Atualizar as propriedades de um objeto deviceComplianceUserOverview.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 05ccf80b957bf52155dfef738c886cf41155fc22
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891102"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="aa4d5-103">Atualizar deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="aa4d5-103">Update deviceComplianceUserOverview</span></span>

> <span data-ttu-id="aa4d5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa4d5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aa4d5-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aa4d5-107">Atualizar as propriedades de um objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="aa4d5-107">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aa4d5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aa4d5-108">Prerequisites</span></span>
<span data-ttu-id="aa4d5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa4d5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa4d5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa4d5-111">Permission type</span></span>|<span data-ttu-id="aa4d5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aa4d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa4d5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa4d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aa4d5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa4d5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aa4d5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa4d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa4d5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-116">Not supported.</span></span>|
|<span data-ttu-id="aa4d5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa4d5-117">Application</span></span>|<span data-ttu-id="aa4d5-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa4d5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa4d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="aa4d5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa4d5-120">Request headers</span></span>
|<span data-ttu-id="aa4d5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aa4d5-121">Header</span></span>|<span data-ttu-id="aa4d5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="aa4d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa4d5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa4d5-123">Authorization</span></span>|<span data-ttu-id="aa4d5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa4d5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aa4d5-125">Accept</span></span>|<span data-ttu-id="aa4d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aa4d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa4d5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa4d5-127">Request body</span></span>
<span data-ttu-id="aa4d5-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="aa4d5-128">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="aa4d5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="aa4d5-129">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="aa4d5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa4d5-130">Property</span></span>|<span data-ttu-id="aa4d5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa4d5-131">Type</span></span>|<span data-ttu-id="aa4d5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa4d5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa4d5-133">id</span><span class="sxs-lookup"><span data-stu-id="aa4d5-133">id</span></span>|<span data-ttu-id="aa4d5-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa4d5-134">String</span></span>|<span data-ttu-id="aa4d5-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-135">Key of the entity.</span></span>|
|<span data-ttu-id="aa4d5-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="aa4d5-136">pendingCount</span></span>|<span data-ttu-id="aa4d5-137">Int32</span><span class="sxs-lookup"><span data-stu-id="aa4d5-137">Int32</span></span>|<span data-ttu-id="aa4d5-138">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="aa4d5-138">Number of pending Users</span></span>|
|<span data-ttu-id="aa4d5-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="aa4d5-139">notApplicableCount</span></span>|<span data-ttu-id="aa4d5-140">Int32</span><span class="sxs-lookup"><span data-stu-id="aa4d5-140">Int32</span></span>|<span data-ttu-id="aa4d5-141">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="aa4d5-141">Number of not applicable users</span></span>|
|<span data-ttu-id="aa4d5-142">successCount</span><span class="sxs-lookup"><span data-stu-id="aa4d5-142">successCount</span></span>|<span data-ttu-id="aa4d5-143">Int32</span><span class="sxs-lookup"><span data-stu-id="aa4d5-143">Int32</span></span>|<span data-ttu-id="aa4d5-144">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="aa4d5-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="aa4d5-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="aa4d5-145">errorCount</span></span>|<span data-ttu-id="aa4d5-146">Int32</span><span class="sxs-lookup"><span data-stu-id="aa4d5-146">Int32</span></span>|<span data-ttu-id="aa4d5-147">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="aa4d5-147">Number of error Users</span></span>|
|<span data-ttu-id="aa4d5-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="aa4d5-148">failedCount</span></span>|<span data-ttu-id="aa4d5-149">Int32</span><span class="sxs-lookup"><span data-stu-id="aa4d5-149">Int32</span></span>|<span data-ttu-id="aa4d5-150">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="aa4d5-150">Number of failed Users</span></span>|
|<span data-ttu-id="aa4d5-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="aa4d5-151">conflictCount</span></span>|<span data-ttu-id="aa4d5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="aa4d5-152">Int32</span></span>|<span data-ttu-id="aa4d5-153">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="aa4d5-153">Number of users in conflict</span></span>|
|<span data-ttu-id="aa4d5-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="aa4d5-154">lastUpdateDateTime</span></span>|<span data-ttu-id="aa4d5-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa4d5-155">DateTimeOffset</span></span>|<span data-ttu-id="aa4d5-156">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="aa4d5-156">Last update time</span></span>|
|<span data-ttu-id="aa4d5-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="aa4d5-157">configurationVersion</span></span>|<span data-ttu-id="aa4d5-158">Int32</span><span class="sxs-lookup"><span data-stu-id="aa4d5-158">Int32</span></span>|<span data-ttu-id="aa4d5-159">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="aa4d5-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="aa4d5-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa4d5-160">Response</span></span>
<span data-ttu-id="aa4d5-161">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-161">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa4d5-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa4d5-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="aa4d5-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa4d5-163">Request</span></span>
<span data-ttu-id="aa4d5-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
Content-type: application/json
Content-length: 236

{
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="aa4d5-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa4d5-165">Response</span></span>
<span data-ttu-id="aa4d5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa4d5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 352

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "2d4f5bf4-5bf4-2d4f-f45b-4f2df45b4f2d",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```





