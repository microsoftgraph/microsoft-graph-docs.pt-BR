---
title: Atualizar managedDeviceMobileAppConfigurationUserSummary
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationUserSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ddeb89575dda5b2250f29e75d97b238d362f30c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754193"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="06d2d-103">Atualizar managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="06d2d-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

<span data-ttu-id="06d2d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06d2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06d2d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06d2d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06d2d-106">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="06d2d-106">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06d2d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06d2d-107">Prerequisites</span></span>
<span data-ttu-id="06d2d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06d2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06d2d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06d2d-110">Permission type</span></span>|<span data-ttu-id="06d2d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06d2d-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06d2d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06d2d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="06d2d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06d2d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="06d2d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06d2d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06d2d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06d2d-115">Not supported.</span></span>|
|<span data-ttu-id="06d2d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06d2d-116">Application</span></span>|<span data-ttu-id="06d2d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06d2d-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06d2d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06d2d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="06d2d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06d2d-119">Request headers</span></span>
|<span data-ttu-id="06d2d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06d2d-120">Header</span></span>|<span data-ttu-id="06d2d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="06d2d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06d2d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="06d2d-122">Authorization</span></span>|<span data-ttu-id="06d2d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06d2d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06d2d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06d2d-124">Accept</span></span>|<span data-ttu-id="06d2d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="06d2d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06d2d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06d2d-126">Request body</span></span>
<span data-ttu-id="06d2d-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="06d2d-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="06d2d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="06d2d-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="06d2d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06d2d-129">Property</span></span>|<span data-ttu-id="06d2d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="06d2d-130">Type</span></span>|<span data-ttu-id="06d2d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="06d2d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06d2d-132">id</span><span class="sxs-lookup"><span data-stu-id="06d2d-132">id</span></span>|<span data-ttu-id="06d2d-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06d2d-133">String</span></span>|<span data-ttu-id="06d2d-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="06d2d-134">Key of the entity.</span></span>|
|<span data-ttu-id="06d2d-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="06d2d-135">pendingCount</span></span>|<span data-ttu-id="06d2d-136">Int32</span><span class="sxs-lookup"><span data-stu-id="06d2d-136">Int32</span></span>|<span data-ttu-id="06d2d-137">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="06d2d-137">Number of pending Users</span></span>|
|<span data-ttu-id="06d2d-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="06d2d-138">notApplicableCount</span></span>|<span data-ttu-id="06d2d-139">Int32</span><span class="sxs-lookup"><span data-stu-id="06d2d-139">Int32</span></span>|<span data-ttu-id="06d2d-140">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="06d2d-140">Number of not applicable users</span></span>|
|<span data-ttu-id="06d2d-141">successCount</span><span class="sxs-lookup"><span data-stu-id="06d2d-141">successCount</span></span>|<span data-ttu-id="06d2d-142">Int32</span><span class="sxs-lookup"><span data-stu-id="06d2d-142">Int32</span></span>|<span data-ttu-id="06d2d-143">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="06d2d-143">Number of succeeded Users</span></span>|
|<span data-ttu-id="06d2d-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="06d2d-144">errorCount</span></span>|<span data-ttu-id="06d2d-145">Int32</span><span class="sxs-lookup"><span data-stu-id="06d2d-145">Int32</span></span>|<span data-ttu-id="06d2d-146">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="06d2d-146">Number of error Users</span></span>|
|<span data-ttu-id="06d2d-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="06d2d-147">failedCount</span></span>|<span data-ttu-id="06d2d-148">Int32</span><span class="sxs-lookup"><span data-stu-id="06d2d-148">Int32</span></span>|<span data-ttu-id="06d2d-149">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="06d2d-149">Number of failed Users</span></span>|
|<span data-ttu-id="06d2d-150">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="06d2d-150">lastUpdateDateTime</span></span>|<span data-ttu-id="06d2d-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06d2d-151">DateTimeOffset</span></span>|<span data-ttu-id="06d2d-152">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="06d2d-152">Last update time</span></span>|
|<span data-ttu-id="06d2d-153">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="06d2d-153">configurationVersion</span></span>|<span data-ttu-id="06d2d-154">Int32</span><span class="sxs-lookup"><span data-stu-id="06d2d-154">Int32</span></span>|<span data-ttu-id="06d2d-155">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="06d2d-155">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="06d2d-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="06d2d-156">Response</span></span>
<span data-ttu-id="06d2d-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06d2d-157">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06d2d-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06d2d-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="06d2d-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06d2d-159">Request</span></span>
<span data-ttu-id="06d2d-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06d2d-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
Content-type: application/json
Content-length: 297

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="06d2d-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="06d2d-161">Response</span></span>
<span data-ttu-id="06d2d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06d2d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "7b953742-3742-7b95-4237-957b4237957b",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```




