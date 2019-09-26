---
title: Criar managedAllDeviceCertificateState
description: Criar um novo objeto managedAllDeviceCertificateState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d11a20463b6421a3975fc516c219fc52b7813cc8
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37183734"
---
# <a name="create-managedalldevicecertificatestate"></a><span data-ttu-id="1442e-103">Criar managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="1442e-103">Create managedAllDeviceCertificateState</span></span>

> <span data-ttu-id="1442e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1442e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1442e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1442e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1442e-106">Criar um novo objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="1442e-106">Create a new [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1442e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1442e-107">Prerequisites</span></span>
<span data-ttu-id="1442e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1442e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1442e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1442e-110">Permission type</span></span>|<span data-ttu-id="1442e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1442e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1442e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1442e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1442e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1442e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1442e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1442e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1442e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1442e-115">Not supported.</span></span>|
|<span data-ttu-id="1442e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1442e-116">Application</span></span>|<span data-ttu-id="1442e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1442e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1442e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1442e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="1442e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1442e-119">Request headers</span></span>
|<span data-ttu-id="1442e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1442e-120">Header</span></span>|<span data-ttu-id="1442e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1442e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1442e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1442e-122">Authorization</span></span>|<span data-ttu-id="1442e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1442e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1442e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1442e-124">Accept</span></span>|<span data-ttu-id="1442e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1442e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1442e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1442e-126">Request body</span></span>
<span data-ttu-id="1442e-127">No corpo da solicitação, forneça uma representação JSON do objeto managedAllDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="1442e-127">In the request body, supply a JSON representation for the managedAllDeviceCertificateState object.</span></span>

<span data-ttu-id="1442e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar managedAllDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="1442e-128">The following table shows the properties that are required when you create the managedAllDeviceCertificateState.</span></span>

|<span data-ttu-id="1442e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1442e-129">Property</span></span>|<span data-ttu-id="1442e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1442e-130">Type</span></span>|<span data-ttu-id="1442e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1442e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1442e-132">id</span><span class="sxs-lookup"><span data-stu-id="1442e-132">id</span></span>|<span data-ttu-id="1442e-133">String</span><span class="sxs-lookup"><span data-stu-id="1442e-133">String</span></span>|<span data-ttu-id="1442e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1442e-134">Key of the entity.</span></span>|
|<span data-ttu-id="1442e-135">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="1442e-135">certificateRevokeStatus</span></span>|[<span data-ttu-id="1442e-136">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="1442e-136">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="1442e-137">Revogar status.</span><span class="sxs-lookup"><span data-stu-id="1442e-137">Revoke status.</span></span> <span data-ttu-id="1442e-138">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="1442e-138">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="1442e-139">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="1442e-139">managedDeviceDisplayName</span></span>|<span data-ttu-id="1442e-140">String</span><span class="sxs-lookup"><span data-stu-id="1442e-140">String</span></span>|<span data-ttu-id="1442e-141">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1442e-141">Device display name</span></span>|
|<span data-ttu-id="1442e-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1442e-142">userPrincipalName</span></span>|<span data-ttu-id="1442e-143">String</span><span class="sxs-lookup"><span data-stu-id="1442e-143">String</span></span>|<span data-ttu-id="1442e-144">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="1442e-144">User principal name</span></span>|
|<span data-ttu-id="1442e-145">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1442e-145">certificateExpirationDateTime</span></span>|<span data-ttu-id="1442e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1442e-146">DateTimeOffset</span></span>|<span data-ttu-id="1442e-147">Data de vencimento do certificado</span><span class="sxs-lookup"><span data-stu-id="1442e-147">Certificate expiry date</span></span>|
|<span data-ttu-id="1442e-148">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="1442e-148">certificateIssuerName</span></span>|<span data-ttu-id="1442e-149">String</span><span class="sxs-lookup"><span data-stu-id="1442e-149">String</span></span>|<span data-ttu-id="1442e-150">Emissor</span><span class="sxs-lookup"><span data-stu-id="1442e-150">Issuer</span></span>|
|<span data-ttu-id="1442e-151">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="1442e-151">certificateThumbprint</span></span>|<span data-ttu-id="1442e-152">String</span><span class="sxs-lookup"><span data-stu-id="1442e-152">String</span></span>|<span data-ttu-id="1442e-153">Identificação</span><span class="sxs-lookup"><span data-stu-id="1442e-153">Thumbprint</span></span>|
|<span data-ttu-id="1442e-154">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="1442e-154">certificateSerialNumber</span></span>|<span data-ttu-id="1442e-155">String</span><span class="sxs-lookup"><span data-stu-id="1442e-155">String</span></span>|<span data-ttu-id="1442e-156">Número de série</span><span class="sxs-lookup"><span data-stu-id="1442e-156">Serial number</span></span>|
|<span data-ttu-id="1442e-157">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="1442e-157">certificateSubjectName</span></span>|<span data-ttu-id="1442e-158">String</span><span class="sxs-lookup"><span data-stu-id="1442e-158">String</span></span>|<span data-ttu-id="1442e-159">Nome do assunto do certificado</span><span class="sxs-lookup"><span data-stu-id="1442e-159">Certificate subject name</span></span>|
|<span data-ttu-id="1442e-160">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="1442e-160">certificateKeyUsages</span></span>|<span data-ttu-id="1442e-161">Int32</span><span class="sxs-lookup"><span data-stu-id="1442e-161">Int32</span></span>|<span data-ttu-id="1442e-162">Uso de chave</span><span class="sxs-lookup"><span data-stu-id="1442e-162">Key Usage</span></span>|
|<span data-ttu-id="1442e-163">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="1442e-163">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="1442e-164">String</span><span class="sxs-lookup"><span data-stu-id="1442e-164">String</span></span>|<span data-ttu-id="1442e-165">Uso avançado de chave</span><span class="sxs-lookup"><span data-stu-id="1442e-165">Enhanced Key Usage</span></span>|
|<span data-ttu-id="1442e-166">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="1442e-166">certificateIssuanceDateTime</span></span>|<span data-ttu-id="1442e-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1442e-167">DateTimeOffset</span></span>|<span data-ttu-id="1442e-168">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="1442e-168">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="1442e-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="1442e-169">Response</span></span>
<span data-ttu-id="1442e-170">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1442e-170">If successful, this method returns a `201 Created` response code and a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1442e-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1442e-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="1442e-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1442e-172">Request</span></span>
<span data-ttu-id="1442e-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1442e-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1442e-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="1442e-174">Response</span></span>
<span data-ttu-id="1442e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1442e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




