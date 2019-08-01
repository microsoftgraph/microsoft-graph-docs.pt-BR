---
title: Atualizar softwareUpdateStatusSummary
description: Atualizar as propriedades de um objeto softwareUpdateStatusSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 619208625337a48d11354b41629738a86c873f44
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017025"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="c966d-103">Atualizar softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="c966d-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="c966d-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c966d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c966d-105">Atualizar as propriedades de um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="c966d-105">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c966d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c966d-106">Prerequisites</span></span>
<span data-ttu-id="c966d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c966d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c966d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c966d-109">Permission type</span></span>|<span data-ttu-id="c966d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c966d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c966d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c966d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c966d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c966d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c966d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c966d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c966d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c966d-114">Not supported.</span></span>|
|<span data-ttu-id="c966d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c966d-115">Application</span></span>|<span data-ttu-id="c966d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c966d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c966d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c966d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="c966d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c966d-118">Request headers</span></span>
|<span data-ttu-id="c966d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c966d-119">Header</span></span>|<span data-ttu-id="c966d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c966d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c966d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c966d-121">Authorization</span></span>|<span data-ttu-id="c966d-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c966d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c966d-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c966d-123">Accept</span></span>|<span data-ttu-id="c966d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c966d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c966d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c966d-125">Request body</span></span>
<span data-ttu-id="c966d-126">No corpo da solicitação, forneça uma representação JSON do objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="c966d-126">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="c966d-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="c966d-127">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="c966d-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c966d-128">Property</span></span>|<span data-ttu-id="c966d-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c966d-129">Type</span></span>|<span data-ttu-id="c966d-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c966d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c966d-131">id</span><span class="sxs-lookup"><span data-stu-id="c966d-131">id</span></span>|<span data-ttu-id="c966d-132">String</span><span class="sxs-lookup"><span data-stu-id="c966d-132">String</span></span>|<span data-ttu-id="c966d-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c966d-133">Key of the entity.</span></span>|
|<span data-ttu-id="c966d-134">displayName</span><span class="sxs-lookup"><span data-stu-id="c966d-134">displayName</span></span>|<span data-ttu-id="c966d-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c966d-135">String</span></span>|<span data-ttu-id="c966d-136">O nome da política.</span><span class="sxs-lookup"><span data-stu-id="c966d-136">The name of the policy.</span></span>|
|<span data-ttu-id="c966d-137">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c966d-137">compliantDeviceCount</span></span>|<span data-ttu-id="c966d-138">Int32</span><span class="sxs-lookup"><span data-stu-id="c966d-138">Int32</span></span>|<span data-ttu-id="c966d-139">Número de dispositivos em conformidade.</span><span class="sxs-lookup"><span data-stu-id="c966d-139">Number of compliant devices.</span></span>|
|<span data-ttu-id="c966d-140">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c966d-140">nonCompliantDeviceCount</span></span>|<span data-ttu-id="c966d-141">Int32</span><span class="sxs-lookup"><span data-stu-id="c966d-141">Int32</span></span>|<span data-ttu-id="c966d-142">Número de dispositivos sem conformidade.</span><span class="sxs-lookup"><span data-stu-id="c966d-142">Number of non compliant devices.</span></span>|
|<span data-ttu-id="c966d-143">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c966d-143">remediatedDeviceCount</span></span>|<span data-ttu-id="c966d-144">Int32</span><span class="sxs-lookup"><span data-stu-id="c966d-144">Int32</span></span>|<span data-ttu-id="c966d-145">Número de dispositivos corrigidos.</span><span class="sxs-lookup"><span data-stu-id="c966d-145">Number of remediated devices.</span></span>|
|<span data-ttu-id="c966d-146">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c966d-146">errorDeviceCount</span></span>|<span data-ttu-id="c966d-147">Int32</span><span class="sxs-lookup"><span data-stu-id="c966d-147">Int32</span></span>|<span data-ttu-id="c966d-148">Número de dispositivos com erro.</span><span class="sxs-lookup"><span data-stu-id="c966d-148">Number of devices had error.</span></span>|
|<span data-ttu-id="c966d-149">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c966d-149">unknownDeviceCount</span></span>|<span data-ttu-id="c966d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c966d-150">Int32</span></span>|<span data-ttu-id="c966d-151">Número de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="c966d-151">Number of unknown devices.</span></span>|
|<span data-ttu-id="c966d-152">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c966d-152">conflictDeviceCount</span></span>|<span data-ttu-id="c966d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c966d-153">Int32</span></span>|<span data-ttu-id="c966d-154">Número de dispositivos em conflito.</span><span class="sxs-lookup"><span data-stu-id="c966d-154">Number of conflict devices.</span></span>|
|<span data-ttu-id="c966d-155">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c966d-155">notApplicableDeviceCount</span></span>|<span data-ttu-id="c966d-156">Int32</span><span class="sxs-lookup"><span data-stu-id="c966d-156">Int32</span></span>|<span data-ttu-id="c966d-157">Número de dispositivos não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="c966d-157">Number of not applicable devices.</span></span>|
|<span data-ttu-id="c966d-158">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="c966d-158">compliantUserCount</span></span>|<span data-ttu-id="c966d-159">Int32</span><span class="sxs-lookup"><span data-stu-id="c966d-159">Int32</span></span>|<span data-ttu-id="c966d-160">Número de usuários em conformidade.</span><span class="sxs-lookup"><span data-stu-id="c966d-160">Number of compliant users.</span></span>|
|<span data-ttu-id="c966d-161">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="c966d-161">nonCompliantUserCount</span></span>|<span data-ttu-id="c966d-162">Int32</span><span class="sxs-lookup"><span data-stu-id="c966d-162">Int32</span></span>|<span data-ttu-id="c966d-163">Número de usuários em não conformidade.</span><span class="sxs-lookup"><span data-stu-id="c966d-163">Number of non compliant users.</span></span>|
|<span data-ttu-id="c966d-164">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="c966d-164">remediatedUserCount</span></span>|<span data-ttu-id="c966d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c966d-165">Int32</span></span>|<span data-ttu-id="c966d-166">Número de usuários corrigidos.</span><span class="sxs-lookup"><span data-stu-id="c966d-166">Number of remediated users.</span></span>|
|<span data-ttu-id="c966d-167">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="c966d-167">errorUserCount</span></span>|<span data-ttu-id="c966d-168">Int32</span><span class="sxs-lookup"><span data-stu-id="c966d-168">Int32</span></span>|<span data-ttu-id="c966d-169">Número de usuários com erro.</span><span class="sxs-lookup"><span data-stu-id="c966d-169">Number of users had error.</span></span>|
|<span data-ttu-id="c966d-170">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="c966d-170">unknownUserCount</span></span>|<span data-ttu-id="c966d-171">Int32</span><span class="sxs-lookup"><span data-stu-id="c966d-171">Int32</span></span>|<span data-ttu-id="c966d-172">Número de usuários desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="c966d-172">Number of unknown users.</span></span>|
|<span data-ttu-id="c966d-173">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="c966d-173">conflictUserCount</span></span>|<span data-ttu-id="c966d-174">Int32</span><span class="sxs-lookup"><span data-stu-id="c966d-174">Int32</span></span>|<span data-ttu-id="c966d-175">Número de usuários com conflitos.</span><span class="sxs-lookup"><span data-stu-id="c966d-175">Number of conflict users.</span></span>|
|<span data-ttu-id="c966d-176">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="c966d-176">notApplicableUserCount</span></span>|<span data-ttu-id="c966d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c966d-177">Int32</span></span>|<span data-ttu-id="c966d-178">Número de usuários não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="c966d-178">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="c966d-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="c966d-179">Response</span></span>
<span data-ttu-id="c966d-180">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c966d-180">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c966d-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c966d-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="c966d-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c966d-182">Request</span></span>
<span data-ttu-id="c966d-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c966d-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/softwareUpdateStatusSummary
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

### <a name="response"></a><span data-ttu-id="c966d-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="c966d-184">Response</span></span>
<span data-ttu-id="c966d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c966d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



