---
title: Atualizar deviceConfigurationUserStateSummary
description: Atualiza as propriedades de um objeto deviceConfigurationUserStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aadb068c2511192cc341404a43dc60b957b0210b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731285"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="5c063-103">Atualizar deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="5c063-103">Update deviceConfigurationUserStateSummary</span></span>

<span data-ttu-id="5c063-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c063-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c063-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5c063-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c063-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5c063-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c063-107">Atualiza as propriedades de um objeto [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="5c063-107">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c063-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5c063-108">Prerequisites</span></span>
<span data-ttu-id="5c063-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c063-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c063-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c063-111">Permission type</span></span>|<span data-ttu-id="5c063-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5c063-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c063-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c063-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c063-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c063-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5c063-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c063-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c063-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c063-116">Not supported.</span></span>|
|<span data-ttu-id="5c063-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c063-117">Application</span></span>|<span data-ttu-id="5c063-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c063-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c063-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c063-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="5c063-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c063-120">Request headers</span></span>
|<span data-ttu-id="5c063-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c063-121">Header</span></span>|<span data-ttu-id="5c063-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5c063-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c063-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c063-123">Authorization</span></span>|<span data-ttu-id="5c063-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c063-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c063-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5c063-125">Accept</span></span>|<span data-ttu-id="5c063-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c063-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c063-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c063-127">Request body</span></span>
<span data-ttu-id="5c063-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="5c063-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="5c063-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="5c063-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="5c063-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c063-130">Property</span></span>|<span data-ttu-id="5c063-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c063-131">Type</span></span>|<span data-ttu-id="5c063-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c063-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c063-133">id</span><span class="sxs-lookup"><span data-stu-id="5c063-133">id</span></span>|<span data-ttu-id="5c063-134">String</span><span class="sxs-lookup"><span data-stu-id="5c063-134">String</span></span>|<span data-ttu-id="5c063-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5c063-135">Key of the entity.</span></span>|
|<span data-ttu-id="5c063-136">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="5c063-136">unknownUserCount</span></span>|<span data-ttu-id="5c063-137">Int32</span><span class="sxs-lookup"><span data-stu-id="5c063-137">Int32</span></span>|<span data-ttu-id="5c063-138">Número de usuários desconhecidos</span><span class="sxs-lookup"><span data-stu-id="5c063-138">Number of unknown users</span></span>|
|<span data-ttu-id="5c063-139">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="5c063-139">notApplicableUserCount</span></span>|<span data-ttu-id="5c063-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5c063-140">Int32</span></span>|<span data-ttu-id="5c063-141">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="5c063-141">Number of not applicable users</span></span>|
|<span data-ttu-id="5c063-142">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="5c063-142">compliantUserCount</span></span>|<span data-ttu-id="5c063-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5c063-143">Int32</span></span>|<span data-ttu-id="5c063-144">Número de usuários em conformidade</span><span class="sxs-lookup"><span data-stu-id="5c063-144">Number of compliant users</span></span>|
|<span data-ttu-id="5c063-145">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="5c063-145">remediatedUserCount</span></span>|<span data-ttu-id="5c063-146">Int32</span><span class="sxs-lookup"><span data-stu-id="5c063-146">Int32</span></span>|<span data-ttu-id="5c063-147">Número de usuários corrigidos</span><span class="sxs-lookup"><span data-stu-id="5c063-147">Number of remediated users</span></span>|
|<span data-ttu-id="5c063-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="5c063-148">nonCompliantUserCount</span></span>|<span data-ttu-id="5c063-149">Int32</span><span class="sxs-lookup"><span data-stu-id="5c063-149">Int32</span></span>|<span data-ttu-id="5c063-150">Número de usuários não compatíveis</span><span class="sxs-lookup"><span data-stu-id="5c063-150">Number of NonCompliant users</span></span>|
|<span data-ttu-id="5c063-151">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="5c063-151">errorUserCount</span></span>|<span data-ttu-id="5c063-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5c063-152">Int32</span></span>|<span data-ttu-id="5c063-153">Número de usuários de erro</span><span class="sxs-lookup"><span data-stu-id="5c063-153">Number of error users</span></span>|
|<span data-ttu-id="5c063-154">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="5c063-154">conflictUserCount</span></span>|<span data-ttu-id="5c063-155">Int32</span><span class="sxs-lookup"><span data-stu-id="5c063-155">Int32</span></span>|<span data-ttu-id="5c063-156">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="5c063-156">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="5c063-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c063-157">Response</span></span>
<span data-ttu-id="5c063-158">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c063-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c063-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c063-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c063-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c063-160">Request</span></span>
<span data-ttu-id="5c063-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c063-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5c063-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c063-162">Response</span></span>
<span data-ttu-id="5c063-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c063-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





