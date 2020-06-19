---
title: Criar managedAllDeviceCertificateState
description: Criar um novo objeto managedAllDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 58f061bd89c3633651e40578e23db1f1f4836406
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792734"
---
# <a name="create-managedalldevicecertificatestate"></a><span data-ttu-id="6eaf9-103">Criar managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="6eaf9-103">Create managedAllDeviceCertificateState</span></span>

<span data-ttu-id="6eaf9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6eaf9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6eaf9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6eaf9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6eaf9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6eaf9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6eaf9-107">Criar um novo objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="6eaf9-107">Create a new [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6eaf9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6eaf9-108">Prerequisites</span></span>
<span data-ttu-id="6eaf9-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="6eaf9-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6eaf9-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6eaf9-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6eaf9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6eaf9-111">Permission type</span></span>|<span data-ttu-id="6eaf9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6eaf9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6eaf9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6eaf9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6eaf9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6eaf9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6eaf9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6eaf9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6eaf9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6eaf9-116">Not supported.</span></span>|
|<span data-ttu-id="6eaf9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6eaf9-117">Application</span></span>|<span data-ttu-id="6eaf9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6eaf9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6eaf9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6eaf9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="6eaf9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6eaf9-120">Request headers</span></span>
|<span data-ttu-id="6eaf9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6eaf9-121">Header</span></span>|<span data-ttu-id="6eaf9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6eaf9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6eaf9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6eaf9-123">Authorization</span></span>|<span data-ttu-id="6eaf9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6eaf9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6eaf9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6eaf9-125">Accept</span></span>|<span data-ttu-id="6eaf9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6eaf9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6eaf9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6eaf9-127">Request body</span></span>
<span data-ttu-id="6eaf9-128">No corpo da solicitação, forneça uma representação JSON do objeto managedAllDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="6eaf9-128">In the request body, supply a JSON representation for the managedAllDeviceCertificateState object.</span></span>

<span data-ttu-id="6eaf9-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedAllDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="6eaf9-129">The following table shows the properties that are required when you create the managedAllDeviceCertificateState.</span></span>

|<span data-ttu-id="6eaf9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6eaf9-130">Property</span></span>|<span data-ttu-id="6eaf9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6eaf9-131">Type</span></span>|<span data-ttu-id="6eaf9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6eaf9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6eaf9-133">id</span><span class="sxs-lookup"><span data-stu-id="6eaf9-133">id</span></span>|<span data-ttu-id="6eaf9-134">String</span><span class="sxs-lookup"><span data-stu-id="6eaf9-134">String</span></span>|<span data-ttu-id="6eaf9-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6eaf9-135">Key of the entity.</span></span>|
|<span data-ttu-id="6eaf9-136">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="6eaf9-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="6eaf9-137">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="6eaf9-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="6eaf9-138">Revogar status.</span><span class="sxs-lookup"><span data-stu-id="6eaf9-138">Revoke status.</span></span> <span data-ttu-id="6eaf9-139">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="6eaf9-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="6eaf9-140">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6eaf9-140">managedDeviceDisplayName</span></span>|<span data-ttu-id="6eaf9-141">String</span><span class="sxs-lookup"><span data-stu-id="6eaf9-141">String</span></span>|<span data-ttu-id="6eaf9-142">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6eaf9-142">Device display name</span></span>|
|<span data-ttu-id="6eaf9-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6eaf9-143">userPrincipalName</span></span>|<span data-ttu-id="6eaf9-144">String</span><span class="sxs-lookup"><span data-stu-id="6eaf9-144">String</span></span>|<span data-ttu-id="6eaf9-145">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="6eaf9-145">User principal name</span></span>|
|<span data-ttu-id="6eaf9-146">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6eaf9-146">certificateExpirationDateTime</span></span>|<span data-ttu-id="6eaf9-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6eaf9-147">DateTimeOffset</span></span>|<span data-ttu-id="6eaf9-148">Data de vencimento do certificado</span><span class="sxs-lookup"><span data-stu-id="6eaf9-148">Certificate expiry date</span></span>|
|<span data-ttu-id="6eaf9-149">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="6eaf9-149">certificateIssuerName</span></span>|<span data-ttu-id="6eaf9-150">String</span><span class="sxs-lookup"><span data-stu-id="6eaf9-150">String</span></span>|<span data-ttu-id="6eaf9-151">Emissor</span><span class="sxs-lookup"><span data-stu-id="6eaf9-151">Issuer</span></span>|
|<span data-ttu-id="6eaf9-152">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="6eaf9-152">certificateThumbprint</span></span>|<span data-ttu-id="6eaf9-153">String</span><span class="sxs-lookup"><span data-stu-id="6eaf9-153">String</span></span>|<span data-ttu-id="6eaf9-154">Identificação</span><span class="sxs-lookup"><span data-stu-id="6eaf9-154">Thumbprint</span></span>|
|<span data-ttu-id="6eaf9-155">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="6eaf9-155">certificateSerialNumber</span></span>|<span data-ttu-id="6eaf9-156">String</span><span class="sxs-lookup"><span data-stu-id="6eaf9-156">String</span></span>|<span data-ttu-id="6eaf9-157">Número de série</span><span class="sxs-lookup"><span data-stu-id="6eaf9-157">Serial number</span></span>|
|<span data-ttu-id="6eaf9-158">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="6eaf9-158">certificateSubjectName</span></span>|<span data-ttu-id="6eaf9-159">String</span><span class="sxs-lookup"><span data-stu-id="6eaf9-159">String</span></span>|<span data-ttu-id="6eaf9-160">Nome do assunto do certificado</span><span class="sxs-lookup"><span data-stu-id="6eaf9-160">Certificate subject name</span></span>|
|<span data-ttu-id="6eaf9-161">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="6eaf9-161">certificateKeyUsages</span></span>|<span data-ttu-id="6eaf9-162">Int32</span><span class="sxs-lookup"><span data-stu-id="6eaf9-162">Int32</span></span>|<span data-ttu-id="6eaf9-163">Uso de chave</span><span class="sxs-lookup"><span data-stu-id="6eaf9-163">Key Usage</span></span>|
|<span data-ttu-id="6eaf9-164">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="6eaf9-164">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="6eaf9-165">String</span><span class="sxs-lookup"><span data-stu-id="6eaf9-165">String</span></span>|<span data-ttu-id="6eaf9-166">Uso avançado de chave</span><span class="sxs-lookup"><span data-stu-id="6eaf9-166">Enhanced Key Usage</span></span>|
|<span data-ttu-id="6eaf9-167">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="6eaf9-167">certificateIssuanceDateTime</span></span>|<span data-ttu-id="6eaf9-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6eaf9-168">DateTimeOffset</span></span>|<span data-ttu-id="6eaf9-169">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="6eaf9-169">Issuance date</span></span>|
|<span data-ttu-id="6eaf9-170">certificateRevokeStatusLastChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="6eaf9-170">certificateRevokeStatusLastChangeDateTime</span></span>|<span data-ttu-id="6eaf9-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6eaf9-171">DateTimeOffset</span></span>|<span data-ttu-id="6eaf9-172">A hora em que o status da revogação foi alterado pela última vez</span><span class="sxs-lookup"><span data-stu-id="6eaf9-172">The time the revoke status was last changed</span></span>|



## <a name="response"></a><span data-ttu-id="6eaf9-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="6eaf9-173">Response</span></span>
<span data-ttu-id="6eaf9-174">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6eaf9-174">If successful, this method returns a `201 Created` response code and a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6eaf9-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6eaf9-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="6eaf9-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6eaf9-176">Request</span></span>
<span data-ttu-id="6eaf9-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6eaf9-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
Content-type: application/json
Content-length: 735

{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "certificateRevokeStatus": "pending",
  "managedDeviceDisplayName": "Managed Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
  "certificateIssuerName": "Certificate Issuer Name value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateSubjectName": "Certificate Subject Name value",
  "certificateKeyUsages": 4,
  "certificateExtendedKeyUsages": "Certificate Extended Key Usages value",
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
  "certificateRevokeStatusLastChangeDateTime": "2016-12-31T23:59:41.5044473-08:00"
}
```

### <a name="response"></a><span data-ttu-id="6eaf9-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="6eaf9-178">Response</span></span>
<span data-ttu-id="6eaf9-179">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="6eaf9-179">Here is an example of the response.</span></span> <span data-ttu-id="6eaf9-180">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="6eaf9-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6eaf9-181">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="6eaf9-181">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 784

{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "id": "987c6a17-6a17-987c-176a-7c98176a7c98",
  "certificateRevokeStatus": "pending",
  "managedDeviceDisplayName": "Managed Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
  "certificateIssuerName": "Certificate Issuer Name value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateSubjectName": "Certificate Subject Name value",
  "certificateKeyUsages": 4,
  "certificateExtendedKeyUsages": "Certificate Extended Key Usages value",
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
  "certificateRevokeStatusLastChangeDateTime": "2016-12-31T23:59:41.5044473-08:00"
}
```



