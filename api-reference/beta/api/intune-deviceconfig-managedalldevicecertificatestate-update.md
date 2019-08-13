---
title: Atualizar managedAllDeviceCertificateState
description: Atualiza as propriedades de um objeto managedAllDeviceCertificateState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 520afd6fb7b2980b8c263dff2f44b52ac2c2f610
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36345614"
---
# <a name="update-managedalldevicecertificatestate"></a><span data-ttu-id="22222-103">Atualizar managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="22222-103">Update managedAllDeviceCertificateState</span></span>

> <span data-ttu-id="22222-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="22222-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22222-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22222-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22222-106">Atualiza as propriedades de um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="22222-106">Update the properties of a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22222-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22222-107">Prerequisites</span></span>
<span data-ttu-id="22222-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22222-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22222-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22222-110">Permission type</span></span>|<span data-ttu-id="22222-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22222-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22222-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22222-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22222-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22222-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="22222-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22222-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22222-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22222-115">Not supported.</span></span>|
|<span data-ttu-id="22222-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22222-116">Application</span></span>|<span data-ttu-id="22222-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22222-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22222-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22222-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="22222-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22222-119">Request headers</span></span>
|<span data-ttu-id="22222-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22222-120">Header</span></span>|<span data-ttu-id="22222-121">Valor</span><span class="sxs-lookup"><span data-stu-id="22222-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22222-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="22222-122">Authorization</span></span>|<span data-ttu-id="22222-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22222-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22222-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22222-124">Accept</span></span>|<span data-ttu-id="22222-125">application/json</span><span class="sxs-lookup"><span data-stu-id="22222-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22222-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22222-126">Request body</span></span>
<span data-ttu-id="22222-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="22222-127">In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

<span data-ttu-id="22222-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="22222-128">The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span></span>

|<span data-ttu-id="22222-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22222-129">Property</span></span>|<span data-ttu-id="22222-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="22222-130">Type</span></span>|<span data-ttu-id="22222-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="22222-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22222-132">id</span><span class="sxs-lookup"><span data-stu-id="22222-132">id</span></span>|<span data-ttu-id="22222-133">String</span><span class="sxs-lookup"><span data-stu-id="22222-133">String</span></span>|<span data-ttu-id="22222-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="22222-134">Key of the entity.</span></span>|
|<span data-ttu-id="22222-135">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="22222-135">certificateRevokeStatus</span></span>|[<span data-ttu-id="22222-136">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="22222-136">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="22222-137">Revogar status.</span><span class="sxs-lookup"><span data-stu-id="22222-137">Revoke status.</span></span> <span data-ttu-id="22222-138">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="22222-138">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="22222-139">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="22222-139">managedDeviceDisplayName</span></span>|<span data-ttu-id="22222-140">String</span><span class="sxs-lookup"><span data-stu-id="22222-140">String</span></span>|<span data-ttu-id="22222-141">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="22222-141">Device display name</span></span>|
|<span data-ttu-id="22222-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="22222-142">userPrincipalName</span></span>|<span data-ttu-id="22222-143">String</span><span class="sxs-lookup"><span data-stu-id="22222-143">String</span></span>|<span data-ttu-id="22222-144">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="22222-144">User principal name</span></span>|
|<span data-ttu-id="22222-145">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="22222-145">certificateExpirationDateTime</span></span>|<span data-ttu-id="22222-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22222-146">DateTimeOffset</span></span>|<span data-ttu-id="22222-147">Data de vencimento do certificado</span><span class="sxs-lookup"><span data-stu-id="22222-147">Certificate expiry date</span></span>|
|<span data-ttu-id="22222-148">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="22222-148">certificateIssuerName</span></span>|<span data-ttu-id="22222-149">String</span><span class="sxs-lookup"><span data-stu-id="22222-149">String</span></span>|<span data-ttu-id="22222-150">Emissor</span><span class="sxs-lookup"><span data-stu-id="22222-150">Issuer</span></span>|
|<span data-ttu-id="22222-151">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="22222-151">certificateThumbprint</span></span>|<span data-ttu-id="22222-152">String</span><span class="sxs-lookup"><span data-stu-id="22222-152">String</span></span>|<span data-ttu-id="22222-153">Identificação</span><span class="sxs-lookup"><span data-stu-id="22222-153">Thumbprint</span></span>|
|<span data-ttu-id="22222-154">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="22222-154">certificateSerialNumber</span></span>|<span data-ttu-id="22222-155">String</span><span class="sxs-lookup"><span data-stu-id="22222-155">String</span></span>|<span data-ttu-id="22222-156">Número de série</span><span class="sxs-lookup"><span data-stu-id="22222-156">Serial number</span></span>|
|<span data-ttu-id="22222-157">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="22222-157">certificateSubjectName</span></span>|<span data-ttu-id="22222-158">String</span><span class="sxs-lookup"><span data-stu-id="22222-158">String</span></span>|<span data-ttu-id="22222-159">Nome do assunto do certificado</span><span class="sxs-lookup"><span data-stu-id="22222-159">Certificate subject name</span></span>|
|<span data-ttu-id="22222-160">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="22222-160">certificateKeyUsages</span></span>|<span data-ttu-id="22222-161">Int32</span><span class="sxs-lookup"><span data-stu-id="22222-161">Int32</span></span>|<span data-ttu-id="22222-162">Uso de chave</span><span class="sxs-lookup"><span data-stu-id="22222-162">Key Usage</span></span>|
|<span data-ttu-id="22222-163">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="22222-163">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="22222-164">String</span><span class="sxs-lookup"><span data-stu-id="22222-164">String</span></span>|<span data-ttu-id="22222-165">Uso avançado de chave</span><span class="sxs-lookup"><span data-stu-id="22222-165">Enhanced Key Usage</span></span>|
|<span data-ttu-id="22222-166">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="22222-166">certificateIssuanceDateTime</span></span>|<span data-ttu-id="22222-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22222-167">DateTimeOffset</span></span>|<span data-ttu-id="22222-168">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="22222-168">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="22222-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="22222-169">Response</span></span>
<span data-ttu-id="22222-170">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22222-170">If successful, this method returns a `200 OK` response code and an updated [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22222-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22222-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="22222-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22222-172">Request</span></span>
<span data-ttu-id="22222-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22222-173">Here is an example of the request.</span></span>
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
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00"
}
```

### <a name="response"></a><span data-ttu-id="22222-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="22222-174">Response</span></span>
<span data-ttu-id="22222-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22222-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00"
}
```






