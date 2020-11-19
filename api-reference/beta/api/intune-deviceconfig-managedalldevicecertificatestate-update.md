---
title: Atualizar managedAllDeviceCertificateState
description: Atualiza as propriedades de um objeto managedAllDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fa71986feba2a6c90094eec48624568a051f3136
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49225891"
---
# <a name="update-managedalldevicecertificatestate"></a><span data-ttu-id="426cc-103">Atualizar managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="426cc-103">Update managedAllDeviceCertificateState</span></span>

<span data-ttu-id="426cc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="426cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="426cc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="426cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="426cc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="426cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="426cc-107">Atualiza as propriedades de um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="426cc-107">Update the properties of a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="426cc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="426cc-108">Prerequisites</span></span>
<span data-ttu-id="426cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="426cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="426cc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="426cc-111">Permission type</span></span>|<span data-ttu-id="426cc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="426cc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="426cc-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="426cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="426cc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="426cc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="426cc-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="426cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="426cc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="426cc-116">Not supported.</span></span>|
|<span data-ttu-id="426cc-117">Application</span><span class="sxs-lookup"><span data-stu-id="426cc-117">Application</span></span>|<span data-ttu-id="426cc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="426cc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="426cc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="426cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="426cc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="426cc-120">Request headers</span></span>
|<span data-ttu-id="426cc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="426cc-121">Header</span></span>|<span data-ttu-id="426cc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="426cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="426cc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="426cc-123">Authorization</span></span>|<span data-ttu-id="426cc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="426cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="426cc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="426cc-125">Accept</span></span>|<span data-ttu-id="426cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="426cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="426cc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="426cc-127">Request body</span></span>
<span data-ttu-id="426cc-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="426cc-128">In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

<span data-ttu-id="426cc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="426cc-129">The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span></span>

