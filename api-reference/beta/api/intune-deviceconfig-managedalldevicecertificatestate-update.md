---
title: Atualizar managedAllDeviceCertificateState
description: Atualiza as propriedades de um objeto managedAllDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5a54626104faa00e443efe1d430fbd53eb9784dd
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792713"
---
# <a name="update-managedalldevicecertificatestate"></a><span data-ttu-id="9566a-103">Atualizar managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="9566a-103">Update managedAllDeviceCertificateState</span></span>

<span data-ttu-id="9566a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9566a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9566a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9566a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9566a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9566a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9566a-107">Atualiza as propriedades de um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="9566a-107">Update the properties of a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9566a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9566a-108">Prerequisites</span></span>
<span data-ttu-id="9566a-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="9566a-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="9566a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9566a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9566a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9566a-111">Permission type</span></span>|<span data-ttu-id="9566a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9566a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9566a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9566a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9566a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9566a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9566a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9566a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9566a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9566a-116">Not supported.</span></span>|
|<span data-ttu-id="9566a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9566a-117">Application</span></span>|<span data-ttu-id="9566a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9566a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9566a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9566a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="9566a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9566a-120">Request headers</span></span>
|<span data-ttu-id="9566a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9566a-121">Header</span></span>|<span data-ttu-id="9566a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9566a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9566a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9566a-123">Authorization</span></span>|<span data-ttu-id="9566a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9566a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9566a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9566a-125">Accept</span></span>|<span data-ttu-id="9566a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9566a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9566a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9566a-127">Request body</span></span>
<span data-ttu-id="9566a-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="9566a-128">In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

<span data-ttu-id="9566a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="9566a-129">The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span></span>

|<span data-ttu-id="9566a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9566a-130">Property</span></span>|<span data-ttu-id="9566a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9566a-131">Type</span></span>|<span data-ttu-id="9566a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9566a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9566a-133">id</span><span class="sxs-lookup"><span data-stu-id="9566a-133">id</span></span>|<span data-ttu-id="9566a-134">String</span><span class="sxs-lookup"><span data-stu-id="9566a-134">String</span></span>|<span data-ttu-id="9566a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9566a-135">Key of the entity.</span></span>|
|<span data-ttu-id="9566a-136">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="9566a-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="9566a-137">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="9566a-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="9566a-138">Revogar status.</span><span class="sxs-lookup"><span data-stu-id="9566a-138">Revoke status.</span></span> <span data-ttu-id="9566a-139">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="9566a-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="9566a-140">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="9566a-140">managedDeviceDisplayName</span></span>|<span data-ttu-id="9566a-141">String</span><span class="sxs-lookup"><span data-stu-id="9566a-141">String</span></span>|<span data-ttu-id="9566a-142">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="9566a-142">Device display name</span></span>|
|<span data-ttu-id="9566a-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9566a-143">userPrincipalName</span></span>|<span data-ttu-id="9566a-144">String</span><span class="sxs-lookup"><span data-stu-id="9566a-144">String</span></span>|<span data-ttu-id="9566a-145">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="9566a-145">User principal name</span></span>|
|<span data-ttu-id="9566a-146">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9566a-146">certificateExpirationDateTime</span></span>|<span data-ttu-id="9566a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9566a-147">DateTimeOffset</span></span>|<span data-ttu-id="9566a-148">Data de vencimento do certificado</span><span class="sxs-lookup"><span data-stu-id="9566a-148">Certificate expiry date</span></span>|
|<span data-ttu-id="9566a-149">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="9566a-149">certificateIssuerName</span></span>|<span data-ttu-id="9566a-150">String</span><span class="sxs-lookup"><span data-stu-id="9566a-150">String</span></span>|<span data-ttu-id="9566a-151">Emissor</span><span class="sxs-lookup"><span data-stu-id="9566a-151">Issuer</span></span>|
|<span data-ttu-id="9566a-152">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="9566a-152">certificateThumbprint</span></span>|<span data-ttu-id="9566a-153">String</span><span class="sxs-lookup"><span data-stu-id="9566a-153">String</span></span>|<span data-ttu-id="9566a-154">Identificação</span><span class="sxs-lookup"><span data-stu-id="9566a-154">Thumbprint</span></span>|
|<span data-ttu-id="9566a-155">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="9566a-155">certificateSerialNumber</span></span>|<span data-ttu-id="9566a-156">String</span><span class="sxs-lookup"><span data-stu-id="9566a-156">String</span></span>|<span data-ttu-id="9566a-157">Número de série</span><span class="sxs-lookup"><span data-stu-id="9566a-157">Serial number</span></span>|
|<span data-ttu-id="9566a-158">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="9566a-158">certificateSubjectName</span></span>|<span data-ttu-id="9566a-159">String</span><span class="sxs-lookup"><span data-stu-id="9566a-159">String</span></span>|<span data-ttu-id="9566a-160">Nome do assunto do certificado</span><span class="sxs-lookup"><span data-stu-id="9566a-160">Certificate subject name</span></span>|
|<span data-ttu-id="9566a-161">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="9566a-161">certificateKeyUsages</span></span>|<span data-ttu-id="9566a-162">Int32</span><span class="sxs-lookup"><span data-stu-id="9566a-162">Int32</span></span>|<span data-ttu-id="9566a-163">Uso de chave</span><span class="sxs-lookup"><span data-stu-id="9566a-163">Key Usage</span></span>|
|<span data-ttu-id="9566a-164">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="9566a-164">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="9566a-165">String</span><span class="sxs-lookup"><span data-stu-id="9566a-165">String</span></span>|<span data-ttu-id="9566a-166">Uso avançado de chave</span><span class="sxs-lookup"><span data-stu-id="9566a-166">Enhanced Key Usage</span></span>|
|<span data-ttu-id="9566a-167">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="9566a-167">certificateIssuanceDateTime</span></span>|<span data-ttu-id="9566a-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9566a-168">DateTimeOffset</span></span>|<span data-ttu-id="9566a-169">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="9566a-169">Issuance date</span></span>|
|<span data-ttu-id="9566a-170">certificateRevokeStatusLastChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="9566a-170">certificateRevokeStatusLastChangeDateTime</span></span>|<span data-ttu-id="9566a-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9566a-171">DateTimeOffset</span></span>|<span data-ttu-id="9566a-172">A hora em que o status da revogação foi alterado pela última vez</span><span class="sxs-lookup"><span data-stu-id="9566a-172">The time the revoke status was last changed</span></span>|



## <a name="response"></a><span data-ttu-id="9566a-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="9566a-173">Response</span></span>
<span data-ttu-id="9566a-174">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9566a-174">If successful, this method returns a `200 OK` response code and an updated [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9566a-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9566a-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="9566a-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9566a-176">Request</span></span>
<span data-ttu-id="9566a-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9566a-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
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

### <a name="response"></a><span data-ttu-id="9566a-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="9566a-178">Response</span></span>
<span data-ttu-id="9566a-179">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="9566a-179">Here is an example of the response.</span></span> <span data-ttu-id="9566a-180">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="9566a-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9566a-181">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="9566a-181">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



