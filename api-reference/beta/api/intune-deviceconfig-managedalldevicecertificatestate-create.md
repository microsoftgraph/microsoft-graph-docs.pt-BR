---
title: Criar managedAllDeviceCertificateState
description: Criar um novo objeto managedAllDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b0924b2b581f758c256072d26531391b51c86453
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43432216"
---
# <a name="create-managedalldevicecertificatestate"></a><span data-ttu-id="78fd4-103">Criar managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="78fd4-103">Create managedAllDeviceCertificateState</span></span>

<span data-ttu-id="78fd4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78fd4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78fd4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="78fd4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78fd4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="78fd4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78fd4-107">Criar um novo objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="78fd4-107">Create a new [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78fd4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="78fd4-108">Prerequisites</span></span>
<span data-ttu-id="78fd4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78fd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78fd4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78fd4-111">Permission type</span></span>|<span data-ttu-id="78fd4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="78fd4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78fd4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78fd4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78fd4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78fd4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="78fd4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78fd4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78fd4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78fd4-116">Not supported.</span></span>|
|<span data-ttu-id="78fd4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78fd4-117">Application</span></span>|<span data-ttu-id="78fd4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78fd4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78fd4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78fd4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="78fd4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78fd4-120">Request headers</span></span>
|<span data-ttu-id="78fd4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="78fd4-121">Header</span></span>|<span data-ttu-id="78fd4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="78fd4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78fd4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="78fd4-123">Authorization</span></span>|<span data-ttu-id="78fd4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78fd4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78fd4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="78fd4-125">Accept</span></span>|<span data-ttu-id="78fd4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78fd4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78fd4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78fd4-127">Request body</span></span>
<span data-ttu-id="78fd4-128">No corpo da solicitação, forneça uma representação JSON do objeto managedAllDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="78fd4-128">In the request body, supply a JSON representation for the managedAllDeviceCertificateState object.</span></span>

<span data-ttu-id="78fd4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedAllDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="78fd4-129">The following table shows the properties that are required when you create the managedAllDeviceCertificateState.</span></span>

|<span data-ttu-id="78fd4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78fd4-130">Property</span></span>|<span data-ttu-id="78fd4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="78fd4-131">Type</span></span>|<span data-ttu-id="78fd4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="78fd4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78fd4-133">id</span><span class="sxs-lookup"><span data-stu-id="78fd4-133">id</span></span>|<span data-ttu-id="78fd4-134">String</span><span class="sxs-lookup"><span data-stu-id="78fd4-134">String</span></span>|<span data-ttu-id="78fd4-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="78fd4-135">Key of the entity.</span></span>|
|<span data-ttu-id="78fd4-136">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="78fd4-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="78fd4-137">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="78fd4-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="78fd4-138">Revogar status.</span><span class="sxs-lookup"><span data-stu-id="78fd4-138">Revoke status.</span></span> <span data-ttu-id="78fd4-139">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="78fd4-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="78fd4-140">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="78fd4-140">managedDeviceDisplayName</span></span>|<span data-ttu-id="78fd4-141">String</span><span class="sxs-lookup"><span data-stu-id="78fd4-141">String</span></span>|<span data-ttu-id="78fd4-142">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="78fd4-142">Device display name</span></span>|
|<span data-ttu-id="78fd4-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="78fd4-143">userPrincipalName</span></span>|<span data-ttu-id="78fd4-144">String</span><span class="sxs-lookup"><span data-stu-id="78fd4-144">String</span></span>|<span data-ttu-id="78fd4-145">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="78fd4-145">User principal name</span></span>|
|<span data-ttu-id="78fd4-146">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="78fd4-146">certificateExpirationDateTime</span></span>|<span data-ttu-id="78fd4-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78fd4-147">DateTimeOffset</span></span>|<span data-ttu-id="78fd4-148">Data de vencimento do certificado</span><span class="sxs-lookup"><span data-stu-id="78fd4-148">Certificate expiry date</span></span>|
|<span data-ttu-id="78fd4-149">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="78fd4-149">certificateIssuerName</span></span>|<span data-ttu-id="78fd4-150">String</span><span class="sxs-lookup"><span data-stu-id="78fd4-150">String</span></span>|<span data-ttu-id="78fd4-151">Emissor</span><span class="sxs-lookup"><span data-stu-id="78fd4-151">Issuer</span></span>|
|<span data-ttu-id="78fd4-152">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="78fd4-152">certificateThumbprint</span></span>|<span data-ttu-id="78fd4-153">String</span><span class="sxs-lookup"><span data-stu-id="78fd4-153">String</span></span>|<span data-ttu-id="78fd4-154">Identificação</span><span class="sxs-lookup"><span data-stu-id="78fd4-154">Thumbprint</span></span>|
|<span data-ttu-id="78fd4-155">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="78fd4-155">certificateSerialNumber</span></span>|<span data-ttu-id="78fd4-156">String</span><span class="sxs-lookup"><span data-stu-id="78fd4-156">String</span></span>|<span data-ttu-id="78fd4-157">Número de série</span><span class="sxs-lookup"><span data-stu-id="78fd4-157">Serial number</span></span>|
|<span data-ttu-id="78fd4-158">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="78fd4-158">certificateSubjectName</span></span>|<span data-ttu-id="78fd4-159">String</span><span class="sxs-lookup"><span data-stu-id="78fd4-159">String</span></span>|<span data-ttu-id="78fd4-160">Nome do assunto do certificado</span><span class="sxs-lookup"><span data-stu-id="78fd4-160">Certificate subject name</span></span>|
|<span data-ttu-id="78fd4-161">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="78fd4-161">certificateKeyUsages</span></span>|<span data-ttu-id="78fd4-162">Int32</span><span class="sxs-lookup"><span data-stu-id="78fd4-162">Int32</span></span>|<span data-ttu-id="78fd4-163">Uso de chave</span><span class="sxs-lookup"><span data-stu-id="78fd4-163">Key Usage</span></span>|
|<span data-ttu-id="78fd4-164">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="78fd4-164">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="78fd4-165">String</span><span class="sxs-lookup"><span data-stu-id="78fd4-165">String</span></span>|<span data-ttu-id="78fd4-166">Uso avançado de chave</span><span class="sxs-lookup"><span data-stu-id="78fd4-166">Enhanced Key Usage</span></span>|
|<span data-ttu-id="78fd4-167">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="78fd4-167">certificateIssuanceDateTime</span></span>|<span data-ttu-id="78fd4-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78fd4-168">DateTimeOffset</span></span>|<span data-ttu-id="78fd4-169">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="78fd4-169">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="78fd4-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="78fd4-170">Response</span></span>
<span data-ttu-id="78fd4-171">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78fd4-171">If successful, this method returns a `201 Created` response code and a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78fd4-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78fd4-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="78fd4-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78fd4-173">Request</span></span>
<span data-ttu-id="78fd4-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78fd4-174">Here is an example of the request.</span></span>
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
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00"
}
```

### <a name="response"></a><span data-ttu-id="78fd4-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="78fd4-175">Response</span></span>
<span data-ttu-id="78fd4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78fd4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00"
}
```



