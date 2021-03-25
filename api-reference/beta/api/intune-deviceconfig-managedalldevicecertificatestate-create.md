---
title: Criar managedAllDeviceCertificateState
description: Crie um novo objeto managedAllDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2f240bde656806928dd03d478acb26c73bcfe8d0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155194"
---
# <a name="create-managedalldevicecertificatestate"></a><span data-ttu-id="642bf-103">Criar managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="642bf-103">Create managedAllDeviceCertificateState</span></span>

<span data-ttu-id="642bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="642bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="642bf-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="642bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="642bf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="642bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="642bf-107">Crie um novo [objeto managedAllDeviceCertificateState.](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)</span><span class="sxs-lookup"><span data-stu-id="642bf-107">Create a new [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="642bf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="642bf-108">Prerequisites</span></span>
<span data-ttu-id="642bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="642bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="642bf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="642bf-111">Permission type</span></span>|<span data-ttu-id="642bf-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="642bf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="642bf-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="642bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="642bf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="642bf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="642bf-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="642bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="642bf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="642bf-116">Not supported.</span></span>|
|<span data-ttu-id="642bf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="642bf-117">Application</span></span>|<span data-ttu-id="642bf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="642bf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="642bf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="642bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="642bf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="642bf-120">Request headers</span></span>
|<span data-ttu-id="642bf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="642bf-121">Header</span></span>|<span data-ttu-id="642bf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="642bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="642bf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="642bf-123">Authorization</span></span>|<span data-ttu-id="642bf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="642bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="642bf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="642bf-125">Accept</span></span>|<span data-ttu-id="642bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="642bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="642bf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="642bf-127">Request body</span></span>
<span data-ttu-id="642bf-128">No corpo da solicitação, fornece uma representação JSON para o objeto managedAllDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="642bf-128">In the request body, supply a JSON representation for the managedAllDeviceCertificateState object.</span></span>

<span data-ttu-id="642bf-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedAllDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="642bf-129">The following table shows the properties that are required when you create the managedAllDeviceCertificateState.</span></span>

|<span data-ttu-id="642bf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="642bf-130">Property</span></span>|<span data-ttu-id="642bf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="642bf-131">Type</span></span>|<span data-ttu-id="642bf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="642bf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="642bf-133">id</span><span class="sxs-lookup"><span data-stu-id="642bf-133">id</span></span>|<span data-ttu-id="642bf-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="642bf-134">String</span></span>|<span data-ttu-id="642bf-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="642bf-135">Key of the entity.</span></span>|
|<span data-ttu-id="642bf-136">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="642bf-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="642bf-137">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="642bf-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="642bf-138">Revogar status.</span><span class="sxs-lookup"><span data-stu-id="642bf-138">Revoke status.</span></span> <span data-ttu-id="642bf-139">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="642bf-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="642bf-140">certificateRevokeStatusLastChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="642bf-140">certificateRevokeStatusLastChangeDateTime</span></span>|<span data-ttu-id="642bf-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="642bf-141">DateTimeOffset</span></span>|<span data-ttu-id="642bf-142">A hora em que o status de revogação foi alterado pela última vez</span><span class="sxs-lookup"><span data-stu-id="642bf-142">The time the revoke status was last changed</span></span>|
|<span data-ttu-id="642bf-143">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="642bf-143">managedDeviceDisplayName</span></span>|<span data-ttu-id="642bf-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="642bf-144">String</span></span>|<span data-ttu-id="642bf-145">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="642bf-145">Device display name</span></span>|
|<span data-ttu-id="642bf-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="642bf-146">userPrincipalName</span></span>|<span data-ttu-id="642bf-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="642bf-147">String</span></span>|<span data-ttu-id="642bf-148">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="642bf-148">User principal name</span></span>|
|<span data-ttu-id="642bf-149">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="642bf-149">certificateExpirationDateTime</span></span>|<span data-ttu-id="642bf-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="642bf-150">DateTimeOffset</span></span>|<span data-ttu-id="642bf-151">Data de expiração do certificado</span><span class="sxs-lookup"><span data-stu-id="642bf-151">Certificate expiry date</span></span>|
|<span data-ttu-id="642bf-152">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="642bf-152">certificateIssuerName</span></span>|<span data-ttu-id="642bf-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="642bf-153">String</span></span>|<span data-ttu-id="642bf-154">Emissor</span><span class="sxs-lookup"><span data-stu-id="642bf-154">Issuer</span></span>|
|<span data-ttu-id="642bf-155">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="642bf-155">certificateThumbprint</span></span>|<span data-ttu-id="642bf-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="642bf-156">String</span></span>|<span data-ttu-id="642bf-157">Impressão Digital</span><span class="sxs-lookup"><span data-stu-id="642bf-157">Thumbprint</span></span>|
|<span data-ttu-id="642bf-158">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="642bf-158">certificateSerialNumber</span></span>|<span data-ttu-id="642bf-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="642bf-159">String</span></span>|<span data-ttu-id="642bf-160">Número de série</span><span class="sxs-lookup"><span data-stu-id="642bf-160">Serial number</span></span>|
|<span data-ttu-id="642bf-161">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="642bf-161">certificateSubjectName</span></span>|<span data-ttu-id="642bf-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="642bf-162">String</span></span>|<span data-ttu-id="642bf-163">Nome do assunto do certificado</span><span class="sxs-lookup"><span data-stu-id="642bf-163">Certificate subject name</span></span>|
|<span data-ttu-id="642bf-164">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="642bf-164">certificateKeyUsages</span></span>|<span data-ttu-id="642bf-165">Int32</span><span class="sxs-lookup"><span data-stu-id="642bf-165">Int32</span></span>|<span data-ttu-id="642bf-166">Uso da Chave</span><span class="sxs-lookup"><span data-stu-id="642bf-166">Key Usage</span></span>|
|<span data-ttu-id="642bf-167">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="642bf-167">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="642bf-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="642bf-168">String</span></span>|<span data-ttu-id="642bf-169">Uso avançado de chave</span><span class="sxs-lookup"><span data-stu-id="642bf-169">Enhanced Key Usage</span></span>|
|<span data-ttu-id="642bf-170">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="642bf-170">certificateIssuanceDateTime</span></span>|<span data-ttu-id="642bf-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="642bf-171">DateTimeOffset</span></span>|<span data-ttu-id="642bf-172">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="642bf-172">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="642bf-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="642bf-173">Response</span></span>
<span data-ttu-id="642bf-174">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="642bf-174">If successful, this method returns a `201 Created` response code and a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="642bf-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="642bf-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="642bf-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="642bf-176">Request</span></span>
<span data-ttu-id="642bf-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="642bf-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="642bf-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="642bf-178">Response</span></span>
<span data-ttu-id="642bf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="642bf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




