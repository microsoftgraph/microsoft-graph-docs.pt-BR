---
title: Criar deviceComplianceUserStatus
description: Criar um novo objeto deviceComplianceUserStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ab8fa48a1ba35397f7e68c26fa370ce2b064333d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406448"
---
# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="021f1-103">Criar deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="021f1-103">Create deviceComplianceUserStatus</span></span>

> <span data-ttu-id="021f1-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="021f1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="021f1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="021f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="021f1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="021f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="021f1-107">Criar um novo objeto [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="021f1-107">Create a new [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="021f1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="021f1-108">Prerequisites</span></span>
<span data-ttu-id="021f1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="021f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="021f1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="021f1-111">Permission type</span></span>|<span data-ttu-id="021f1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="021f1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="021f1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="021f1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="021f1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="021f1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="021f1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="021f1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="021f1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="021f1-116">Not supported.</span></span>|
|<span data-ttu-id="021f1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="021f1-117">Application</span></span>|<span data-ttu-id="021f1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="021f1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="021f1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="021f1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="021f1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="021f1-120">Request headers</span></span>
|<span data-ttu-id="021f1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="021f1-121">Header</span></span>|<span data-ttu-id="021f1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="021f1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="021f1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="021f1-123">Authorization</span></span>|<span data-ttu-id="021f1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="021f1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="021f1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="021f1-125">Accept</span></span>|<span data-ttu-id="021f1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="021f1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="021f1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="021f1-127">Request body</span></span>
<span data-ttu-id="021f1-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="021f1-128">In the request body, supply a JSON representation for the deviceComplianceUserStatus object.</span></span>

<span data-ttu-id="021f1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="021f1-129">The following table shows the properties that are required when you create the deviceComplianceUserStatus.</span></span>

|<span data-ttu-id="021f1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="021f1-130">Property</span></span>|<span data-ttu-id="021f1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="021f1-131">Type</span></span>|<span data-ttu-id="021f1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="021f1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="021f1-133">id</span><span class="sxs-lookup"><span data-stu-id="021f1-133">id</span></span>|<span data-ttu-id="021f1-134">String</span><span class="sxs-lookup"><span data-stu-id="021f1-134">String</span></span>|<span data-ttu-id="021f1-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="021f1-135">Key of the entity.</span></span>|
|<span data-ttu-id="021f1-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="021f1-136">userDisplayName</span></span>|<span data-ttu-id="021f1-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="021f1-137">String</span></span>|<span data-ttu-id="021f1-138">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="021f1-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="021f1-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="021f1-139">devicesCount</span></span>|<span data-ttu-id="021f1-140">Int32</span><span class="sxs-lookup"><span data-stu-id="021f1-140">Int32</span></span>|<span data-ttu-id="021f1-141">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="021f1-141">Devices count for that user.</span></span>|
|<span data-ttu-id="021f1-142">status</span><span class="sxs-lookup"><span data-stu-id="021f1-142">status</span></span>|[<span data-ttu-id="021f1-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="021f1-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="021f1-144">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="021f1-144">Compliance status of the policy report.</span></span> <span data-ttu-id="021f1-145">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="021f1-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="021f1-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="021f1-146">lastReportedDateTime</span></span>|<span data-ttu-id="021f1-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="021f1-147">DateTimeOffset</span></span>|<span data-ttu-id="021f1-148">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="021f1-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="021f1-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="021f1-149">userPrincipalName</span></span>|<span data-ttu-id="021f1-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="021f1-150">String</span></span>|<span data-ttu-id="021f1-151">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="021f1-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="021f1-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="021f1-152">Response</span></span>
<span data-ttu-id="021f1-153">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="021f1-153">If successful, this method returns a `201 Created` response code and a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="021f1-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="021f1-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="021f1-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="021f1-155">Request</span></span>
<span data-ttu-id="021f1-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="021f1-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
Content-type: application/json
Content-length: 287

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="021f1-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="021f1-157">Response</span></span>
<span data-ttu-id="021f1-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="021f1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 336

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




