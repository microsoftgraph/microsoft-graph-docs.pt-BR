---
title: Atualizar managedAllDeviceCertificateState
description: Atualiza as propriedades de um objeto managedAllDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fcd25b88d46eddadeedf6d53474e209cc70e3c10
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122949"
---
# <a name="update-managedalldevicecertificatestate"></a><span data-ttu-id="9ac6f-103">Atualizar managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="9ac6f-103">Update managedAllDeviceCertificateState</span></span>

<span data-ttu-id="9ac6f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ac6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ac6f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9ac6f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ac6f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ac6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ac6f-107">Atualiza as propriedades de um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="9ac6f-107">Update the properties of a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ac6f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9ac6f-108">Prerequisites</span></span>
<span data-ttu-id="9ac6f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ac6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ac6f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ac6f-111">Permission type</span></span>|<span data-ttu-id="9ac6f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9ac6f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ac6f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ac6f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ac6f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ac6f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ac6f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ac6f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ac6f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ac6f-116">Not supported.</span></span>|
|<span data-ttu-id="9ac6f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ac6f-117">Application</span></span>|<span data-ttu-id="9ac6f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ac6f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ac6f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ac6f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="9ac6f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ac6f-120">Request headers</span></span>
|<span data-ttu-id="9ac6f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ac6f-121">Header</span></span>|<span data-ttu-id="9ac6f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9ac6f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ac6f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ac6f-123">Authorization</span></span>|<span data-ttu-id="9ac6f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ac6f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ac6f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9ac6f-125">Accept</span></span>|<span data-ttu-id="9ac6f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ac6f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ac6f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ac6f-127">Request body</span></span>
<span data-ttu-id="9ac6f-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="9ac6f-128">In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

<span data-ttu-id="9ac6f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="9ac6f-129">The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span></span>

|<span data-ttu-id="9ac6f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ac6f-130">Property</span></span>|<span data-ttu-id="9ac6f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ac6f-131">Type</span></span>|<span data-ttu-id="9ac6f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ac6f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ac6f-133">id</span><span class="sxs-lookup"><span data-stu-id="9ac6f-133">id</span></span>|<span data-ttu-id="9ac6f-134">String</span><span class="sxs-lookup"><span data-stu-id="9ac6f-134">String</span></span>|<span data-ttu-id="9ac6f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9ac6f-135">Key of the entity.</span></span>|
|<span data-ttu-id="9ac6f-136">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="9ac6f-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="9ac6f-137">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="9ac6f-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="9ac6f-138">Revogar status.</span><span class="sxs-lookup"><span data-stu-id="9ac6f-138">Revoke status.</span></span> <span data-ttu-id="9ac6f-139">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="9ac6f-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="9ac6f-140">certificateRevokeStatusLastChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="9ac6f-140">certificateRevokeStatusLastChangeDateTime</span></span>|<span data-ttu-id="9ac6f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ac6f-141">DateTimeOffset</span></span>|<span data-ttu-id="9ac6f-142">A hora em que o status da revogação foi alterado pela última vez</span><span class="sxs-lookup"><span data-stu-id="9ac6f-142">The time the revoke status was last changed</span></span>|
|<span data-ttu-id="9ac6f-143">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="9ac6f-143">managedDeviceDisplayName</span></span>|<span data-ttu-id="9ac6f-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ac6f-144">String</span></span>|<span data-ttu-id="9ac6f-145">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="9ac6f-145">Device display name</span></span>|
|<span data-ttu-id="9ac6f-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9ac6f-146">userPrincipalName</span></span>|<span data-ttu-id="9ac6f-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ac6f-147">String</span></span>|<span data-ttu-id="9ac6f-148">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="9ac6f-148">User principal name</span></span>|
|<span data-ttu-id="9ac6f-149">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9ac6f-149">certificateExpirationDateTime</span></span>|<span data-ttu-id="9ac6f-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ac6f-150">DateTimeOffset</span></span>|<span data-ttu-id="9ac6f-151">Data de vencimento do certificado</span><span class="sxs-lookup"><span data-stu-id="9ac6f-151">Certificate expiry date</span></span>|
|<span data-ttu-id="9ac6f-152">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="9ac6f-152">certificateIssuerName</span></span>|<span data-ttu-id="9ac6f-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ac6f-153">String</span></span>|<span data-ttu-id="9ac6f-154">Emissor</span><span class="sxs-lookup"><span data-stu-id="9ac6f-154">Issuer</span></span>|
|<span data-ttu-id="9ac6f-155">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="9ac6f-155">certificateThumbprint</span></span>|<span data-ttu-id="9ac6f-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ac6f-156">String</span></span>|<span data-ttu-id="9ac6f-157">Identificação</span><span class="sxs-lookup"><span data-stu-id="9ac6f-157">Thumbprint</span></span>|
|<span data-ttu-id="9ac6f-158">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="9ac6f-158">certificateSerialNumber</span></span>|<span data-ttu-id="9ac6f-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ac6f-159">String</span></span>|<span data-ttu-id="9ac6f-160">Número de série</span><span class="sxs-lookup"><span data-stu-id="9ac6f-160">Serial number</span></span>|
|<span data-ttu-id="9ac6f-161">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="9ac6f-161">certificateSubjectName</span></span>|<span data-ttu-id="9ac6f-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ac6f-162">String</span></span>|<span data-ttu-id="9ac6f-163">Nome do assunto do certificado</span><span class="sxs-lookup"><span data-stu-id="9ac6f-163">Certificate subject name</span></span>|
|<span data-ttu-id="9ac6f-164">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="9ac6f-164">certificateKeyUsages</span></span>|<span data-ttu-id="9ac6f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9ac6f-165">Int32</span></span>|<span data-ttu-id="9ac6f-166">Uso de chave</span><span class="sxs-lookup"><span data-stu-id="9ac6f-166">Key Usage</span></span>|
|<span data-ttu-id="9ac6f-167">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="9ac6f-167">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="9ac6f-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ac6f-168">String</span></span>|<span data-ttu-id="9ac6f-169">Uso avançado de chave</span><span class="sxs-lookup"><span data-stu-id="9ac6f-169">Enhanced Key Usage</span></span>|
|<span data-ttu-id="9ac6f-170">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="9ac6f-170">certificateIssuanceDateTime</span></span>|<span data-ttu-id="9ac6f-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ac6f-171">DateTimeOffset</span></span>|<span data-ttu-id="9ac6f-172">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="9ac6f-172">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="9ac6f-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ac6f-173">Response</span></span>
<span data-ttu-id="9ac6f-174">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ac6f-174">If successful, this method returns a `200 OK` response code and an updated [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ac6f-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ac6f-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ac6f-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ac6f-176">Request</span></span>
<span data-ttu-id="9ac6f-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ac6f-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9ac6f-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ac6f-178">Response</span></span>
<span data-ttu-id="9ac6f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ac6f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



