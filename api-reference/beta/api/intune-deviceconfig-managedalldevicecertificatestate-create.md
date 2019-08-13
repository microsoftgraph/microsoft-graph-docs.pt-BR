---
title: Criar managedAllDeviceCertificateState
description: Criar um novo objeto managedAllDeviceCertificateState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 50877255e069c70749ae77b515d7f45a90398a33
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338585"
---
# <a name="create-managedalldevicecertificatestate"></a><span data-ttu-id="ce613-103">Criar managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="ce613-103">Create managedAllDeviceCertificateState</span></span>

> <span data-ttu-id="ce613-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ce613-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce613-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ce613-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce613-106">Criar um novo objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="ce613-106">Create a new [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce613-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ce613-107">Prerequisites</span></span>
<span data-ttu-id="ce613-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce613-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce613-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce613-110">Permission type</span></span>|<span data-ttu-id="ce613-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ce613-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce613-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce613-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ce613-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce613-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ce613-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce613-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce613-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce613-115">Not supported.</span></span>|
|<span data-ttu-id="ce613-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce613-116">Application</span></span>|<span data-ttu-id="ce613-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce613-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce613-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce613-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="ce613-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce613-119">Request headers</span></span>
|<span data-ttu-id="ce613-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ce613-120">Header</span></span>|<span data-ttu-id="ce613-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ce613-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce613-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce613-122">Authorization</span></span>|<span data-ttu-id="ce613-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce613-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce613-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ce613-124">Accept</span></span>|<span data-ttu-id="ce613-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ce613-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce613-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce613-126">Request body</span></span>
<span data-ttu-id="ce613-127">No corpo da solicitação, forneça uma representação JSON do objeto managedAllDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="ce613-127">In the request body, supply a JSON representation for the managedAllDeviceCertificateState object.</span></span>

<span data-ttu-id="ce613-128">A tabela a seguir mostra as propriedades que são necessárias ao criar managedAllDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="ce613-128">The following table shows the properties that are required when you create the managedAllDeviceCertificateState.</span></span>

|<span data-ttu-id="ce613-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce613-129">Property</span></span>|<span data-ttu-id="ce613-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce613-130">Type</span></span>|<span data-ttu-id="ce613-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce613-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce613-132">id</span><span class="sxs-lookup"><span data-stu-id="ce613-132">id</span></span>|<span data-ttu-id="ce613-133">String</span><span class="sxs-lookup"><span data-stu-id="ce613-133">String</span></span>|<span data-ttu-id="ce613-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ce613-134">Key of the entity.</span></span>|
|<span data-ttu-id="ce613-135">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="ce613-135">certificateRevokeStatus</span></span>|[<span data-ttu-id="ce613-136">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="ce613-136">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="ce613-137">Revogar status.</span><span class="sxs-lookup"><span data-stu-id="ce613-137">Revoke status.</span></span> <span data-ttu-id="ce613-138">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="ce613-138">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="ce613-139">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ce613-139">managedDeviceDisplayName</span></span>|<span data-ttu-id="ce613-140">String</span><span class="sxs-lookup"><span data-stu-id="ce613-140">String</span></span>|<span data-ttu-id="ce613-141">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ce613-141">Device display name</span></span>|
|<span data-ttu-id="ce613-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ce613-142">userPrincipalName</span></span>|<span data-ttu-id="ce613-143">String</span><span class="sxs-lookup"><span data-stu-id="ce613-143">String</span></span>|<span data-ttu-id="ce613-144">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="ce613-144">User principal name</span></span>|
|<span data-ttu-id="ce613-145">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ce613-145">certificateExpirationDateTime</span></span>|<span data-ttu-id="ce613-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce613-146">DateTimeOffset</span></span>|<span data-ttu-id="ce613-147">Data de vencimento do certificado</span><span class="sxs-lookup"><span data-stu-id="ce613-147">Certificate expiry date</span></span>|
|<span data-ttu-id="ce613-148">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="ce613-148">certificateIssuerName</span></span>|<span data-ttu-id="ce613-149">String</span><span class="sxs-lookup"><span data-stu-id="ce613-149">String</span></span>|<span data-ttu-id="ce613-150">Emissor</span><span class="sxs-lookup"><span data-stu-id="ce613-150">Issuer</span></span>|
|<span data-ttu-id="ce613-151">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="ce613-151">certificateThumbprint</span></span>|<span data-ttu-id="ce613-152">String</span><span class="sxs-lookup"><span data-stu-id="ce613-152">String</span></span>|<span data-ttu-id="ce613-153">Identificação</span><span class="sxs-lookup"><span data-stu-id="ce613-153">Thumbprint</span></span>|
|<span data-ttu-id="ce613-154">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="ce613-154">certificateSerialNumber</span></span>|<span data-ttu-id="ce613-155">String</span><span class="sxs-lookup"><span data-stu-id="ce613-155">String</span></span>|<span data-ttu-id="ce613-156">Número de série</span><span class="sxs-lookup"><span data-stu-id="ce613-156">Serial number</span></span>|
|<span data-ttu-id="ce613-157">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="ce613-157">certificateSubjectName</span></span>|<span data-ttu-id="ce613-158">String</span><span class="sxs-lookup"><span data-stu-id="ce613-158">String</span></span>|<span data-ttu-id="ce613-159">Nome do assunto do certificado</span><span class="sxs-lookup"><span data-stu-id="ce613-159">Certificate subject name</span></span>|
|<span data-ttu-id="ce613-160">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="ce613-160">certificateKeyUsages</span></span>|<span data-ttu-id="ce613-161">Int32</span><span class="sxs-lookup"><span data-stu-id="ce613-161">Int32</span></span>|<span data-ttu-id="ce613-162">Uso de chave</span><span class="sxs-lookup"><span data-stu-id="ce613-162">Key Usage</span></span>|
|<span data-ttu-id="ce613-163">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="ce613-163">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="ce613-164">String</span><span class="sxs-lookup"><span data-stu-id="ce613-164">String</span></span>|<span data-ttu-id="ce613-165">Uso avançado de chave</span><span class="sxs-lookup"><span data-stu-id="ce613-165">Enhanced Key Usage</span></span>|
|<span data-ttu-id="ce613-166">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="ce613-166">certificateIssuanceDateTime</span></span>|<span data-ttu-id="ce613-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce613-167">DateTimeOffset</span></span>|<span data-ttu-id="ce613-168">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="ce613-168">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="ce613-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce613-169">Response</span></span>
<span data-ttu-id="ce613-170">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce613-170">If successful, this method returns a `201 Created` response code and a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce613-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce613-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce613-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce613-172">Request</span></span>
<span data-ttu-id="ce613-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce613-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ce613-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce613-174">Response</span></span>
<span data-ttu-id="ce613-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce613-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






