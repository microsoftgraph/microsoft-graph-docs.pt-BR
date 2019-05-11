---
title: Atualizar softwareUpdateStatusSummary
description: Atualizar as propriedades de um objeto softwareUpdateStatusSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2cc4bf0486a0d5e1a8e210ee2507d5201e749e23
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33921839"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="44834-103">Atualizar softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="44834-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="44834-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="44834-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44834-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="44834-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44834-106">Atualizar as propriedades de um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="44834-106">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44834-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="44834-107">Prerequisites</span></span>
<span data-ttu-id="44834-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44834-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44834-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44834-110">Permission type</span></span>|<span data-ttu-id="44834-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="44834-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44834-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44834-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44834-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44834-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44834-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44834-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44834-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44834-115">Not supported.</span></span>|
|<span data-ttu-id="44834-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44834-116">Application</span></span>|<span data-ttu-id="44834-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44834-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44834-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44834-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="44834-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44834-119">Request headers</span></span>
|<span data-ttu-id="44834-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="44834-120">Header</span></span>|<span data-ttu-id="44834-121">Valor</span><span class="sxs-lookup"><span data-stu-id="44834-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44834-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="44834-122">Authorization</span></span>|<span data-ttu-id="44834-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44834-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44834-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="44834-124">Accept</span></span>|<span data-ttu-id="44834-125">application/json</span><span class="sxs-lookup"><span data-stu-id="44834-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44834-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44834-126">Request body</span></span>
<span data-ttu-id="44834-127">No corpo da solicitação, forneça uma representação JSON do objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="44834-127">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="44834-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="44834-128">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="44834-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44834-129">Property</span></span>|<span data-ttu-id="44834-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="44834-130">Type</span></span>|<span data-ttu-id="44834-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="44834-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44834-132">id</span><span class="sxs-lookup"><span data-stu-id="44834-132">id</span></span>|<span data-ttu-id="44834-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44834-133">String</span></span>|<span data-ttu-id="44834-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="44834-134">Key of the entity.</span></span>|
|<span data-ttu-id="44834-135">displayName</span><span class="sxs-lookup"><span data-stu-id="44834-135">displayName</span></span>|<span data-ttu-id="44834-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44834-136">String</span></span>|<span data-ttu-id="44834-137">O nome da política.</span><span class="sxs-lookup"><span data-stu-id="44834-137">The name of the policy.</span></span>|
|<span data-ttu-id="44834-138">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44834-138">compliantDeviceCount</span></span>|<span data-ttu-id="44834-139">Int32</span><span class="sxs-lookup"><span data-stu-id="44834-139">Int32</span></span>|<span data-ttu-id="44834-140">Número de dispositivos em conformidade.</span><span class="sxs-lookup"><span data-stu-id="44834-140">Number of compliant devices.</span></span>|
|<span data-ttu-id="44834-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44834-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="44834-142">Int32</span><span class="sxs-lookup"><span data-stu-id="44834-142">Int32</span></span>|<span data-ttu-id="44834-143">Número de dispositivos sem conformidade.</span><span class="sxs-lookup"><span data-stu-id="44834-143">Number of non compliant devices.</span></span>|
|<span data-ttu-id="44834-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44834-144">remediatedDeviceCount</span></span>|<span data-ttu-id="44834-145">Int32</span><span class="sxs-lookup"><span data-stu-id="44834-145">Int32</span></span>|<span data-ttu-id="44834-146">Número de dispositivos corrigidos.</span><span class="sxs-lookup"><span data-stu-id="44834-146">Number of remediated devices.</span></span>|
|<span data-ttu-id="44834-147">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44834-147">errorDeviceCount</span></span>|<span data-ttu-id="44834-148">Int32</span><span class="sxs-lookup"><span data-stu-id="44834-148">Int32</span></span>|<span data-ttu-id="44834-149">Número de dispositivos com erro.</span><span class="sxs-lookup"><span data-stu-id="44834-149">Number of devices had error.</span></span>|
|<span data-ttu-id="44834-150">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44834-150">unknownDeviceCount</span></span>|<span data-ttu-id="44834-151">Int32</span><span class="sxs-lookup"><span data-stu-id="44834-151">Int32</span></span>|<span data-ttu-id="44834-152">Número de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="44834-152">Number of unknown devices.</span></span>|
|<span data-ttu-id="44834-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44834-153">conflictDeviceCount</span></span>|<span data-ttu-id="44834-154">Int32</span><span class="sxs-lookup"><span data-stu-id="44834-154">Int32</span></span>|<span data-ttu-id="44834-155">Número de dispositivos em conflito.</span><span class="sxs-lookup"><span data-stu-id="44834-155">Number of conflict devices.</span></span>|
|<span data-ttu-id="44834-156">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44834-156">notApplicableDeviceCount</span></span>|<span data-ttu-id="44834-157">Int32</span><span class="sxs-lookup"><span data-stu-id="44834-157">Int32</span></span>|<span data-ttu-id="44834-158">Número de dispositivos não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="44834-158">Number of not applicable devices.</span></span>|
|<span data-ttu-id="44834-159">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="44834-159">compliantUserCount</span></span>|<span data-ttu-id="44834-160">Int32</span><span class="sxs-lookup"><span data-stu-id="44834-160">Int32</span></span>|<span data-ttu-id="44834-161">Número de usuários em conformidade.</span><span class="sxs-lookup"><span data-stu-id="44834-161">Number of compliant users.</span></span>|
|<span data-ttu-id="44834-162">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="44834-162">nonCompliantUserCount</span></span>|<span data-ttu-id="44834-163">Int32</span><span class="sxs-lookup"><span data-stu-id="44834-163">Int32</span></span>|<span data-ttu-id="44834-164">Número de usuários em não conformidade.</span><span class="sxs-lookup"><span data-stu-id="44834-164">Number of non compliant users.</span></span>|
|<span data-ttu-id="44834-165">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="44834-165">remediatedUserCount</span></span>|<span data-ttu-id="44834-166">Int32</span><span class="sxs-lookup"><span data-stu-id="44834-166">Int32</span></span>|<span data-ttu-id="44834-167">Número de usuários corrigidos.</span><span class="sxs-lookup"><span data-stu-id="44834-167">Number of remediated users.</span></span>|
|<span data-ttu-id="44834-168">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="44834-168">errorUserCount</span></span>|<span data-ttu-id="44834-169">Int32</span><span class="sxs-lookup"><span data-stu-id="44834-169">Int32</span></span>|<span data-ttu-id="44834-170">Número de usuários com erro.</span><span class="sxs-lookup"><span data-stu-id="44834-170">Number of users had error.</span></span>|
|<span data-ttu-id="44834-171">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="44834-171">unknownUserCount</span></span>|<span data-ttu-id="44834-172">Int32</span><span class="sxs-lookup"><span data-stu-id="44834-172">Int32</span></span>|<span data-ttu-id="44834-173">Número de usuários desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="44834-173">Number of unknown users.</span></span>|
|<span data-ttu-id="44834-174">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="44834-174">conflictUserCount</span></span>|<span data-ttu-id="44834-175">Int32</span><span class="sxs-lookup"><span data-stu-id="44834-175">Int32</span></span>|<span data-ttu-id="44834-176">Número de usuários com conflitos.</span><span class="sxs-lookup"><span data-stu-id="44834-176">Number of conflict users.</span></span>|
|<span data-ttu-id="44834-177">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="44834-177">notApplicableUserCount</span></span>|<span data-ttu-id="44834-178">Int32</span><span class="sxs-lookup"><span data-stu-id="44834-178">Int32</span></span>|<span data-ttu-id="44834-179">Número de usuários não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="44834-179">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="44834-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="44834-180">Response</span></span>
<span data-ttu-id="44834-181">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44834-181">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44834-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44834-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="44834-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44834-183">Request</span></span>
<span data-ttu-id="44834-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44834-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="44834-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="44834-185">Response</span></span>
<span data-ttu-id="44834-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="44834-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




