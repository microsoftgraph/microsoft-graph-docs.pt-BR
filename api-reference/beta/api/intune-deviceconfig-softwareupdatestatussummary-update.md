---
title: Atualizar softwareUpdateStatusSummary
description: Atualizar as propriedades de um objeto softwareUpdateStatusSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8a3ceff462e9e2ee32ec1a7a32b3b1f5dd129b41
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734970"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="fad0e-103">Atualizar softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="fad0e-103">Update softwareUpdateStatusSummary</span></span>

<span data-ttu-id="fad0e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fad0e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fad0e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fad0e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fad0e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fad0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fad0e-107">Atualizar as propriedades de um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="fad0e-107">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fad0e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fad0e-108">Prerequisites</span></span>
<span data-ttu-id="fad0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fad0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fad0e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fad0e-111">Permission type</span></span>|<span data-ttu-id="fad0e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fad0e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fad0e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fad0e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fad0e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fad0e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fad0e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fad0e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fad0e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fad0e-116">Not supported.</span></span>|
|<span data-ttu-id="fad0e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fad0e-117">Application</span></span>|<span data-ttu-id="fad0e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fad0e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fad0e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fad0e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="fad0e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fad0e-120">Request headers</span></span>
|<span data-ttu-id="fad0e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fad0e-121">Header</span></span>|<span data-ttu-id="fad0e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fad0e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fad0e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fad0e-123">Authorization</span></span>|<span data-ttu-id="fad0e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fad0e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fad0e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fad0e-125">Accept</span></span>|<span data-ttu-id="fad0e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fad0e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fad0e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fad0e-127">Request body</span></span>
<span data-ttu-id="fad0e-128">No corpo da solicitação, forneça uma representação JSON do objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="fad0e-128">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="fad0e-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="fad0e-129">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="fad0e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fad0e-130">Property</span></span>|<span data-ttu-id="fad0e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fad0e-131">Type</span></span>|<span data-ttu-id="fad0e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fad0e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fad0e-133">id</span><span class="sxs-lookup"><span data-stu-id="fad0e-133">id</span></span>|<span data-ttu-id="fad0e-134">String</span><span class="sxs-lookup"><span data-stu-id="fad0e-134">String</span></span>|<span data-ttu-id="fad0e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fad0e-135">Key of the entity.</span></span>|
|<span data-ttu-id="fad0e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="fad0e-136">displayName</span></span>|<span data-ttu-id="fad0e-137">String</span><span class="sxs-lookup"><span data-stu-id="fad0e-137">String</span></span>|<span data-ttu-id="fad0e-138">O nome da política.</span><span class="sxs-lookup"><span data-stu-id="fad0e-138">The name of the policy.</span></span>|
|<span data-ttu-id="fad0e-139">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fad0e-139">compliantDeviceCount</span></span>|<span data-ttu-id="fad0e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="fad0e-140">Int32</span></span>|<span data-ttu-id="fad0e-141">Número de dispositivos em conformidade.</span><span class="sxs-lookup"><span data-stu-id="fad0e-141">Number of compliant devices.</span></span>|
|<span data-ttu-id="fad0e-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fad0e-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="fad0e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="fad0e-143">Int32</span></span>|<span data-ttu-id="fad0e-144">Número de dispositivos sem conformidade.</span><span class="sxs-lookup"><span data-stu-id="fad0e-144">Number of non compliant devices.</span></span>|
|<span data-ttu-id="fad0e-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fad0e-145">remediatedDeviceCount</span></span>|<span data-ttu-id="fad0e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="fad0e-146">Int32</span></span>|<span data-ttu-id="fad0e-147">Número de dispositivos corrigidos.</span><span class="sxs-lookup"><span data-stu-id="fad0e-147">Number of remediated devices.</span></span>|
|<span data-ttu-id="fad0e-148">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fad0e-148">errorDeviceCount</span></span>|<span data-ttu-id="fad0e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="fad0e-149">Int32</span></span>|<span data-ttu-id="fad0e-150">Número de dispositivos com erro.</span><span class="sxs-lookup"><span data-stu-id="fad0e-150">Number of devices had error.</span></span>|
|<span data-ttu-id="fad0e-151">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fad0e-151">unknownDeviceCount</span></span>|<span data-ttu-id="fad0e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="fad0e-152">Int32</span></span>|<span data-ttu-id="fad0e-153">Número de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="fad0e-153">Number of unknown devices.</span></span>|
|<span data-ttu-id="fad0e-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fad0e-154">conflictDeviceCount</span></span>|<span data-ttu-id="fad0e-155">Int32</span><span class="sxs-lookup"><span data-stu-id="fad0e-155">Int32</span></span>|<span data-ttu-id="fad0e-156">Número de dispositivos em conflito.</span><span class="sxs-lookup"><span data-stu-id="fad0e-156">Number of conflict devices.</span></span>|
|<span data-ttu-id="fad0e-157">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fad0e-157">notApplicableDeviceCount</span></span>|<span data-ttu-id="fad0e-158">Int32</span><span class="sxs-lookup"><span data-stu-id="fad0e-158">Int32</span></span>|<span data-ttu-id="fad0e-159">Número de dispositivos não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="fad0e-159">Number of not applicable devices.</span></span>|
|<span data-ttu-id="fad0e-160">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="fad0e-160">compliantUserCount</span></span>|<span data-ttu-id="fad0e-161">Int32</span><span class="sxs-lookup"><span data-stu-id="fad0e-161">Int32</span></span>|<span data-ttu-id="fad0e-162">Número de usuários em conformidade.</span><span class="sxs-lookup"><span data-stu-id="fad0e-162">Number of compliant users.</span></span>|
|<span data-ttu-id="fad0e-163">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="fad0e-163">nonCompliantUserCount</span></span>|<span data-ttu-id="fad0e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="fad0e-164">Int32</span></span>|<span data-ttu-id="fad0e-165">Número de usuários em não conformidade.</span><span class="sxs-lookup"><span data-stu-id="fad0e-165">Number of non compliant users.</span></span>|
|<span data-ttu-id="fad0e-166">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="fad0e-166">remediatedUserCount</span></span>|<span data-ttu-id="fad0e-167">Int32</span><span class="sxs-lookup"><span data-stu-id="fad0e-167">Int32</span></span>|<span data-ttu-id="fad0e-168">Número de usuários corrigidos.</span><span class="sxs-lookup"><span data-stu-id="fad0e-168">Number of remediated users.</span></span>|
|<span data-ttu-id="fad0e-169">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="fad0e-169">errorUserCount</span></span>|<span data-ttu-id="fad0e-170">Int32</span><span class="sxs-lookup"><span data-stu-id="fad0e-170">Int32</span></span>|<span data-ttu-id="fad0e-171">Número de usuários com erro.</span><span class="sxs-lookup"><span data-stu-id="fad0e-171">Number of users had error.</span></span>|
|<span data-ttu-id="fad0e-172">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="fad0e-172">unknownUserCount</span></span>|<span data-ttu-id="fad0e-173">Int32</span><span class="sxs-lookup"><span data-stu-id="fad0e-173">Int32</span></span>|<span data-ttu-id="fad0e-174">Número de usuários desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="fad0e-174">Number of unknown users.</span></span>|
|<span data-ttu-id="fad0e-175">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="fad0e-175">conflictUserCount</span></span>|<span data-ttu-id="fad0e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="fad0e-176">Int32</span></span>|<span data-ttu-id="fad0e-177">Número de usuários com conflitos.</span><span class="sxs-lookup"><span data-stu-id="fad0e-177">Number of conflict users.</span></span>|
|<span data-ttu-id="fad0e-178">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="fad0e-178">notApplicableUserCount</span></span>|<span data-ttu-id="fad0e-179">Int32</span><span class="sxs-lookup"><span data-stu-id="fad0e-179">Int32</span></span>|<span data-ttu-id="fad0e-180">Número de usuários não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="fad0e-180">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="fad0e-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="fad0e-181">Response</span></span>
<span data-ttu-id="fad0e-182">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fad0e-182">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fad0e-183">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fad0e-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="fad0e-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fad0e-184">Request</span></span>
<span data-ttu-id="fad0e-185">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fad0e-185">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/softwareUpdateStatusSummary
Content-type: application/json
Content-length: 518

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```

### <a name="response"></a><span data-ttu-id="fad0e-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="fad0e-186">Response</span></span>
<span data-ttu-id="fad0e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fad0e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "4f71421f-421f-4f71-1f42-714f1f42714f",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```





