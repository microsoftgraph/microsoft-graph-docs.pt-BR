---
title: Atualizar managedAllDeviceCertificateState
description: Atualize as propriedades de um objeto managedAllDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: feb45298263ee3fe4a3d02ec03f729dd7d2d382f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155138"
---
# <a name="update-managedalldevicecertificatestate"></a><span data-ttu-id="07a70-103">Atualizar managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="07a70-103">Update managedAllDeviceCertificateState</span></span>

<span data-ttu-id="07a70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07a70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07a70-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="07a70-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07a70-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07a70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07a70-107">Atualize as propriedades de [um objeto managedAllDeviceCertificateState.](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)</span><span class="sxs-lookup"><span data-stu-id="07a70-107">Update the properties of a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07a70-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="07a70-108">Prerequisites</span></span>
<span data-ttu-id="07a70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07a70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07a70-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07a70-111">Permission type</span></span>|<span data-ttu-id="07a70-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07a70-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07a70-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07a70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07a70-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07a70-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="07a70-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07a70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07a70-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07a70-116">Not supported.</span></span>|
|<span data-ttu-id="07a70-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07a70-117">Application</span></span>|<span data-ttu-id="07a70-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07a70-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07a70-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07a70-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="07a70-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07a70-120">Request headers</span></span>
|<span data-ttu-id="07a70-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07a70-121">Header</span></span>|<span data-ttu-id="07a70-122">Valor</span><span class="sxs-lookup"><span data-stu-id="07a70-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07a70-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="07a70-123">Authorization</span></span>|<span data-ttu-id="07a70-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07a70-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07a70-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="07a70-125">Accept</span></span>|<span data-ttu-id="07a70-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07a70-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07a70-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07a70-127">Request body</span></span>
<span data-ttu-id="07a70-128">No corpo da solicitação, fornece uma representação JSON para [o objeto managedAllDeviceCertificateState.](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)</span><span class="sxs-lookup"><span data-stu-id="07a70-128">In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

<span data-ttu-id="07a70-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="07a70-129">The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span></span>

|<span data-ttu-id="07a70-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07a70-130">Property</span></span>|<span data-ttu-id="07a70-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="07a70-131">Type</span></span>|<span data-ttu-id="07a70-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="07a70-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07a70-133">id</span><span class="sxs-lookup"><span data-stu-id="07a70-133">id</span></span>|<span data-ttu-id="07a70-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07a70-134">String</span></span>|<span data-ttu-id="07a70-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="07a70-135">Key of the entity.</span></span>|
|<span data-ttu-id="07a70-136">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="07a70-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="07a70-137">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="07a70-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="07a70-138">Revogar status.</span><span class="sxs-lookup"><span data-stu-id="07a70-138">Revoke status.</span></span> <span data-ttu-id="07a70-139">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="07a70-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="07a70-140">certificateRevokeStatusLastChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="07a70-140">certificateRevokeStatusLastChangeDateTime</span></span>|<span data-ttu-id="07a70-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07a70-141">DateTimeOffset</span></span>|<span data-ttu-id="07a70-142">A hora em que o status de revogação foi alterado pela última vez</span><span class="sxs-lookup"><span data-stu-id="07a70-142">The time the revoke status was last changed</span></span>|
|<span data-ttu-id="07a70-143">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="07a70-143">managedDeviceDisplayName</span></span>|<span data-ttu-id="07a70-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07a70-144">String</span></span>|<span data-ttu-id="07a70-145">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="07a70-145">Device display name</span></span>|
|<span data-ttu-id="07a70-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="07a70-146">userPrincipalName</span></span>|<span data-ttu-id="07a70-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07a70-147">String</span></span>|<span data-ttu-id="07a70-148">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="07a70-148">User principal name</span></span>|
|<span data-ttu-id="07a70-149">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="07a70-149">certificateExpirationDateTime</span></span>|<span data-ttu-id="07a70-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07a70-150">DateTimeOffset</span></span>|<span data-ttu-id="07a70-151">Data de expiração do certificado</span><span class="sxs-lookup"><span data-stu-id="07a70-151">Certificate expiry date</span></span>|
|<span data-ttu-id="07a70-152">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="07a70-152">certificateIssuerName</span></span>|<span data-ttu-id="07a70-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07a70-153">String</span></span>|<span data-ttu-id="07a70-154">Emissor</span><span class="sxs-lookup"><span data-stu-id="07a70-154">Issuer</span></span>|
|<span data-ttu-id="07a70-155">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="07a70-155">certificateThumbprint</span></span>|<span data-ttu-id="07a70-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07a70-156">String</span></span>|<span data-ttu-id="07a70-157">Impressão Digital</span><span class="sxs-lookup"><span data-stu-id="07a70-157">Thumbprint</span></span>|
|<span data-ttu-id="07a70-158">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="07a70-158">certificateSerialNumber</span></span>|<span data-ttu-id="07a70-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07a70-159">String</span></span>|<span data-ttu-id="07a70-160">Número de série</span><span class="sxs-lookup"><span data-stu-id="07a70-160">Serial number</span></span>|
|<span data-ttu-id="07a70-161">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="07a70-161">certificateSubjectName</span></span>|<span data-ttu-id="07a70-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07a70-162">String</span></span>|<span data-ttu-id="07a70-163">Nome do assunto do certificado</span><span class="sxs-lookup"><span data-stu-id="07a70-163">Certificate subject name</span></span>|
|<span data-ttu-id="07a70-164">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="07a70-164">certificateKeyUsages</span></span>|<span data-ttu-id="07a70-165">Int32</span><span class="sxs-lookup"><span data-stu-id="07a70-165">Int32</span></span>|<span data-ttu-id="07a70-166">Uso da Chave</span><span class="sxs-lookup"><span data-stu-id="07a70-166">Key Usage</span></span>|
|<span data-ttu-id="07a70-167">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="07a70-167">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="07a70-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07a70-168">String</span></span>|<span data-ttu-id="07a70-169">Uso avançado de chave</span><span class="sxs-lookup"><span data-stu-id="07a70-169">Enhanced Key Usage</span></span>|
|<span data-ttu-id="07a70-170">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="07a70-170">certificateIssuanceDateTime</span></span>|<span data-ttu-id="07a70-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07a70-171">DateTimeOffset</span></span>|<span data-ttu-id="07a70-172">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="07a70-172">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="07a70-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="07a70-173">Response</span></span>
<span data-ttu-id="07a70-174">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07a70-174">If successful, this method returns a `200 OK` response code and an updated [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07a70-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07a70-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="07a70-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07a70-176">Request</span></span>
<span data-ttu-id="07a70-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07a70-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="07a70-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="07a70-178">Response</span></span>
<span data-ttu-id="07a70-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07a70-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




