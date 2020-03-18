---
title: ação getSettingNonComplianceReport
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4bce2a5b73205eb42ee499673b65e588f1de0b6c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801359"
---
# <a name="getsettingnoncompliancereport-action"></a><span data-ttu-id="45750-103">ação getSettingNonComplianceReport</span><span class="sxs-lookup"><span data-stu-id="45750-103">getSettingNonComplianceReport action</span></span>

> <span data-ttu-id="45750-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45750-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45750-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45750-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45750-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="45750-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45750-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45750-107">Prerequisites</span></span>
<span data-ttu-id="45750-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45750-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45750-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45750-110">Permission type</span></span>|<span data-ttu-id="45750-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="45750-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45750-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45750-112">Delegated (work or school account)</span></span>|<span data-ttu-id="45750-113">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="45750-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="45750-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45750-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45750-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45750-115">Not supported.</span></span>|
|<span data-ttu-id="45750-116">Application</span><span class="sxs-lookup"><span data-stu-id="45750-116">Application</span></span>|<span data-ttu-id="45750-117">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="45750-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45750-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45750-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getSettingNonComplianceReport
```

## <a name="request-headers"></a><span data-ttu-id="45750-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45750-119">Request headers</span></span>
|<span data-ttu-id="45750-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45750-120">Header</span></span>|<span data-ttu-id="45750-121">Valor</span><span class="sxs-lookup"><span data-stu-id="45750-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45750-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="45750-122">Authorization</span></span>|<span data-ttu-id="45750-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45750-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45750-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="45750-124">Accept</span></span>|<span data-ttu-id="45750-125">application/json</span><span class="sxs-lookup"><span data-stu-id="45750-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45750-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45750-126">Request body</span></span>
<span data-ttu-id="45750-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="45750-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="45750-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="45750-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="45750-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45750-129">Property</span></span>|<span data-ttu-id="45750-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="45750-130">Type</span></span>|<span data-ttu-id="45750-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="45750-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45750-132">nome</span><span class="sxs-lookup"><span data-stu-id="45750-132">name</span></span>|<span data-ttu-id="45750-133">String</span><span class="sxs-lookup"><span data-stu-id="45750-133">String</span></span>|<span data-ttu-id="45750-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="45750-134">Not yet documented</span></span>|
|<span data-ttu-id="45750-135">select</span><span class="sxs-lookup"><span data-stu-id="45750-135">select</span></span>|<span data-ttu-id="45750-136">String collection</span><span class="sxs-lookup"><span data-stu-id="45750-136">String collection</span></span>|<span data-ttu-id="45750-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="45750-137">Not yet documented</span></span>|
|<span data-ttu-id="45750-138">search</span><span class="sxs-lookup"><span data-stu-id="45750-138">search</span></span>|<span data-ttu-id="45750-139">String</span><span class="sxs-lookup"><span data-stu-id="45750-139">String</span></span>|<span data-ttu-id="45750-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="45750-140">Not yet documented</span></span>|
|<span data-ttu-id="45750-141">groupBy</span><span class="sxs-lookup"><span data-stu-id="45750-141">groupBy</span></span>|<span data-ttu-id="45750-142">String collection</span><span class="sxs-lookup"><span data-stu-id="45750-142">String collection</span></span>|<span data-ttu-id="45750-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="45750-143">Not yet documented</span></span>|
|<span data-ttu-id="45750-144">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="45750-144">orderBy</span></span>|<span data-ttu-id="45750-145">String collection</span><span class="sxs-lookup"><span data-stu-id="45750-145">String collection</span></span>|<span data-ttu-id="45750-146">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="45750-146">Not yet documented</span></span>|
|<span data-ttu-id="45750-147">skip</span><span class="sxs-lookup"><span data-stu-id="45750-147">skip</span></span>|<span data-ttu-id="45750-148">Int32</span><span class="sxs-lookup"><span data-stu-id="45750-148">Int32</span></span>|<span data-ttu-id="45750-149">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="45750-149">Not yet documented</span></span>|
|<span data-ttu-id="45750-150">top</span><span class="sxs-lookup"><span data-stu-id="45750-150">top</span></span>|<span data-ttu-id="45750-151">Int32</span><span class="sxs-lookup"><span data-stu-id="45750-151">Int32</span></span>|<span data-ttu-id="45750-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="45750-152">Not yet documented</span></span>|
|<span data-ttu-id="45750-153">Identificação_da_sessão</span><span class="sxs-lookup"><span data-stu-id="45750-153">sessionId</span></span>|<span data-ttu-id="45750-154">String</span><span class="sxs-lookup"><span data-stu-id="45750-154">String</span></span>|<span data-ttu-id="45750-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="45750-155">Not yet documented</span></span>|
|<span data-ttu-id="45750-156">filter</span><span class="sxs-lookup"><span data-stu-id="45750-156">filter</span></span>|<span data-ttu-id="45750-157">String</span><span class="sxs-lookup"><span data-stu-id="45750-157">String</span></span>|<span data-ttu-id="45750-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="45750-158">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="45750-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="45750-159">Response</span></span>
<span data-ttu-id="45750-160">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e um fluxo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45750-160">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45750-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45750-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="45750-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45750-162">Request</span></span>
<span data-ttu-id="45750-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45750-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getSettingNonComplianceReport

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

### <a name="response"></a><span data-ttu-id="45750-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="45750-164">Response</span></span>
<span data-ttu-id="45750-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45750-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 54

{
  "value": "<Unknown Primitive Type Edm.Stream>"
}
```




