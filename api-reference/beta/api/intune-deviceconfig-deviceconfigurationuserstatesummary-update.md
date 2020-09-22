---
title: Atualizar deviceConfigurationUserStateSummary
description: Atualiza as propriedades de um objeto deviceConfigurationUserStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 33adacd5aaaba5d388b15b82ee7eabe717a75f87
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088374"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="d4c59-103">Atualizar deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="d4c59-103">Update deviceConfigurationUserStateSummary</span></span>

<span data-ttu-id="d4c59-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4c59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4c59-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d4c59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4c59-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d4c59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4c59-107">Atualiza as propriedades de um objeto [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d4c59-107">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4c59-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d4c59-108">Prerequisites</span></span>
<span data-ttu-id="d4c59-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4c59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4c59-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4c59-111">Permission type</span></span>|<span data-ttu-id="d4c59-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d4c59-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4c59-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4c59-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4c59-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4c59-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4c59-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4c59-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4c59-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4c59-116">Not supported.</span></span>|
|<span data-ttu-id="d4c59-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4c59-117">Application</span></span>|<span data-ttu-id="d4c59-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4c59-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4c59-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4c59-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="d4c59-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4c59-120">Request headers</span></span>
|<span data-ttu-id="d4c59-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4c59-121">Header</span></span>|<span data-ttu-id="d4c59-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d4c59-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4c59-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4c59-123">Authorization</span></span>|<span data-ttu-id="d4c59-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4c59-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4c59-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d4c59-125">Accept</span></span>|<span data-ttu-id="d4c59-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4c59-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4c59-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4c59-127">Request body</span></span>
<span data-ttu-id="d4c59-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d4c59-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="d4c59-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d4c59-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="d4c59-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4c59-130">Property</span></span>|<span data-ttu-id="d4c59-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4c59-131">Type</span></span>|<span data-ttu-id="d4c59-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4c59-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4c59-133">id</span><span class="sxs-lookup"><span data-stu-id="d4c59-133">id</span></span>|<span data-ttu-id="d4c59-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4c59-134">String</span></span>|<span data-ttu-id="d4c59-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d4c59-135">Key of the entity.</span></span>|
|<span data-ttu-id="d4c59-136">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="d4c59-136">unknownUserCount</span></span>|<span data-ttu-id="d4c59-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d4c59-137">Int32</span></span>|<span data-ttu-id="d4c59-138">Número de usuários desconhecidos</span><span class="sxs-lookup"><span data-stu-id="d4c59-138">Number of unknown users</span></span>|
|<span data-ttu-id="d4c59-139">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="d4c59-139">notApplicableUserCount</span></span>|<span data-ttu-id="d4c59-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d4c59-140">Int32</span></span>|<span data-ttu-id="d4c59-141">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="d4c59-141">Number of not applicable users</span></span>|
|<span data-ttu-id="d4c59-142">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="d4c59-142">compliantUserCount</span></span>|<span data-ttu-id="d4c59-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d4c59-143">Int32</span></span>|<span data-ttu-id="d4c59-144">Número de usuários em conformidade</span><span class="sxs-lookup"><span data-stu-id="d4c59-144">Number of compliant users</span></span>|
|<span data-ttu-id="d4c59-145">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="d4c59-145">remediatedUserCount</span></span>|<span data-ttu-id="d4c59-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d4c59-146">Int32</span></span>|<span data-ttu-id="d4c59-147">Número de usuários corrigidos</span><span class="sxs-lookup"><span data-stu-id="d4c59-147">Number of remediated users</span></span>|
|<span data-ttu-id="d4c59-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="d4c59-148">nonCompliantUserCount</span></span>|<span data-ttu-id="d4c59-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d4c59-149">Int32</span></span>|<span data-ttu-id="d4c59-150">Número de usuários não compatíveis</span><span class="sxs-lookup"><span data-stu-id="d4c59-150">Number of NonCompliant users</span></span>|
|<span data-ttu-id="d4c59-151">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="d4c59-151">errorUserCount</span></span>|<span data-ttu-id="d4c59-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d4c59-152">Int32</span></span>|<span data-ttu-id="d4c59-153">Número de usuários de erro</span><span class="sxs-lookup"><span data-stu-id="d4c59-153">Number of error users</span></span>|
|<span data-ttu-id="d4c59-154">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="d4c59-154">conflictUserCount</span></span>|<span data-ttu-id="d4c59-155">Int32</span><span class="sxs-lookup"><span data-stu-id="d4c59-155">Int32</span></span>|<span data-ttu-id="d4c59-156">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="d4c59-156">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="d4c59-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4c59-157">Response</span></span>
<span data-ttu-id="d4c59-158">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4c59-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4c59-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4c59-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4c59-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4c59-160">Request</span></span>
<span data-ttu-id="d4c59-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4c59-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d4c59-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4c59-162">Response</span></span>
<span data-ttu-id="d4c59-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4c59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






