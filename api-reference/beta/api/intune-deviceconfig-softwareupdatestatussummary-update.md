---
title: Atualizar softwareUpdateStatusSummary
description: Atualizar as propriedades de um objeto softwareUpdateStatusSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 40f85340e9eb3f80e09610f187669f905214dbda
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947740"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="19b5a-103">Atualizar softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="19b5a-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="19b5a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="19b5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19b5a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="19b5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19b5a-106">Atualizar as propriedades de um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="19b5a-106">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19b5a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="19b5a-107">Prerequisites</span></span>
<span data-ttu-id="19b5a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19b5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19b5a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19b5a-110">Permission type</span></span>|<span data-ttu-id="19b5a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="19b5a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19b5a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19b5a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19b5a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19b5a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="19b5a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19b5a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19b5a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19b5a-115">Not supported.</span></span>|
|<span data-ttu-id="19b5a-116">Application</span><span class="sxs-lookup"><span data-stu-id="19b5a-116">Application</span></span>|<span data-ttu-id="19b5a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19b5a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="19b5a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19b5a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="19b5a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19b5a-119">Request headers</span></span>
|<span data-ttu-id="19b5a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="19b5a-120">Header</span></span>|<span data-ttu-id="19b5a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="19b5a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19b5a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="19b5a-122">Authorization</span></span>|<span data-ttu-id="19b5a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19b5a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19b5a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="19b5a-124">Accept</span></span>|<span data-ttu-id="19b5a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="19b5a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19b5a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19b5a-126">Request body</span></span>
<span data-ttu-id="19b5a-127">No corpo da solicitação, forneça uma representação JSON do objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="19b5a-127">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="19b5a-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="19b5a-128">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="19b5a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19b5a-129">Property</span></span>|<span data-ttu-id="19b5a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="19b5a-130">Type</span></span>|<span data-ttu-id="19b5a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="19b5a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19b5a-132">id</span><span class="sxs-lookup"><span data-stu-id="19b5a-132">id</span></span>|<span data-ttu-id="19b5a-133">String</span><span class="sxs-lookup"><span data-stu-id="19b5a-133">String</span></span>|<span data-ttu-id="19b5a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="19b5a-134">Key of the entity.</span></span>|
|<span data-ttu-id="19b5a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="19b5a-135">displayName</span></span>|<span data-ttu-id="19b5a-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19b5a-136">String</span></span>|<span data-ttu-id="19b5a-137">O nome da política.</span><span class="sxs-lookup"><span data-stu-id="19b5a-137">The name of the policy.</span></span>|
|<span data-ttu-id="19b5a-138">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19b5a-138">compliantDeviceCount</span></span>|<span data-ttu-id="19b5a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="19b5a-139">Int32</span></span>|<span data-ttu-id="19b5a-140">Número de dispositivos em conformidade.</span><span class="sxs-lookup"><span data-stu-id="19b5a-140">Number of compliant devices.</span></span>|
|<span data-ttu-id="19b5a-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19b5a-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="19b5a-142">Int32</span><span class="sxs-lookup"><span data-stu-id="19b5a-142">Int32</span></span>|<span data-ttu-id="19b5a-143">Número de dispositivos sem conformidade.</span><span class="sxs-lookup"><span data-stu-id="19b5a-143">Number of non compliant devices.</span></span>|
|<span data-ttu-id="19b5a-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19b5a-144">remediatedDeviceCount</span></span>|<span data-ttu-id="19b5a-145">Int32</span><span class="sxs-lookup"><span data-stu-id="19b5a-145">Int32</span></span>|<span data-ttu-id="19b5a-146">Número de dispositivos corrigidos.</span><span class="sxs-lookup"><span data-stu-id="19b5a-146">Number of remediated devices.</span></span>|
|<span data-ttu-id="19b5a-147">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19b5a-147">errorDeviceCount</span></span>|<span data-ttu-id="19b5a-148">Int32</span><span class="sxs-lookup"><span data-stu-id="19b5a-148">Int32</span></span>|<span data-ttu-id="19b5a-149">Número de dispositivos com erro.</span><span class="sxs-lookup"><span data-stu-id="19b5a-149">Number of devices had error.</span></span>|
|<span data-ttu-id="19b5a-150">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19b5a-150">unknownDeviceCount</span></span>|<span data-ttu-id="19b5a-151">Int32</span><span class="sxs-lookup"><span data-stu-id="19b5a-151">Int32</span></span>|<span data-ttu-id="19b5a-152">Número de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="19b5a-152">Number of unknown devices.</span></span>|
|<span data-ttu-id="19b5a-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19b5a-153">conflictDeviceCount</span></span>|<span data-ttu-id="19b5a-154">Int32</span><span class="sxs-lookup"><span data-stu-id="19b5a-154">Int32</span></span>|<span data-ttu-id="19b5a-155">Número de dispositivos em conflito.</span><span class="sxs-lookup"><span data-stu-id="19b5a-155">Number of conflict devices.</span></span>|
|<span data-ttu-id="19b5a-156">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19b5a-156">notApplicableDeviceCount</span></span>|<span data-ttu-id="19b5a-157">Int32</span><span class="sxs-lookup"><span data-stu-id="19b5a-157">Int32</span></span>|<span data-ttu-id="19b5a-158">Número de dispositivos não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="19b5a-158">Number of not applicable devices.</span></span>|
|<span data-ttu-id="19b5a-159">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="19b5a-159">compliantUserCount</span></span>|<span data-ttu-id="19b5a-160">Int32</span><span class="sxs-lookup"><span data-stu-id="19b5a-160">Int32</span></span>|<span data-ttu-id="19b5a-161">Número de usuários em conformidade.</span><span class="sxs-lookup"><span data-stu-id="19b5a-161">Number of compliant users.</span></span>|
|<span data-ttu-id="19b5a-162">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="19b5a-162">nonCompliantUserCount</span></span>|<span data-ttu-id="19b5a-163">Int32</span><span class="sxs-lookup"><span data-stu-id="19b5a-163">Int32</span></span>|<span data-ttu-id="19b5a-164">Número de usuários em não conformidade.</span><span class="sxs-lookup"><span data-stu-id="19b5a-164">Number of non compliant users.</span></span>|
|<span data-ttu-id="19b5a-165">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="19b5a-165">remediatedUserCount</span></span>|<span data-ttu-id="19b5a-166">Int32</span><span class="sxs-lookup"><span data-stu-id="19b5a-166">Int32</span></span>|<span data-ttu-id="19b5a-167">Número de usuários corrigidos.</span><span class="sxs-lookup"><span data-stu-id="19b5a-167">Number of remediated users.</span></span>|
|<span data-ttu-id="19b5a-168">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="19b5a-168">errorUserCount</span></span>|<span data-ttu-id="19b5a-169">Int32</span><span class="sxs-lookup"><span data-stu-id="19b5a-169">Int32</span></span>|<span data-ttu-id="19b5a-170">Número de usuários com erro.</span><span class="sxs-lookup"><span data-stu-id="19b5a-170">Number of users had error.</span></span>|
|<span data-ttu-id="19b5a-171">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="19b5a-171">unknownUserCount</span></span>|<span data-ttu-id="19b5a-172">Int32</span><span class="sxs-lookup"><span data-stu-id="19b5a-172">Int32</span></span>|<span data-ttu-id="19b5a-173">Número de usuários desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="19b5a-173">Number of unknown users.</span></span>|
|<span data-ttu-id="19b5a-174">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="19b5a-174">conflictUserCount</span></span>|<span data-ttu-id="19b5a-175">Int32</span><span class="sxs-lookup"><span data-stu-id="19b5a-175">Int32</span></span>|<span data-ttu-id="19b5a-176">Número de usuários com conflitos.</span><span class="sxs-lookup"><span data-stu-id="19b5a-176">Number of conflict users.</span></span>|
|<span data-ttu-id="19b5a-177">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="19b5a-177">notApplicableUserCount</span></span>|<span data-ttu-id="19b5a-178">Int32</span><span class="sxs-lookup"><span data-stu-id="19b5a-178">Int32</span></span>|<span data-ttu-id="19b5a-179">Número de usuários não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="19b5a-179">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="19b5a-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="19b5a-180">Response</span></span>
<span data-ttu-id="19b5a-181">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19b5a-181">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19b5a-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19b5a-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="19b5a-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19b5a-183">Request</span></span>
<span data-ttu-id="19b5a-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19b5a-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="19b5a-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="19b5a-185">Response</span></span>
<span data-ttu-id="19b5a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19b5a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





