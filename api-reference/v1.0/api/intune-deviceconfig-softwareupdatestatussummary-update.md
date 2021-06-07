---
title: Atualizar softwareUpdateStatusSummary
description: Atualizar as propriedades de um objeto softwareUpdateStatusSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 48585dc0ccd4605c84e5bad0b8395f30bc248707
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756236"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="eb6c6-103">Atualizar softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="eb6c6-103">Update softwareUpdateStatusSummary</span></span>

<span data-ttu-id="eb6c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb6c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb6c6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb6c6-106">Atualizar as propriedades de um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="eb6c6-106">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb6c6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eb6c6-107">Prerequisites</span></span>
<span data-ttu-id="eb6c6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb6c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb6c6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb6c6-110">Permission type</span></span>|<span data-ttu-id="eb6c6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb6c6-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb6c6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb6c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb6c6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb6c6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eb6c6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb6c6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb6c6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-115">Not supported.</span></span>|
|<span data-ttu-id="eb6c6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb6c6-116">Application</span></span>|<span data-ttu-id="eb6c6-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb6c6-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb6c6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb6c6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="eb6c6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb6c6-119">Request headers</span></span>
|<span data-ttu-id="eb6c6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb6c6-120">Header</span></span>|<span data-ttu-id="eb6c6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="eb6c6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb6c6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb6c6-122">Authorization</span></span>|<span data-ttu-id="eb6c6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb6c6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eb6c6-124">Accept</span></span>|<span data-ttu-id="eb6c6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb6c6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb6c6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb6c6-126">Request body</span></span>
<span data-ttu-id="eb6c6-127">No corpo da solicitação, forneça uma representação JSON do objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="eb6c6-127">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="eb6c6-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="eb6c6-128">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="eb6c6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb6c6-129">Property</span></span>|<span data-ttu-id="eb6c6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb6c6-130">Type</span></span>|<span data-ttu-id="eb6c6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb6c6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb6c6-132">id</span><span class="sxs-lookup"><span data-stu-id="eb6c6-132">id</span></span>|<span data-ttu-id="eb6c6-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb6c6-133">String</span></span>|<span data-ttu-id="eb6c6-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-134">Key of the entity.</span></span>|
|<span data-ttu-id="eb6c6-135">displayName</span><span class="sxs-lookup"><span data-stu-id="eb6c6-135">displayName</span></span>|<span data-ttu-id="eb6c6-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb6c6-136">String</span></span>|<span data-ttu-id="eb6c6-137">O nome da política.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-137">The name of the policy.</span></span>|
|<span data-ttu-id="eb6c6-138">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eb6c6-138">compliantDeviceCount</span></span>|<span data-ttu-id="eb6c6-139">Int32</span><span class="sxs-lookup"><span data-stu-id="eb6c6-139">Int32</span></span>|<span data-ttu-id="eb6c6-140">Número de dispositivos em conformidade.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-140">Number of compliant devices.</span></span>|
|<span data-ttu-id="eb6c6-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eb6c6-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="eb6c6-142">Int32</span><span class="sxs-lookup"><span data-stu-id="eb6c6-142">Int32</span></span>|<span data-ttu-id="eb6c6-143">Número de dispositivos sem conformidade.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-143">Number of non compliant devices.</span></span>|
|<span data-ttu-id="eb6c6-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eb6c6-144">remediatedDeviceCount</span></span>|<span data-ttu-id="eb6c6-145">Int32</span><span class="sxs-lookup"><span data-stu-id="eb6c6-145">Int32</span></span>|<span data-ttu-id="eb6c6-146">Número de dispositivos corrigidos.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-146">Number of remediated devices.</span></span>|
|<span data-ttu-id="eb6c6-147">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eb6c6-147">errorDeviceCount</span></span>|<span data-ttu-id="eb6c6-148">Int32</span><span class="sxs-lookup"><span data-stu-id="eb6c6-148">Int32</span></span>|<span data-ttu-id="eb6c6-149">Número de dispositivos com erro.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-149">Number of devices had error.</span></span>|
|<span data-ttu-id="eb6c6-150">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eb6c6-150">unknownDeviceCount</span></span>|<span data-ttu-id="eb6c6-151">Int32</span><span class="sxs-lookup"><span data-stu-id="eb6c6-151">Int32</span></span>|<span data-ttu-id="eb6c6-152">Número de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-152">Number of unknown devices.</span></span>|
|<span data-ttu-id="eb6c6-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eb6c6-153">conflictDeviceCount</span></span>|<span data-ttu-id="eb6c6-154">Int32</span><span class="sxs-lookup"><span data-stu-id="eb6c6-154">Int32</span></span>|<span data-ttu-id="eb6c6-155">Número de dispositivos em conflito.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-155">Number of conflict devices.</span></span>|
|<span data-ttu-id="eb6c6-156">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eb6c6-156">notApplicableDeviceCount</span></span>|<span data-ttu-id="eb6c6-157">Int32</span><span class="sxs-lookup"><span data-stu-id="eb6c6-157">Int32</span></span>|<span data-ttu-id="eb6c6-158">Número de dispositivos não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-158">Number of not applicable devices.</span></span>|
|<span data-ttu-id="eb6c6-159">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="eb6c6-159">compliantUserCount</span></span>|<span data-ttu-id="eb6c6-160">Int32</span><span class="sxs-lookup"><span data-stu-id="eb6c6-160">Int32</span></span>|<span data-ttu-id="eb6c6-161">Número de usuários em conformidade.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-161">Number of compliant users.</span></span>|
|<span data-ttu-id="eb6c6-162">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="eb6c6-162">nonCompliantUserCount</span></span>|<span data-ttu-id="eb6c6-163">Int32</span><span class="sxs-lookup"><span data-stu-id="eb6c6-163">Int32</span></span>|<span data-ttu-id="eb6c6-164">Número de usuários em não conformidade.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-164">Number of non compliant users.</span></span>|
|<span data-ttu-id="eb6c6-165">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="eb6c6-165">remediatedUserCount</span></span>|<span data-ttu-id="eb6c6-166">Int32</span><span class="sxs-lookup"><span data-stu-id="eb6c6-166">Int32</span></span>|<span data-ttu-id="eb6c6-167">Número de usuários corrigidos.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-167">Number of remediated users.</span></span>|
|<span data-ttu-id="eb6c6-168">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="eb6c6-168">errorUserCount</span></span>|<span data-ttu-id="eb6c6-169">Int32</span><span class="sxs-lookup"><span data-stu-id="eb6c6-169">Int32</span></span>|<span data-ttu-id="eb6c6-170">Número de usuários com erro.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-170">Number of users had error.</span></span>|
|<span data-ttu-id="eb6c6-171">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="eb6c6-171">unknownUserCount</span></span>|<span data-ttu-id="eb6c6-172">Int32</span><span class="sxs-lookup"><span data-stu-id="eb6c6-172">Int32</span></span>|<span data-ttu-id="eb6c6-173">Número de usuários desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-173">Number of unknown users.</span></span>|
|<span data-ttu-id="eb6c6-174">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="eb6c6-174">conflictUserCount</span></span>|<span data-ttu-id="eb6c6-175">Int32</span><span class="sxs-lookup"><span data-stu-id="eb6c6-175">Int32</span></span>|<span data-ttu-id="eb6c6-176">Número de usuários com conflitos.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-176">Number of conflict users.</span></span>|
|<span data-ttu-id="eb6c6-177">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="eb6c6-177">notApplicableUserCount</span></span>|<span data-ttu-id="eb6c6-178">Int32</span><span class="sxs-lookup"><span data-stu-id="eb6c6-178">Int32</span></span>|<span data-ttu-id="eb6c6-179">Número de usuários não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-179">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="eb6c6-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb6c6-180">Response</span></span>
<span data-ttu-id="eb6c6-181">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-181">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb6c6-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb6c6-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb6c6-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb6c6-183">Request</span></span>
<span data-ttu-id="eb6c6-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eb6c6-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb6c6-185">Response</span></span>
<span data-ttu-id="eb6c6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb6c6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




