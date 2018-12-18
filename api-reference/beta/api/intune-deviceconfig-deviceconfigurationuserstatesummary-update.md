---
title: Atualizar deviceConfigurationUserStateSummary
description: Atualize as propriedades de um objeto deviceConfigurationUserStateSummary.
author: tfitzmac
ms.openlocfilehash: a11c4447fee84116b68416ba78f610e8067a6104
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301565"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="9ae5e-103">Atualizar deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="9ae5e-103">Update deviceConfigurationUserStateSummary</span></span>

> <span data-ttu-id="9ae5e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9ae5e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ae5e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9ae5e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ae5e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9ae5e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ae5e-107">Atualize as propriedades de um objeto [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="9ae5e-107">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9ae5e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9ae5e-108">Prerequisites</span></span>
<span data-ttu-id="9ae5e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ae5e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ae5e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ae5e-111">Permission type</span></span>|<span data-ttu-id="9ae5e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9ae5e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ae5e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ae5e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ae5e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ae5e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ae5e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ae5e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ae5e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ae5e-116">Not supported.</span></span>|
|<span data-ttu-id="9ae5e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ae5e-117">Application</span></span>|<span data-ttu-id="9ae5e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ae5e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ae5e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ae5e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="9ae5e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ae5e-120">Request headers</span></span>
|<span data-ttu-id="9ae5e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ae5e-121">Header</span></span>|<span data-ttu-id="9ae5e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9ae5e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ae5e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ae5e-123">Authorization</span></span>|<span data-ttu-id="9ae5e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ae5e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ae5e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9ae5e-125">Accept</span></span>|<span data-ttu-id="9ae5e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ae5e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ae5e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ae5e-127">Request body</span></span>
<span data-ttu-id="9ae5e-128">No corpo da solicitação, fornece uma representação JSON para o objeto [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="9ae5e-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="9ae5e-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="9ae5e-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="9ae5e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ae5e-130">Property</span></span>|<span data-ttu-id="9ae5e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ae5e-131">Type</span></span>|<span data-ttu-id="9ae5e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ae5e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ae5e-133">id</span><span class="sxs-lookup"><span data-stu-id="9ae5e-133">id</span></span>|<span data-ttu-id="9ae5e-134">String</span><span class="sxs-lookup"><span data-stu-id="9ae5e-134">String</span></span>|<span data-ttu-id="9ae5e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9ae5e-135">Key of the entity.</span></span>|
|<span data-ttu-id="9ae5e-136">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="9ae5e-136">unknownUserCount</span></span>|<span data-ttu-id="9ae5e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9ae5e-137">Int32</span></span>|<span data-ttu-id="9ae5e-138">Número de usuários desconhecidos</span><span class="sxs-lookup"><span data-stu-id="9ae5e-138">Number of unknown users</span></span>|
|<span data-ttu-id="9ae5e-139">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="9ae5e-139">notApplicableUserCount</span></span>|<span data-ttu-id="9ae5e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9ae5e-140">Int32</span></span>|<span data-ttu-id="9ae5e-141">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="9ae5e-141">Number of not applicable users</span></span>|
|<span data-ttu-id="9ae5e-142">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="9ae5e-142">compliantUserCount</span></span>|<span data-ttu-id="9ae5e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9ae5e-143">Int32</span></span>|<span data-ttu-id="9ae5e-144">Número de usuários compatíveis</span><span class="sxs-lookup"><span data-stu-id="9ae5e-144">Number of compliant users</span></span>|
|<span data-ttu-id="9ae5e-145">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="9ae5e-145">remediatedUserCount</span></span>|<span data-ttu-id="9ae5e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9ae5e-146">Int32</span></span>|<span data-ttu-id="9ae5e-147">Número de usuários remediados por teste</span><span class="sxs-lookup"><span data-stu-id="9ae5e-147">Number of remediated users</span></span>|
|<span data-ttu-id="9ae5e-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="9ae5e-148">nonCompliantUserCount</span></span>|<span data-ttu-id="9ae5e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9ae5e-149">Int32</span></span>|<span data-ttu-id="9ae5e-150">Número de usuários de fora de conformidade</span><span class="sxs-lookup"><span data-stu-id="9ae5e-150">Number of NonCompliant users</span></span>|
|<span data-ttu-id="9ae5e-151">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="9ae5e-151">errorUserCount</span></span>|<span data-ttu-id="9ae5e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9ae5e-152">Int32</span></span>|<span data-ttu-id="9ae5e-153">Número de usuários de erro</span><span class="sxs-lookup"><span data-stu-id="9ae5e-153">Number of error users</span></span>|
|<span data-ttu-id="9ae5e-154">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="9ae5e-154">conflictUserCount</span></span>|<span data-ttu-id="9ae5e-155">Int32</span><span class="sxs-lookup"><span data-stu-id="9ae5e-155">Int32</span></span>|<span data-ttu-id="9ae5e-156">Número de usuários de conflito</span><span class="sxs-lookup"><span data-stu-id="9ae5e-156">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="9ae5e-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ae5e-157">Response</span></span>
<span data-ttu-id="9ae5e-158">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ae5e-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ae5e-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ae5e-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="9ae5e-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ae5e-160">Request</span></span>
<span data-ttu-id="9ae5e-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ae5e-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationUserStateSummaries
Content-type: application/json
Content-length: 201

{
  "unknownUserCount": 0,
  "notApplicableUserCount": 6,
  "compliantUserCount": 2,
  "remediatedUserCount": 3,
  "nonCompliantUserCount": 5,
  "errorUserCount": 14,
  "conflictUserCount": 1
}
```

### <a name="response"></a><span data-ttu-id="9ae5e-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ae5e-162">Response</span></span>
<span data-ttu-id="9ae5e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ae5e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





