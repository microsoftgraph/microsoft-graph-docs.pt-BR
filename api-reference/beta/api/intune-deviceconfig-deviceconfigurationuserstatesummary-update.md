---
title: Atualizar deviceConfigurationUserStateSummary
description: Atualiza as propriedades de um objeto deviceConfigurationUserStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dfbaa2cc4b76a1c1e7cb59685c2ee1bd9d3674de
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927269"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="f5ac0-103">Atualizar deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="f5ac0-103">Update deviceConfigurationUserStateSummary</span></span>

> <span data-ttu-id="f5ac0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f5ac0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5ac0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f5ac0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5ac0-106">Atualiza as propriedades de um objeto [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="f5ac0-106">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5ac0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f5ac0-107">Prerequisites</span></span>
<span data-ttu-id="f5ac0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5ac0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5ac0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5ac0-110">Permission type</span></span>|<span data-ttu-id="f5ac0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f5ac0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5ac0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5ac0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f5ac0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5ac0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f5ac0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5ac0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5ac0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5ac0-115">Not supported.</span></span>|
|<span data-ttu-id="f5ac0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5ac0-116">Application</span></span>|<span data-ttu-id="f5ac0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5ac0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5ac0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5ac0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="f5ac0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5ac0-119">Request headers</span></span>
|<span data-ttu-id="f5ac0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5ac0-120">Header</span></span>|<span data-ttu-id="f5ac0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f5ac0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5ac0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5ac0-122">Authorization</span></span>|<span data-ttu-id="f5ac0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5ac0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5ac0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f5ac0-124">Accept</span></span>|<span data-ttu-id="f5ac0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f5ac0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5ac0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5ac0-126">Request body</span></span>
<span data-ttu-id="f5ac0-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="f5ac0-127">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="f5ac0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f5ac0-128">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="f5ac0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5ac0-129">Property</span></span>|<span data-ttu-id="f5ac0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5ac0-130">Type</span></span>|<span data-ttu-id="f5ac0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5ac0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5ac0-132">id</span><span class="sxs-lookup"><span data-stu-id="f5ac0-132">id</span></span>|<span data-ttu-id="f5ac0-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5ac0-133">String</span></span>|<span data-ttu-id="f5ac0-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f5ac0-134">Key of the entity.</span></span>|
|<span data-ttu-id="f5ac0-135">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="f5ac0-135">unknownUserCount</span></span>|<span data-ttu-id="f5ac0-136">Int32</span><span class="sxs-lookup"><span data-stu-id="f5ac0-136">Int32</span></span>|<span data-ttu-id="f5ac0-137">Número de usuários desconhecidos</span><span class="sxs-lookup"><span data-stu-id="f5ac0-137">Number of unknown users</span></span>|
|<span data-ttu-id="f5ac0-138">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="f5ac0-138">notApplicableUserCount</span></span>|<span data-ttu-id="f5ac0-139">Int32</span><span class="sxs-lookup"><span data-stu-id="f5ac0-139">Int32</span></span>|<span data-ttu-id="f5ac0-140">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="f5ac0-140">Number of not applicable users</span></span>|
|<span data-ttu-id="f5ac0-141">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="f5ac0-141">compliantUserCount</span></span>|<span data-ttu-id="f5ac0-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f5ac0-142">Int32</span></span>|<span data-ttu-id="f5ac0-143">Número de usuários em conformidade</span><span class="sxs-lookup"><span data-stu-id="f5ac0-143">Number of compliant users</span></span>|
|<span data-ttu-id="f5ac0-144">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="f5ac0-144">remediatedUserCount</span></span>|<span data-ttu-id="f5ac0-145">Int32</span><span class="sxs-lookup"><span data-stu-id="f5ac0-145">Int32</span></span>|<span data-ttu-id="f5ac0-146">Número de usuários corrigidos</span><span class="sxs-lookup"><span data-stu-id="f5ac0-146">Number of remediated users</span></span>|
|<span data-ttu-id="f5ac0-147">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="f5ac0-147">nonCompliantUserCount</span></span>|<span data-ttu-id="f5ac0-148">Int32</span><span class="sxs-lookup"><span data-stu-id="f5ac0-148">Int32</span></span>|<span data-ttu-id="f5ac0-149">Número de usuários não compatíveis</span><span class="sxs-lookup"><span data-stu-id="f5ac0-149">Number of NonCompliant users</span></span>|
|<span data-ttu-id="f5ac0-150">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="f5ac0-150">errorUserCount</span></span>|<span data-ttu-id="f5ac0-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f5ac0-151">Int32</span></span>|<span data-ttu-id="f5ac0-152">Número de usuários de erro</span><span class="sxs-lookup"><span data-stu-id="f5ac0-152">Number of error users</span></span>|
|<span data-ttu-id="f5ac0-153">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="f5ac0-153">conflictUserCount</span></span>|<span data-ttu-id="f5ac0-154">Int32</span><span class="sxs-lookup"><span data-stu-id="f5ac0-154">Int32</span></span>|<span data-ttu-id="f5ac0-155">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="f5ac0-155">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="f5ac0-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5ac0-156">Response</span></span>
<span data-ttu-id="f5ac0-157">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5ac0-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5ac0-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5ac0-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5ac0-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5ac0-159">Request</span></span>
<span data-ttu-id="f5ac0-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5ac0-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationUserStateSummaries
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "unknownUserCount": 0,
  "notApplicableUserCount": 6,
  "compliantUserCount": 2,
  "remediatedUserCount": 3,
  "nonCompliantUserCount": 5,
  "errorUserCount": 14,
  "conflictUserCount": 1
}
```

### <a name="response"></a><span data-ttu-id="f5ac0-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5ac0-161">Response</span></span>
<span data-ttu-id="f5ac0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5ac0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "id": "e8957887-7887-e895-8778-95e8877895e8",
  "unknownUserCount": 0,
  "notApplicableUserCount": 6,
  "compliantUserCount": 2,
  "remediatedUserCount": 3,
  "nonCompliantUserCount": 5,
  "errorUserCount": 14,
  "conflictUserCount": 1
}
```




