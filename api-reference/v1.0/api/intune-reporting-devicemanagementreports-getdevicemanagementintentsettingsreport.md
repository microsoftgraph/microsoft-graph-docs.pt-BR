---
title: ação getDeviceManagementIntentSettingsReport
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6d94e6f07a612db27e1d1a9b712e78f0f0203f84
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758506"
---
# <a name="getdevicemanagementintentsettingsreport-action"></a><span data-ttu-id="ddea3-103">ação getDeviceManagementIntentSettingsReport</span><span class="sxs-lookup"><span data-stu-id="ddea3-103">getDeviceManagementIntentSettingsReport action</span></span>

<span data-ttu-id="ddea3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddea3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ddea3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ddea3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddea3-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ddea3-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddea3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ddea3-107">Prerequisites</span></span>
<span data-ttu-id="ddea3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddea3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddea3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddea3-110">Permission type</span></span>|<span data-ttu-id="ddea3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ddea3-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddea3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddea3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ddea3-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddea3-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ddea3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddea3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddea3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddea3-115">Not supported.</span></span>|
|<span data-ttu-id="ddea3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddea3-116">Application</span></span>|<span data-ttu-id="ddea3-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddea3-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddea3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddea3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getDeviceManagementIntentSettingsReport
```

## <a name="request-headers"></a><span data-ttu-id="ddea3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddea3-119">Request headers</span></span>
|<span data-ttu-id="ddea3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ddea3-120">Header</span></span>|<span data-ttu-id="ddea3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ddea3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddea3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddea3-122">Authorization</span></span>|<span data-ttu-id="ddea3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddea3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddea3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ddea3-124">Accept</span></span>|<span data-ttu-id="ddea3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ddea3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddea3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddea3-126">Request body</span></span>
<span data-ttu-id="ddea3-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ddea3-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ddea3-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ddea3-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ddea3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ddea3-129">Property</span></span>|<span data-ttu-id="ddea3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddea3-130">Type</span></span>|<span data-ttu-id="ddea3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddea3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddea3-132">nome</span><span class="sxs-lookup"><span data-stu-id="ddea3-132">name</span></span>|<span data-ttu-id="ddea3-133">String</span><span class="sxs-lookup"><span data-stu-id="ddea3-133">String</span></span>|<span data-ttu-id="ddea3-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ddea3-134">Not yet documented</span></span>|
|<span data-ttu-id="ddea3-135">select</span><span class="sxs-lookup"><span data-stu-id="ddea3-135">select</span></span>|<span data-ttu-id="ddea3-136">String collection</span><span class="sxs-lookup"><span data-stu-id="ddea3-136">String collection</span></span>|<span data-ttu-id="ddea3-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ddea3-137">Not yet documented</span></span>|
|<span data-ttu-id="ddea3-138">search</span><span class="sxs-lookup"><span data-stu-id="ddea3-138">search</span></span>|<span data-ttu-id="ddea3-139">String</span><span class="sxs-lookup"><span data-stu-id="ddea3-139">String</span></span>|<span data-ttu-id="ddea3-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ddea3-140">Not yet documented</span></span>|
|<span data-ttu-id="ddea3-141">groupBy</span><span class="sxs-lookup"><span data-stu-id="ddea3-141">groupBy</span></span>|<span data-ttu-id="ddea3-142">String collection</span><span class="sxs-lookup"><span data-stu-id="ddea3-142">String collection</span></span>|<span data-ttu-id="ddea3-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ddea3-143">Not yet documented</span></span>|
|<span data-ttu-id="ddea3-144">orderBy</span><span class="sxs-lookup"><span data-stu-id="ddea3-144">orderBy</span></span>|<span data-ttu-id="ddea3-145">String collection</span><span class="sxs-lookup"><span data-stu-id="ddea3-145">String collection</span></span>|<span data-ttu-id="ddea3-146">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ddea3-146">Not yet documented</span></span>|
|<span data-ttu-id="ddea3-147">skip</span><span class="sxs-lookup"><span data-stu-id="ddea3-147">skip</span></span>|<span data-ttu-id="ddea3-148">Int32</span><span class="sxs-lookup"><span data-stu-id="ddea3-148">Int32</span></span>|<span data-ttu-id="ddea3-149">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ddea3-149">Not yet documented</span></span>|
|<span data-ttu-id="ddea3-150">top</span><span class="sxs-lookup"><span data-stu-id="ddea3-150">top</span></span>|<span data-ttu-id="ddea3-151">Int32</span><span class="sxs-lookup"><span data-stu-id="ddea3-151">Int32</span></span>|<span data-ttu-id="ddea3-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ddea3-152">Not yet documented</span></span>|
|<span data-ttu-id="ddea3-153">sessionId</span><span class="sxs-lookup"><span data-stu-id="ddea3-153">sessionId</span></span>|<span data-ttu-id="ddea3-154">String</span><span class="sxs-lookup"><span data-stu-id="ddea3-154">String</span></span>|<span data-ttu-id="ddea3-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ddea3-155">Not yet documented</span></span>|
|<span data-ttu-id="ddea3-156">filter</span><span class="sxs-lookup"><span data-stu-id="ddea3-156">filter</span></span>|<span data-ttu-id="ddea3-157">String</span><span class="sxs-lookup"><span data-stu-id="ddea3-157">String</span></span>|<span data-ttu-id="ddea3-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ddea3-158">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ddea3-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddea3-159">Response</span></span>
<span data-ttu-id="ddea3-160">Se tiver êxito, essa ação retornará `200 OK` um código de resposta e um Stream no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddea3-160">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddea3-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ddea3-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddea3-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddea3-162">Request</span></span>
<span data-ttu-id="ddea3-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddea3-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/reports/getDeviceManagementIntentSettingsReport

Content-type: application/json
Content-length: 278

{
  "name": "Name value",
  "select": [
    "Select value"
  ],
  "search": "Search value",
  "groupBy": [
    "Group By value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "skip": 4,
  "top": 3,
  "sessionId": "Session Id value",
  "filter": "Filter value"
}
```

### <a name="response"></a><span data-ttu-id="ddea3-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddea3-164">Response</span></span>
<span data-ttu-id="ddea3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddea3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 111

{
  "value": "Z2V0RGV2aWNlTWFuYWdlbWVudEludGVudFNldHRpbmdzUmVwb3J0IEludHVuZSBEb2MgU2FtcGxlIDc2OTIyMjczOA=="
}
```




