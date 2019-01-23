---
title: Atualizar softwareUpdateStatusSummary
description: Atualizar as propriedades de um objeto softwareUpdateStatusSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0140d0035c05182a22264d36bf3c87db18760a19
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416199"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="27e12-103">Atualizar softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="27e12-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="27e12-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="27e12-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="27e12-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="27e12-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27e12-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="27e12-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27e12-107">Atualizar as propriedades de um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="27e12-107">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27e12-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27e12-108">Prerequisites</span></span>
<span data-ttu-id="27e12-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="27e12-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="27e12-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27e12-111">Permission type</span></span>|<span data-ttu-id="27e12-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="27e12-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27e12-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27e12-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27e12-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27e12-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="27e12-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27e12-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27e12-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27e12-116">Not supported.</span></span>|
|<span data-ttu-id="27e12-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27e12-117">Application</span></span>|<span data-ttu-id="27e12-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27e12-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27e12-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27e12-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="27e12-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27e12-120">Request headers</span></span>
|<span data-ttu-id="27e12-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27e12-121">Header</span></span>|<span data-ttu-id="27e12-122">Valor</span><span class="sxs-lookup"><span data-stu-id="27e12-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27e12-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="27e12-123">Authorization</span></span>|<span data-ttu-id="27e12-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27e12-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27e12-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="27e12-125">Accept</span></span>|<span data-ttu-id="27e12-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27e12-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27e12-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27e12-127">Request body</span></span>
<span data-ttu-id="27e12-128">No corpo da solicitação, forneça uma representação JSON do objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="27e12-128">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="27e12-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="27e12-129">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="27e12-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27e12-130">Property</span></span>|<span data-ttu-id="27e12-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="27e12-131">Type</span></span>|<span data-ttu-id="27e12-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="27e12-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27e12-133">id</span><span class="sxs-lookup"><span data-stu-id="27e12-133">id</span></span>|<span data-ttu-id="27e12-134">String</span><span class="sxs-lookup"><span data-stu-id="27e12-134">String</span></span>|<span data-ttu-id="27e12-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="27e12-135">Key of the entity.</span></span>|
|<span data-ttu-id="27e12-136">displayName</span><span class="sxs-lookup"><span data-stu-id="27e12-136">displayName</span></span>|<span data-ttu-id="27e12-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27e12-137">String</span></span>|<span data-ttu-id="27e12-138">O nome da política.</span><span class="sxs-lookup"><span data-stu-id="27e12-138">The name of the policy.</span></span>|
|<span data-ttu-id="27e12-139">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27e12-139">compliantDeviceCount</span></span>|<span data-ttu-id="27e12-140">Int32</span><span class="sxs-lookup"><span data-stu-id="27e12-140">Int32</span></span>|<span data-ttu-id="27e12-141">Número de dispositivos em conformidade.</span><span class="sxs-lookup"><span data-stu-id="27e12-141">Number of compliant devices.</span></span>|
|<span data-ttu-id="27e12-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27e12-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="27e12-143">Int32</span><span class="sxs-lookup"><span data-stu-id="27e12-143">Int32</span></span>|<span data-ttu-id="27e12-144">Número de dispositivos sem conformidade.</span><span class="sxs-lookup"><span data-stu-id="27e12-144">Number of non compliant devices.</span></span>|
|<span data-ttu-id="27e12-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27e12-145">remediatedDeviceCount</span></span>|<span data-ttu-id="27e12-146">Int32</span><span class="sxs-lookup"><span data-stu-id="27e12-146">Int32</span></span>|<span data-ttu-id="27e12-147">Número de dispositivos corrigidos.</span><span class="sxs-lookup"><span data-stu-id="27e12-147">Number of remediated devices.</span></span>|
|<span data-ttu-id="27e12-148">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27e12-148">errorDeviceCount</span></span>|<span data-ttu-id="27e12-149">Int32</span><span class="sxs-lookup"><span data-stu-id="27e12-149">Int32</span></span>|<span data-ttu-id="27e12-150">Número de dispositivos com erro.</span><span class="sxs-lookup"><span data-stu-id="27e12-150">Number of devices had error.</span></span>|
|<span data-ttu-id="27e12-151">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27e12-151">unknownDeviceCount</span></span>|<span data-ttu-id="27e12-152">Int32</span><span class="sxs-lookup"><span data-stu-id="27e12-152">Int32</span></span>|<span data-ttu-id="27e12-153">Número de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="27e12-153">Number of unknown devices.</span></span>|
|<span data-ttu-id="27e12-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27e12-154">conflictDeviceCount</span></span>|<span data-ttu-id="27e12-155">Int32</span><span class="sxs-lookup"><span data-stu-id="27e12-155">Int32</span></span>|<span data-ttu-id="27e12-156">Número de dispositivos em conflito.</span><span class="sxs-lookup"><span data-stu-id="27e12-156">Number of conflict devices.</span></span>|
|<span data-ttu-id="27e12-157">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27e12-157">notApplicableDeviceCount</span></span>|<span data-ttu-id="27e12-158">Int32</span><span class="sxs-lookup"><span data-stu-id="27e12-158">Int32</span></span>|<span data-ttu-id="27e12-159">Número de dispositivos não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="27e12-159">Number of not applicable devices.</span></span>|
|<span data-ttu-id="27e12-160">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="27e12-160">compliantUserCount</span></span>|<span data-ttu-id="27e12-161">Int32</span><span class="sxs-lookup"><span data-stu-id="27e12-161">Int32</span></span>|<span data-ttu-id="27e12-162">Número de usuários em conformidade.</span><span class="sxs-lookup"><span data-stu-id="27e12-162">Number of compliant users.</span></span>|
|<span data-ttu-id="27e12-163">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="27e12-163">nonCompliantUserCount</span></span>|<span data-ttu-id="27e12-164">Int32</span><span class="sxs-lookup"><span data-stu-id="27e12-164">Int32</span></span>|<span data-ttu-id="27e12-165">Número de usuários em não conformidade.</span><span class="sxs-lookup"><span data-stu-id="27e12-165">Number of non compliant users.</span></span>|
|<span data-ttu-id="27e12-166">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="27e12-166">remediatedUserCount</span></span>|<span data-ttu-id="27e12-167">Int32</span><span class="sxs-lookup"><span data-stu-id="27e12-167">Int32</span></span>|<span data-ttu-id="27e12-168">Número de usuários corrigidos.</span><span class="sxs-lookup"><span data-stu-id="27e12-168">Number of remediated users.</span></span>|
|<span data-ttu-id="27e12-169">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="27e12-169">errorUserCount</span></span>|<span data-ttu-id="27e12-170">Int32</span><span class="sxs-lookup"><span data-stu-id="27e12-170">Int32</span></span>|<span data-ttu-id="27e12-171">Número de usuários com erro.</span><span class="sxs-lookup"><span data-stu-id="27e12-171">Number of users had error.</span></span>|
|<span data-ttu-id="27e12-172">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="27e12-172">unknownUserCount</span></span>|<span data-ttu-id="27e12-173">Int32</span><span class="sxs-lookup"><span data-stu-id="27e12-173">Int32</span></span>|<span data-ttu-id="27e12-174">Número de usuários desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="27e12-174">Number of unknown users.</span></span>|
|<span data-ttu-id="27e12-175">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="27e12-175">conflictUserCount</span></span>|<span data-ttu-id="27e12-176">Int32</span><span class="sxs-lookup"><span data-stu-id="27e12-176">Int32</span></span>|<span data-ttu-id="27e12-177">Número de usuários com conflitos.</span><span class="sxs-lookup"><span data-stu-id="27e12-177">Number of conflict users.</span></span>|
|<span data-ttu-id="27e12-178">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="27e12-178">notApplicableUserCount</span></span>|<span data-ttu-id="27e12-179">Int32</span><span class="sxs-lookup"><span data-stu-id="27e12-179">Int32</span></span>|<span data-ttu-id="27e12-180">Número de usuários não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="27e12-180">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="27e12-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="27e12-181">Response</span></span>
<span data-ttu-id="27e12-182">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27e12-182">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27e12-183">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27e12-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="27e12-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27e12-184">Request</span></span>
<span data-ttu-id="27e12-185">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27e12-185">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="27e12-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="27e12-186">Response</span></span>
<span data-ttu-id="27e12-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27e12-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