|<span data-ttu-id="426cc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="426cc-130">Property</span></span>|<span data-ttu-id="426cc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="426cc-131">Type</span></span>|<span data-ttu-id="426cc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="426cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="426cc-133">id</span><span class="sxs-lookup"><span data-stu-id="426cc-133">id</span></span>|<span data-ttu-id="426cc-134">String</span><span class="sxs-lookup"><span data-stu-id="426cc-134">String</span></span>|<span data-ttu-id="426cc-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="426cc-135">Key of the entity.</span></span>|
|<span data-ttu-id="426cc-136">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="426cc-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="426cc-137">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="426cc-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="426cc-138">Revogar status.</span><span class="sxs-lookup"><span data-stu-id="426cc-138">Revoke status.</span></span> <span data-ttu-id="426cc-139">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="426cc-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="426cc-140">certificateRevokeStatusLastChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="426cc-140">certificateRevokeStatusLastChangeDateTime</span></span>|<span data-ttu-id="426cc-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="426cc-141">DateTimeOffset</span></span>|<span data-ttu-id="426cc-142">A hora em que o status da revogação foi alterado pela última vez</span><span class="sxs-lookup"><span data-stu-id="426cc-142">The time the revoke status was last changed</span></span>|
|<span data-ttu-id="426cc-143">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="426cc-143">managedDeviceDisplayName</span></span>|<span data-ttu-id="426cc-144">String</span><span class="sxs-lookup"><span data-stu-id="426cc-144">String</span></span>|<span data-ttu-id="426cc-145">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="426cc-145">Device display name</span></span>|
|<span data-ttu-id="426cc-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="426cc-146">userPrincipalName</span></span>|<span data-ttu-id="426cc-147">String</span><span class="sxs-lookup"><span data-stu-id="426cc-147">String</span></span>|<span data-ttu-id="426cc-148">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="426cc-148">User principal name</span></span>|
|<span data-ttu-id="426cc-149">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="426cc-149">certificateExpirationDateTime</span></span>|<span data-ttu-id="426cc-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="426cc-150">DateTimeOffset</span></span>|<span data-ttu-id="426cc-151">Data de vencimento do certificado</span><span class="sxs-lookup"><span data-stu-id="426cc-151">Certificate expiry date</span></span>|
|<span data-ttu-id="426cc-152">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="426cc-152">certificateIssuerName</span></span>|<span data-ttu-id="426cc-153">String</span><span class="sxs-lookup"><span data-stu-id="426cc-153">String</span></span>|<span data-ttu-id="426cc-154">Emissor</span><span class="sxs-lookup"><span data-stu-id="426cc-154">Issuer</span></span>|
|<span data-ttu-id="426cc-155">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="426cc-155">certificateThumbprint</span></span>|<span data-ttu-id="426cc-156">String</span><span class="sxs-lookup"><span data-stu-id="426cc-156">String</span></span>|<span data-ttu-id="426cc-157">Impressão Digital</span><span class="sxs-lookup"><span data-stu-id="426cc-157">Thumbprint</span></span>|
|<span data-ttu-id="426cc-158">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="426cc-158">certificateSerialNumber</span></span>|<span data-ttu-id="426cc-159">String</span><span class="sxs-lookup"><span data-stu-id="426cc-159">String</span></span>|<span data-ttu-id="426cc-160">Número de série</span><span class="sxs-lookup"><span data-stu-id="426cc-160">Serial number</span></span>|
|<span data-ttu-id="426cc-161">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="426cc-161">certificateSubjectName</span></span>|<span data-ttu-id="426cc-162">String</span><span class="sxs-lookup"><span data-stu-id="426cc-162">String</span></span>|<span data-ttu-id="426cc-163">Nome do assunto do certificado</span><span class="sxs-lookup"><span data-stu-id="426cc-163">Certificate subject name</span></span>|
|<span data-ttu-id="426cc-164">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="426cc-164">certificateKeyUsages</span></span>|<span data-ttu-id="426cc-165">Int32</span><span class="sxs-lookup"><span data-stu-id="426cc-165">Int32</span></span>|<span data-ttu-id="426cc-166">Uso de chave</span><span class="sxs-lookup"><span data-stu-id="426cc-166">Key Usage</span></span>|
|<span data-ttu-id="426cc-167">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="426cc-167">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="426cc-168">String</span><span class="sxs-lookup"><span data-stu-id="426cc-168">String</span></span>|<span data-ttu-id="426cc-169">Uso avançado de chave</span><span class="sxs-lookup"><span data-stu-id="426cc-169">Enhanced Key Usage</span></span>|
|<span data-ttu-id="426cc-170">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="426cc-170">certificateIssuanceDateTime</span></span>|<span data-ttu-id="426cc-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="426cc-171">DateTimeOffset</span></span>|<span data-ttu-id="426cc-172">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="426cc-172">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="426cc-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="426cc-173">Response</span></span>
<span data-ttu-id="426cc-174">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="426cc-174">If successful, this method returns a `200 OK` response code and an updated [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="426cc-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="426cc-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="426cc-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="426cc-176">Request</span></span>
<span data-ttu-id="426cc-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="426cc-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
Content-type: application/json
Content-length: 820

{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "certificateRevokeStatus": "pending",
  "certificateRevokeStatusLastChangeDateTime": "2016-12-31T23:59:34.9547208-08:00",
  "managedDeviceDisplayName": "Managed Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
  "certificateIssuerName": "Certificate Issuer Name value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateSubjectName": "Certificate Subject Name value",
  "certificateKeyUsages": 4,
  "certificateExtendedKeyUsages": "Certificate Extended Key Usages value",
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00"
}
```

### <a name="response"></a><span data-ttu-id="426cc-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="426cc-178">Response</span></span>
<span data-ttu-id="426cc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="426cc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 869

{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "id": "987c6a17-6a17-987c-176a-7c98176a7c98",
  "certificateRevokeStatus": "pending",
  "certificateRevokeStatusLastChangeDateTime": "2016-12-31T23:59:34.9547208-08:00",
  "managedDeviceDisplayName": "Managed Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
  "certificateIssuerName": "Certificate Issuer Name value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateSubjectName": "Certificate Subject Name value",
  "certificateKeyUsages": 4,
  "certificateExtendedKeyUsages": "Certificate Extended Key Usages value",
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00"
}
```




