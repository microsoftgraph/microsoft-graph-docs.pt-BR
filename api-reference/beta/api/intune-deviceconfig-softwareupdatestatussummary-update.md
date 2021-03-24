---
title: Atualizar softwareUpdateStatusSummary
description: Atualizar as propriedades de um objeto softwareUpdateStatusSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a35c52de0da15a20c4607ae7626f9c989795a41d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137053"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="a8513-103">Atualizar softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="a8513-103">Update softwareUpdateStatusSummary</span></span>

<span data-ttu-id="a8513-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8513-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8513-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a8513-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8513-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8513-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8513-107">Atualizar as propriedades de um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="a8513-107">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8513-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a8513-108">Prerequisites</span></span>
<span data-ttu-id="a8513-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8513-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8513-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8513-111">Permission type</span></span>|<span data-ttu-id="a8513-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8513-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8513-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8513-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8513-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8513-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a8513-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8513-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8513-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8513-116">Not supported.</span></span>|
|<span data-ttu-id="a8513-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8513-117">Application</span></span>|<span data-ttu-id="a8513-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8513-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8513-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8513-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="a8513-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8513-120">Request headers</span></span>
|<span data-ttu-id="a8513-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8513-121">Header</span></span>|<span data-ttu-id="a8513-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a8513-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8513-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8513-123">Authorization</span></span>|<span data-ttu-id="a8513-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8513-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8513-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a8513-125">Accept</span></span>|<span data-ttu-id="a8513-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8513-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8513-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8513-127">Request body</span></span>
<span data-ttu-id="a8513-128">No corpo da solicitação, forneça uma representação JSON do objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="a8513-128">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="a8513-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="a8513-129">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="a8513-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8513-130">Property</span></span>|<span data-ttu-id="a8513-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8513-131">Type</span></span>|<span data-ttu-id="a8513-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8513-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8513-133">id</span><span class="sxs-lookup"><span data-stu-id="a8513-133">id</span></span>|<span data-ttu-id="a8513-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8513-134">String</span></span>|<span data-ttu-id="a8513-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a8513-135">Key of the entity.</span></span>|
|<span data-ttu-id="a8513-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a8513-136">displayName</span></span>|<span data-ttu-id="a8513-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8513-137">String</span></span>|<span data-ttu-id="a8513-138">O nome da política.</span><span class="sxs-lookup"><span data-stu-id="a8513-138">The name of the policy.</span></span>|
|<span data-ttu-id="a8513-139">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8513-139">compliantDeviceCount</span></span>|<span data-ttu-id="a8513-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a8513-140">Int32</span></span>|<span data-ttu-id="a8513-141">Número de dispositivos em conformidade.</span><span class="sxs-lookup"><span data-stu-id="a8513-141">Number of compliant devices.</span></span>|
|<span data-ttu-id="a8513-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8513-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a8513-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a8513-143">Int32</span></span>|<span data-ttu-id="a8513-144">Número de dispositivos sem conformidade.</span><span class="sxs-lookup"><span data-stu-id="a8513-144">Number of non compliant devices.</span></span>|
|<span data-ttu-id="a8513-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8513-145">remediatedDeviceCount</span></span>|<span data-ttu-id="a8513-146">Int32</span><span class="sxs-lookup"><span data-stu-id="a8513-146">Int32</span></span>|<span data-ttu-id="a8513-147">Número de dispositivos corrigidos.</span><span class="sxs-lookup"><span data-stu-id="a8513-147">Number of remediated devices.</span></span>|
|<span data-ttu-id="a8513-148">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8513-148">errorDeviceCount</span></span>|<span data-ttu-id="a8513-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a8513-149">Int32</span></span>|<span data-ttu-id="a8513-150">Número de dispositivos com erro.</span><span class="sxs-lookup"><span data-stu-id="a8513-150">Number of devices had error.</span></span>|
|<span data-ttu-id="a8513-151">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8513-151">unknownDeviceCount</span></span>|<span data-ttu-id="a8513-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a8513-152">Int32</span></span>|<span data-ttu-id="a8513-153">Número de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="a8513-153">Number of unknown devices.</span></span>|
|<span data-ttu-id="a8513-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8513-154">conflictDeviceCount</span></span>|<span data-ttu-id="a8513-155">Int32</span><span class="sxs-lookup"><span data-stu-id="a8513-155">Int32</span></span>|<span data-ttu-id="a8513-156">Número de dispositivos em conflito.</span><span class="sxs-lookup"><span data-stu-id="a8513-156">Number of conflict devices.</span></span>|
|<span data-ttu-id="a8513-157">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8513-157">notApplicableDeviceCount</span></span>|<span data-ttu-id="a8513-158">Int32</span><span class="sxs-lookup"><span data-stu-id="a8513-158">Int32</span></span>|<span data-ttu-id="a8513-159">Número de dispositivos não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="a8513-159">Number of not applicable devices.</span></span>|
|<span data-ttu-id="a8513-160">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="a8513-160">compliantUserCount</span></span>|<span data-ttu-id="a8513-161">Int32</span><span class="sxs-lookup"><span data-stu-id="a8513-161">Int32</span></span>|<span data-ttu-id="a8513-162">Número de usuários em conformidade.</span><span class="sxs-lookup"><span data-stu-id="a8513-162">Number of compliant users.</span></span>|
|<span data-ttu-id="a8513-163">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="a8513-163">nonCompliantUserCount</span></span>|<span data-ttu-id="a8513-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a8513-164">Int32</span></span>|<span data-ttu-id="a8513-165">Número de usuários em não conformidade.</span><span class="sxs-lookup"><span data-stu-id="a8513-165">Number of non compliant users.</span></span>|
|<span data-ttu-id="a8513-166">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="a8513-166">remediatedUserCount</span></span>|<span data-ttu-id="a8513-167">Int32</span><span class="sxs-lookup"><span data-stu-id="a8513-167">Int32</span></span>|<span data-ttu-id="a8513-168">Número de usuários corrigidos.</span><span class="sxs-lookup"><span data-stu-id="a8513-168">Number of remediated users.</span></span>|
|<span data-ttu-id="a8513-169">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="a8513-169">errorUserCount</span></span>|<span data-ttu-id="a8513-170">Int32</span><span class="sxs-lookup"><span data-stu-id="a8513-170">Int32</span></span>|<span data-ttu-id="a8513-171">Número de usuários com erro.</span><span class="sxs-lookup"><span data-stu-id="a8513-171">Number of users had error.</span></span>|
|<span data-ttu-id="a8513-172">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="a8513-172">unknownUserCount</span></span>|<span data-ttu-id="a8513-173">Int32</span><span class="sxs-lookup"><span data-stu-id="a8513-173">Int32</span></span>|<span data-ttu-id="a8513-174">Número de usuários desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="a8513-174">Number of unknown users.</span></span>|
|<span data-ttu-id="a8513-175">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="a8513-175">conflictUserCount</span></span>|<span data-ttu-id="a8513-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a8513-176">Int32</span></span>|<span data-ttu-id="a8513-177">Número de usuários com conflitos.</span><span class="sxs-lookup"><span data-stu-id="a8513-177">Number of conflict users.</span></span>|
|<span data-ttu-id="a8513-178">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="a8513-178">notApplicableUserCount</span></span>|<span data-ttu-id="a8513-179">Int32</span><span class="sxs-lookup"><span data-stu-id="a8513-179">Int32</span></span>|<span data-ttu-id="a8513-180">Número de usuários não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="a8513-180">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="a8513-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8513-181">Response</span></span>
<span data-ttu-id="a8513-182">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8513-182">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8513-183">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8513-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8513-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8513-184">Request</span></span>
<span data-ttu-id="a8513-185">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8513-185">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a8513-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8513-186">Response</span></span>
<span data-ttu-id="a8513-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8513-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




