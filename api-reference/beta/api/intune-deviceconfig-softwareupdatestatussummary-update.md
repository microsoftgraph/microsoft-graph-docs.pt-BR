---
title: Atualizar softwareUpdateStatusSummary
description: Atualizar as propriedades de um objeto softwareUpdateStatusSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9696daa56c723a8bc6d5ef9d3d674ce16c6e2667
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984812"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="999a3-103">Atualizar softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="999a3-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="999a3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="999a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="999a3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="999a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="999a3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="999a3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="999a3-107">Atualizar as propriedades de um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="999a3-107">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="999a3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="999a3-108">Prerequisites</span></span>
<span data-ttu-id="999a3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="999a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="999a3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="999a3-111">Permission type</span></span>|<span data-ttu-id="999a3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="999a3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="999a3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="999a3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="999a3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="999a3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="999a3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="999a3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="999a3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="999a3-116">Not supported.</span></span>|
|<span data-ttu-id="999a3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="999a3-117">Application</span></span>|<span data-ttu-id="999a3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="999a3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="999a3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="999a3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="999a3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="999a3-120">Request headers</span></span>
|<span data-ttu-id="999a3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="999a3-121">Header</span></span>|<span data-ttu-id="999a3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="999a3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="999a3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="999a3-123">Authorization</span></span>|<span data-ttu-id="999a3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="999a3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="999a3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="999a3-125">Accept</span></span>|<span data-ttu-id="999a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="999a3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="999a3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="999a3-127">Request body</span></span>
<span data-ttu-id="999a3-128">No corpo da solicitação, forneça uma representação JSON do objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="999a3-128">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="999a3-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="999a3-129">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="999a3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="999a3-130">Property</span></span>|<span data-ttu-id="999a3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="999a3-131">Type</span></span>|<span data-ttu-id="999a3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="999a3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="999a3-133">id</span><span class="sxs-lookup"><span data-stu-id="999a3-133">id</span></span>|<span data-ttu-id="999a3-134">String</span><span class="sxs-lookup"><span data-stu-id="999a3-134">String</span></span>|<span data-ttu-id="999a3-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="999a3-135">Key of the entity.</span></span>|
|<span data-ttu-id="999a3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="999a3-136">displayName</span></span>|<span data-ttu-id="999a3-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="999a3-137">String</span></span>|<span data-ttu-id="999a3-138">O nome da política.</span><span class="sxs-lookup"><span data-stu-id="999a3-138">The name of the policy.</span></span>|
|<span data-ttu-id="999a3-139">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="999a3-139">compliantDeviceCount</span></span>|<span data-ttu-id="999a3-140">Int32</span><span class="sxs-lookup"><span data-stu-id="999a3-140">Int32</span></span>|<span data-ttu-id="999a3-141">Número de dispositivos em conformidade.</span><span class="sxs-lookup"><span data-stu-id="999a3-141">Number of compliant devices.</span></span>|
|<span data-ttu-id="999a3-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="999a3-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="999a3-143">Int32</span><span class="sxs-lookup"><span data-stu-id="999a3-143">Int32</span></span>|<span data-ttu-id="999a3-144">Número de dispositivos sem conformidade.</span><span class="sxs-lookup"><span data-stu-id="999a3-144">Number of non compliant devices.</span></span>|
|<span data-ttu-id="999a3-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="999a3-145">remediatedDeviceCount</span></span>|<span data-ttu-id="999a3-146">Int32</span><span class="sxs-lookup"><span data-stu-id="999a3-146">Int32</span></span>|<span data-ttu-id="999a3-147">Número de dispositivos corrigidos.</span><span class="sxs-lookup"><span data-stu-id="999a3-147">Number of remediated devices.</span></span>|
|<span data-ttu-id="999a3-148">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="999a3-148">errorDeviceCount</span></span>|<span data-ttu-id="999a3-149">Int32</span><span class="sxs-lookup"><span data-stu-id="999a3-149">Int32</span></span>|<span data-ttu-id="999a3-150">Número de dispositivos com erro.</span><span class="sxs-lookup"><span data-stu-id="999a3-150">Number of devices had error.</span></span>|
|<span data-ttu-id="999a3-151">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="999a3-151">unknownDeviceCount</span></span>|<span data-ttu-id="999a3-152">Int32</span><span class="sxs-lookup"><span data-stu-id="999a3-152">Int32</span></span>|<span data-ttu-id="999a3-153">Número de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="999a3-153">Number of unknown devices.</span></span>|
|<span data-ttu-id="999a3-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="999a3-154">conflictDeviceCount</span></span>|<span data-ttu-id="999a3-155">Int32</span><span class="sxs-lookup"><span data-stu-id="999a3-155">Int32</span></span>|<span data-ttu-id="999a3-156">Número de dispositivos em conflito.</span><span class="sxs-lookup"><span data-stu-id="999a3-156">Number of conflict devices.</span></span>|
|<span data-ttu-id="999a3-157">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="999a3-157">notApplicableDeviceCount</span></span>|<span data-ttu-id="999a3-158">Int32</span><span class="sxs-lookup"><span data-stu-id="999a3-158">Int32</span></span>|<span data-ttu-id="999a3-159">Número de dispositivos não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="999a3-159">Number of not applicable devices.</span></span>|
|<span data-ttu-id="999a3-160">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="999a3-160">compliantUserCount</span></span>|<span data-ttu-id="999a3-161">Int32</span><span class="sxs-lookup"><span data-stu-id="999a3-161">Int32</span></span>|<span data-ttu-id="999a3-162">Número de usuários em conformidade.</span><span class="sxs-lookup"><span data-stu-id="999a3-162">Number of compliant users.</span></span>|
|<span data-ttu-id="999a3-163">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="999a3-163">nonCompliantUserCount</span></span>|<span data-ttu-id="999a3-164">Int32</span><span class="sxs-lookup"><span data-stu-id="999a3-164">Int32</span></span>|<span data-ttu-id="999a3-165">Número de usuários em não conformidade.</span><span class="sxs-lookup"><span data-stu-id="999a3-165">Number of non compliant users.</span></span>|
|<span data-ttu-id="999a3-166">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="999a3-166">remediatedUserCount</span></span>|<span data-ttu-id="999a3-167">Int32</span><span class="sxs-lookup"><span data-stu-id="999a3-167">Int32</span></span>|<span data-ttu-id="999a3-168">Número de usuários corrigidos.</span><span class="sxs-lookup"><span data-stu-id="999a3-168">Number of remediated users.</span></span>|
|<span data-ttu-id="999a3-169">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="999a3-169">errorUserCount</span></span>|<span data-ttu-id="999a3-170">Int32</span><span class="sxs-lookup"><span data-stu-id="999a3-170">Int32</span></span>|<span data-ttu-id="999a3-171">Número de usuários com erro.</span><span class="sxs-lookup"><span data-stu-id="999a3-171">Number of users had error.</span></span>|
|<span data-ttu-id="999a3-172">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="999a3-172">unknownUserCount</span></span>|<span data-ttu-id="999a3-173">Int32</span><span class="sxs-lookup"><span data-stu-id="999a3-173">Int32</span></span>|<span data-ttu-id="999a3-174">Número de usuários desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="999a3-174">Number of unknown users.</span></span>|
|<span data-ttu-id="999a3-175">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="999a3-175">conflictUserCount</span></span>|<span data-ttu-id="999a3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="999a3-176">Int32</span></span>|<span data-ttu-id="999a3-177">Número de usuários com conflitos.</span><span class="sxs-lookup"><span data-stu-id="999a3-177">Number of conflict users.</span></span>|
|<span data-ttu-id="999a3-178">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="999a3-178">notApplicableUserCount</span></span>|<span data-ttu-id="999a3-179">Int32</span><span class="sxs-lookup"><span data-stu-id="999a3-179">Int32</span></span>|<span data-ttu-id="999a3-180">Número de usuários não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="999a3-180">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="999a3-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="999a3-181">Response</span></span>
<span data-ttu-id="999a3-182">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="999a3-182">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="999a3-183">Exemplo</span><span class="sxs-lookup"><span data-stu-id="999a3-183">Example</span></span>
### <a name="request"></a><span data-ttu-id="999a3-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="999a3-184">Request</span></span>
<span data-ttu-id="999a3-185">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="999a3-185">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/softwareUpdateStatusSummary
Content-type: application/json
Content-length: 452

{
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

### <a name="response"></a><span data-ttu-id="999a3-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="999a3-186">Response</span></span>
<span data-ttu-id="999a3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="999a3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





