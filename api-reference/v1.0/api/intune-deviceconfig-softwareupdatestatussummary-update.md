---
title: Atualizar softwareUpdateStatusSummary
description: Atualizar as propriedades de um objeto softwareUpdateStatusSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ea208150ac85aefb4fb3e34b4d081d02089bdee
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982410"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="a1c97-103">Atualizar softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="a1c97-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="a1c97-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1c97-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1c97-105">Atualizar as propriedades de um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="a1c97-105">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1c97-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1c97-106">Prerequisites</span></span>
<span data-ttu-id="a1c97-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1c97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1c97-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1c97-109">Permission type</span></span>|<span data-ttu-id="a1c97-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1c97-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1c97-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1c97-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a1c97-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1c97-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1c97-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1c97-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1c97-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1c97-114">Not supported.</span></span>|
|<span data-ttu-id="a1c97-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1c97-115">Application</span></span>|<span data-ttu-id="a1c97-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1c97-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1c97-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1c97-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="a1c97-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1c97-118">Request headers</span></span>
|<span data-ttu-id="a1c97-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1c97-119">Header</span></span>|<span data-ttu-id="a1c97-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a1c97-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1c97-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1c97-121">Authorization</span></span>|<span data-ttu-id="a1c97-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1c97-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1c97-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1c97-123">Accept</span></span>|<span data-ttu-id="a1c97-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a1c97-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1c97-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1c97-125">Request body</span></span>
<span data-ttu-id="a1c97-126">No corpo da solicitação, forneça uma representação JSON do objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="a1c97-126">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="a1c97-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="a1c97-127">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="a1c97-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1c97-128">Property</span></span>|<span data-ttu-id="a1c97-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1c97-129">Type</span></span>|<span data-ttu-id="a1c97-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1c97-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1c97-131">id</span><span class="sxs-lookup"><span data-stu-id="a1c97-131">id</span></span>|<span data-ttu-id="a1c97-132">String</span><span class="sxs-lookup"><span data-stu-id="a1c97-132">String</span></span>|<span data-ttu-id="a1c97-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a1c97-133">Key of the entity.</span></span>|
|<span data-ttu-id="a1c97-134">displayName</span><span class="sxs-lookup"><span data-stu-id="a1c97-134">displayName</span></span>|<span data-ttu-id="a1c97-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1c97-135">String</span></span>|<span data-ttu-id="a1c97-136">O nome da política.</span><span class="sxs-lookup"><span data-stu-id="a1c97-136">The name of the policy.</span></span>|
|<span data-ttu-id="a1c97-137">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a1c97-137">compliantDeviceCount</span></span>|<span data-ttu-id="a1c97-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a1c97-138">Int32</span></span>|<span data-ttu-id="a1c97-139">Número de dispositivos em conformidade.</span><span class="sxs-lookup"><span data-stu-id="a1c97-139">Number of compliant devices.</span></span>|
|<span data-ttu-id="a1c97-140">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a1c97-140">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a1c97-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a1c97-141">Int32</span></span>|<span data-ttu-id="a1c97-142">Número de dispositivos sem conformidade.</span><span class="sxs-lookup"><span data-stu-id="a1c97-142">Number of non compliant devices.</span></span>|
|<span data-ttu-id="a1c97-143">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a1c97-143">remediatedDeviceCount</span></span>|<span data-ttu-id="a1c97-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a1c97-144">Int32</span></span>|<span data-ttu-id="a1c97-145">Número de dispositivos corrigidos.</span><span class="sxs-lookup"><span data-stu-id="a1c97-145">Number of remediated devices.</span></span>|
|<span data-ttu-id="a1c97-146">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a1c97-146">errorDeviceCount</span></span>|<span data-ttu-id="a1c97-147">Int32</span><span class="sxs-lookup"><span data-stu-id="a1c97-147">Int32</span></span>|<span data-ttu-id="a1c97-148">Número de dispositivos com erro.</span><span class="sxs-lookup"><span data-stu-id="a1c97-148">Number of devices had error.</span></span>|
|<span data-ttu-id="a1c97-149">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a1c97-149">unknownDeviceCount</span></span>|<span data-ttu-id="a1c97-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a1c97-150">Int32</span></span>|<span data-ttu-id="a1c97-151">Número de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="a1c97-151">Number of unknown devices.</span></span>|
|<span data-ttu-id="a1c97-152">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a1c97-152">conflictDeviceCount</span></span>|<span data-ttu-id="a1c97-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a1c97-153">Int32</span></span>|<span data-ttu-id="a1c97-154">Número de dispositivos em conflito.</span><span class="sxs-lookup"><span data-stu-id="a1c97-154">Number of conflict devices.</span></span>|
|<span data-ttu-id="a1c97-155">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a1c97-155">notApplicableDeviceCount</span></span>|<span data-ttu-id="a1c97-156">Int32</span><span class="sxs-lookup"><span data-stu-id="a1c97-156">Int32</span></span>|<span data-ttu-id="a1c97-157">Número de dispositivos não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="a1c97-157">Number of not applicable devices.</span></span>|
|<span data-ttu-id="a1c97-158">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="a1c97-158">compliantUserCount</span></span>|<span data-ttu-id="a1c97-159">Int32</span><span class="sxs-lookup"><span data-stu-id="a1c97-159">Int32</span></span>|<span data-ttu-id="a1c97-160">Número de usuários em conformidade.</span><span class="sxs-lookup"><span data-stu-id="a1c97-160">Number of compliant users.</span></span>|
|<span data-ttu-id="a1c97-161">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="a1c97-161">nonCompliantUserCount</span></span>|<span data-ttu-id="a1c97-162">Int32</span><span class="sxs-lookup"><span data-stu-id="a1c97-162">Int32</span></span>|<span data-ttu-id="a1c97-163">Número de usuários em não conformidade.</span><span class="sxs-lookup"><span data-stu-id="a1c97-163">Number of non compliant users.</span></span>|
|<span data-ttu-id="a1c97-164">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="a1c97-164">remediatedUserCount</span></span>|<span data-ttu-id="a1c97-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a1c97-165">Int32</span></span>|<span data-ttu-id="a1c97-166">Número de usuários corrigidos.</span><span class="sxs-lookup"><span data-stu-id="a1c97-166">Number of remediated users.</span></span>|
|<span data-ttu-id="a1c97-167">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="a1c97-167">errorUserCount</span></span>|<span data-ttu-id="a1c97-168">Int32</span><span class="sxs-lookup"><span data-stu-id="a1c97-168">Int32</span></span>|<span data-ttu-id="a1c97-169">Número de usuários com erro.</span><span class="sxs-lookup"><span data-stu-id="a1c97-169">Number of users had error.</span></span>|
|<span data-ttu-id="a1c97-170">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="a1c97-170">unknownUserCount</span></span>|<span data-ttu-id="a1c97-171">Int32</span><span class="sxs-lookup"><span data-stu-id="a1c97-171">Int32</span></span>|<span data-ttu-id="a1c97-172">Número de usuários desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="a1c97-172">Number of unknown users.</span></span>|
|<span data-ttu-id="a1c97-173">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="a1c97-173">conflictUserCount</span></span>|<span data-ttu-id="a1c97-174">Int32</span><span class="sxs-lookup"><span data-stu-id="a1c97-174">Int32</span></span>|<span data-ttu-id="a1c97-175">Número de usuários com conflitos.</span><span class="sxs-lookup"><span data-stu-id="a1c97-175">Number of conflict users.</span></span>|
|<span data-ttu-id="a1c97-176">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="a1c97-176">notApplicableUserCount</span></span>|<span data-ttu-id="a1c97-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a1c97-177">Int32</span></span>|<span data-ttu-id="a1c97-178">Número de usuários não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="a1c97-178">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="a1c97-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1c97-179">Response</span></span>
<span data-ttu-id="a1c97-180">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1c97-180">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1c97-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1c97-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1c97-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1c97-182">Request</span></span>
<span data-ttu-id="a1c97-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1c97-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a1c97-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1c97-184">Response</span></span>
<span data-ttu-id="a1c97-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1c97-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



