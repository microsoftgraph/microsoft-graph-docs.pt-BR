---
title: Criar managedAllDeviceCertificateState
description: Criar um novo objeto managedAllDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 44c9b00511dc3bd8e4a1c9fb9226e6e62a80dc22
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122970"
---
# <a name="create-managedalldevicecertificatestate"></a><span data-ttu-id="05c55-103">Criar managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="05c55-103">Create managedAllDeviceCertificateState</span></span>

<span data-ttu-id="05c55-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05c55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05c55-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="05c55-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05c55-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="05c55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05c55-107">Criar um novo objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="05c55-107">Create a new [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05c55-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="05c55-108">Prerequisites</span></span>
<span data-ttu-id="05c55-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05c55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05c55-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05c55-111">Permission type</span></span>|<span data-ttu-id="05c55-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="05c55-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05c55-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05c55-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05c55-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05c55-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="05c55-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05c55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05c55-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05c55-116">Not supported.</span></span>|
|<span data-ttu-id="05c55-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05c55-117">Application</span></span>|<span data-ttu-id="05c55-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05c55-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05c55-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05c55-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="05c55-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05c55-120">Request headers</span></span>
|<span data-ttu-id="05c55-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05c55-121">Header</span></span>|<span data-ttu-id="05c55-122">Valor</span><span class="sxs-lookup"><span data-stu-id="05c55-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05c55-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="05c55-123">Authorization</span></span>|<span data-ttu-id="05c55-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05c55-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05c55-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="05c55-125">Accept</span></span>|<span data-ttu-id="05c55-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05c55-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05c55-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05c55-127">Request body</span></span>
<span data-ttu-id="05c55-128">No corpo da solicitação, forneça uma representação JSON do objeto managedAllDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="05c55-128">In the request body, supply a JSON representation for the managedAllDeviceCertificateState object.</span></span>

<span data-ttu-id="05c55-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedAllDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="05c55-129">The following table shows the properties that are required when you create the managedAllDeviceCertificateState.</span></span>

|<span data-ttu-id="05c55-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05c55-130">Property</span></span>|<span data-ttu-id="05c55-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="05c55-131">Type</span></span>|<span data-ttu-id="05c55-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="05c55-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05c55-133">id</span><span class="sxs-lookup"><span data-stu-id="05c55-133">id</span></span>|<span data-ttu-id="05c55-134">String</span><span class="sxs-lookup"><span data-stu-id="05c55-134">String</span></span>|<span data-ttu-id="05c55-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="05c55-135">Key of the entity.</span></span>|
|<span data-ttu-id="05c55-136">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="05c55-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="05c55-137">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="05c55-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="05c55-138">Revogar status.</span><span class="sxs-lookup"><span data-stu-id="05c55-138">Revoke status.</span></span> <span data-ttu-id="05c55-139">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="05c55-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="05c55-140">certificateRevokeStatusLastChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="05c55-140">certificateRevokeStatusLastChangeDateTime</span></span>|<span data-ttu-id="05c55-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05c55-141">DateTimeOffset</span></span>|<span data-ttu-id="05c55-142">A hora em que o status da revogação foi alterado pela última vez</span><span class="sxs-lookup"><span data-stu-id="05c55-142">The time the revoke status was last changed</span></span>|
|<span data-ttu-id="05c55-143">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="05c55-143">managedDeviceDisplayName</span></span>|<span data-ttu-id="05c55-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05c55-144">String</span></span>|<span data-ttu-id="05c55-145">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="05c55-145">Device display name</span></span>|
|<span data-ttu-id="05c55-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="05c55-146">userPrincipalName</span></span>|<span data-ttu-id="05c55-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05c55-147">String</span></span>|<span data-ttu-id="05c55-148">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="05c55-148">User principal name</span></span>|
|<span data-ttu-id="05c55-149">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="05c55-149">certificateExpirationDateTime</span></span>|<span data-ttu-id="05c55-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05c55-150">DateTimeOffset</span></span>|<span data-ttu-id="05c55-151">Data de vencimento do certificado</span><span class="sxs-lookup"><span data-stu-id="05c55-151">Certificate expiry date</span></span>|
|<span data-ttu-id="05c55-152">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="05c55-152">certificateIssuerName</span></span>|<span data-ttu-id="05c55-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05c55-153">String</span></span>|<span data-ttu-id="05c55-154">Emissor</span><span class="sxs-lookup"><span data-stu-id="05c55-154">Issuer</span></span>|
|<span data-ttu-id="05c55-155">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="05c55-155">certificateThumbprint</span></span>|<span data-ttu-id="05c55-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05c55-156">String</span></span>|<span data-ttu-id="05c55-157">Identificação</span><span class="sxs-lookup"><span data-stu-id="05c55-157">Thumbprint</span></span>|
|<span data-ttu-id="05c55-158">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="05c55-158">certificateSerialNumber</span></span>|<span data-ttu-id="05c55-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05c55-159">String</span></span>|<span data-ttu-id="05c55-160">Número de série</span><span class="sxs-lookup"><span data-stu-id="05c55-160">Serial number</span></span>|
|<span data-ttu-id="05c55-161">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="05c55-161">certificateSubjectName</span></span>|<span data-ttu-id="05c55-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05c55-162">String</span></span>|<span data-ttu-id="05c55-163">Nome do assunto do certificado</span><span class="sxs-lookup"><span data-stu-id="05c55-163">Certificate subject name</span></span>|
|<span data-ttu-id="05c55-164">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="05c55-164">certificateKeyUsages</span></span>|<span data-ttu-id="05c55-165">Int32</span><span class="sxs-lookup"><span data-stu-id="05c55-165">Int32</span></span>|<span data-ttu-id="05c55-166">Uso de chave</span><span class="sxs-lookup"><span data-stu-id="05c55-166">Key Usage</span></span>|
|<span data-ttu-id="05c55-167">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="05c55-167">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="05c55-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05c55-168">String</span></span>|<span data-ttu-id="05c55-169">Uso avançado de chave</span><span class="sxs-lookup"><span data-stu-id="05c55-169">Enhanced Key Usage</span></span>|
|<span data-ttu-id="05c55-170">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="05c55-170">certificateIssuanceDateTime</span></span>|<span data-ttu-id="05c55-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05c55-171">DateTimeOffset</span></span>|<span data-ttu-id="05c55-172">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="05c55-172">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="05c55-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="05c55-173">Response</span></span>
<span data-ttu-id="05c55-174">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05c55-174">If successful, this method returns a `201 Created` response code and a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05c55-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05c55-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="05c55-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05c55-176">Request</span></span>
<span data-ttu-id="05c55-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05c55-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
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

### <a name="response"></a><span data-ttu-id="05c55-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="05c55-178">Response</span></span>
<span data-ttu-id="05c55-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05c55-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



