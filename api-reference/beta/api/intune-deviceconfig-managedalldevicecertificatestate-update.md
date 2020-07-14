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
# <a name="update-managedalldevicecertificatestate"></a><span data-ttu-id="ee4de-103">Atualizar managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="ee4de-103">Update managedAllDeviceCertificateState</span></span>

<span data-ttu-id="ee4de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee4de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee4de-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ee4de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee4de-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ee4de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee4de-107">Atualiza as propriedades de um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="ee4de-107">Update the properties of a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee4de-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ee4de-108">Prerequisites</span></span>
<span data-ttu-id="ee4de-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="ee4de-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ee4de-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee4de-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee4de-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee4de-111">Permission type</span></span>|<span data-ttu-id="ee4de-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ee4de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee4de-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee4de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee4de-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee4de-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ee4de-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee4de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee4de-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee4de-116">Not supported.</span></span>|
|<span data-ttu-id="ee4de-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee4de-117">Application</span></span>|<span data-ttu-id="ee4de-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee4de-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee4de-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee4de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="ee4de-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee4de-120">Request headers</span></span>
|<span data-ttu-id="ee4de-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ee4de-121">Header</span></span>|<span data-ttu-id="ee4de-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ee4de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee4de-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee4de-123">Authorization</span></span>|<span data-ttu-id="ee4de-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee4de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee4de-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ee4de-125">Accept</span></span>|<span data-ttu-id="ee4de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee4de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee4de-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee4de-127">Request body</span></span>
<span data-ttu-id="ee4de-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="ee4de-128">In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

<span data-ttu-id="ee4de-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="ee4de-129">The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span></span>

|<span data-ttu-id="ee4de-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee4de-130">Property</span></span>|<span data-ttu-id="ee4de-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee4de-131">Type</span></span>|<span data-ttu-id="ee4de-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee4de-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee4de-133">id</span><span class="sxs-lookup"><span data-stu-id="ee4de-133">id</span></span>|<span data-ttu-id="ee4de-134">String</span><span class="sxs-lookup"><span data-stu-id="ee4de-134">String</span></span>|<span data-ttu-id="ee4de-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ee4de-135">Key of the entity.</span></span>|
|<span data-ttu-id="ee4de-136">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="ee4de-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="ee4de-137">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="ee4de-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="ee4de-138">Revogar status.</span><span class="sxs-lookup"><span data-stu-id="ee4de-138">Revoke status.</span></span> <span data-ttu-id="ee4de-139">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="ee4de-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="ee4de-140">certificateRevokeStatusLastChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="ee4de-140">certificateRevokeStatusLastChangeDateTime</span></span>|<span data-ttu-id="ee4de-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee4de-141">DateTimeOffset</span></span>|<span data-ttu-id="ee4de-142">A hora em que o status da revogação foi alterado pela última vez</span><span class="sxs-lookup"><span data-stu-id="ee4de-142">The time the revoke status was last changed</span></span>|
|<span data-ttu-id="ee4de-143">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ee4de-143">managedDeviceDisplayName</span></span>|<span data-ttu-id="ee4de-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee4de-144">String</span></span>|<span data-ttu-id="ee4de-145">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee4de-145">Device display name</span></span>|
|<span data-ttu-id="ee4de-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ee4de-146">userPrincipalName</span></span>|<span data-ttu-id="ee4de-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee4de-147">String</span></span>|<span data-ttu-id="ee4de-148">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="ee4de-148">User principal name</span></span>|
|<span data-ttu-id="ee4de-149">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ee4de-149">certificateExpirationDateTime</span></span>|<span data-ttu-id="ee4de-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee4de-150">DateTimeOffset</span></span>|<span data-ttu-id="ee4de-151">Data de vencimento do certificado</span><span class="sxs-lookup"><span data-stu-id="ee4de-151">Certificate expiry date</span></span>|
|<span data-ttu-id="ee4de-152">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="ee4de-152">certificateIssuerName</span></span>|<span data-ttu-id="ee4de-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee4de-153">String</span></span>|<span data-ttu-id="ee4de-154">Emissor</span><span class="sxs-lookup"><span data-stu-id="ee4de-154">Issuer</span></span>|
|<span data-ttu-id="ee4de-155">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="ee4de-155">certificateThumbprint</span></span>|<span data-ttu-id="ee4de-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee4de-156">String</span></span>|<span data-ttu-id="ee4de-157">Identificação</span><span class="sxs-lookup"><span data-stu-id="ee4de-157">Thumbprint</span></span>|
|<span data-ttu-id="ee4de-158">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="ee4de-158">certificateSerialNumber</span></span>|<span data-ttu-id="ee4de-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee4de-159">String</span></span>|<span data-ttu-id="ee4de-160">Número de série</span><span class="sxs-lookup"><span data-stu-id="ee4de-160">Serial number</span></span>|
|<span data-ttu-id="ee4de-161">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="ee4de-161">certificateSubjectName</span></span>|<span data-ttu-id="ee4de-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee4de-162">String</span></span>|<span data-ttu-id="ee4de-163">Nome do assunto do certificado</span><span class="sxs-lookup"><span data-stu-id="ee4de-163">Certificate subject name</span></span>|
|<span data-ttu-id="ee4de-164">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="ee4de-164">certificateKeyUsages</span></span>|<span data-ttu-id="ee4de-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ee4de-165">Int32</span></span>|<span data-ttu-id="ee4de-166">Uso de chave</span><span class="sxs-lookup"><span data-stu-id="ee4de-166">Key Usage</span></span>|
|<span data-ttu-id="ee4de-167">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="ee4de-167">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="ee4de-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee4de-168">String</span></span>|<span data-ttu-id="ee4de-169">Uso avançado de chave</span><span class="sxs-lookup"><span data-stu-id="ee4de-169">Enhanced Key Usage</span></span>|
|<span data-ttu-id="ee4de-170">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="ee4de-170">certificateIssuanceDateTime</span></span>|<span data-ttu-id="ee4de-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee4de-171">DateTimeOffset</span></span>|<span data-ttu-id="ee4de-172">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="ee4de-172">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="ee4de-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee4de-173">Response</span></span>
<span data-ttu-id="ee4de-174">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee4de-174">If successful, this method returns a `200 OK` response code and an updated [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee4de-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee4de-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee4de-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee4de-176">Request</span></span>
<span data-ttu-id="ee4de-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee4de-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ee4de-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee4de-178">Response</span></span>
<span data-ttu-id="ee4de-179">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="ee4de-179">Here is an example of the response.</span></span> <span data-ttu-id="ee4de-180">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="ee4de-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ee4de-181">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="ee4de-181">All of the properties will be returned from an actual call.</span></span>
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



