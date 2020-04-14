---
title: Atualizar managedAllDeviceCertificateState
description: Atualiza as propriedades de um objeto managedAllDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d0eb7ec8aaedde3f725c09b3eea9b4e537f3015a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43432132"
---
# <a name="update-managedalldevicecertificatestate"></a><span data-ttu-id="3136b-103">Atualizar managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="3136b-103">Update managedAllDeviceCertificateState</span></span>

<span data-ttu-id="3136b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3136b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3136b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3136b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3136b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3136b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3136b-107">Atualiza as propriedades de um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="3136b-107">Update the properties of a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3136b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3136b-108">Prerequisites</span></span>
<span data-ttu-id="3136b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3136b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3136b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3136b-111">Permission type</span></span>|<span data-ttu-id="3136b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3136b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3136b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3136b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3136b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3136b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3136b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3136b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3136b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3136b-116">Not supported.</span></span>|
|<span data-ttu-id="3136b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3136b-117">Application</span></span>|<span data-ttu-id="3136b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3136b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3136b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3136b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="3136b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3136b-120">Request headers</span></span>
|<span data-ttu-id="3136b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3136b-121">Header</span></span>|<span data-ttu-id="3136b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3136b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3136b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3136b-123">Authorization</span></span>|<span data-ttu-id="3136b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3136b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3136b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3136b-125">Accept</span></span>|<span data-ttu-id="3136b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3136b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3136b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3136b-127">Request body</span></span>
<span data-ttu-id="3136b-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="3136b-128">In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

<span data-ttu-id="3136b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="3136b-129">The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span></span>

|<span data-ttu-id="3136b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3136b-130">Property</span></span>|<span data-ttu-id="3136b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3136b-131">Type</span></span>|<span data-ttu-id="3136b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3136b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3136b-133">id</span><span class="sxs-lookup"><span data-stu-id="3136b-133">id</span></span>|<span data-ttu-id="3136b-134">String</span><span class="sxs-lookup"><span data-stu-id="3136b-134">String</span></span>|<span data-ttu-id="3136b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3136b-135">Key of the entity.</span></span>|
|<span data-ttu-id="3136b-136">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="3136b-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="3136b-137">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="3136b-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="3136b-138">Revogar status.</span><span class="sxs-lookup"><span data-stu-id="3136b-138">Revoke status.</span></span> <span data-ttu-id="3136b-139">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="3136b-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="3136b-140">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="3136b-140">managedDeviceDisplayName</span></span>|<span data-ttu-id="3136b-141">String</span><span class="sxs-lookup"><span data-stu-id="3136b-141">String</span></span>|<span data-ttu-id="3136b-142">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3136b-142">Device display name</span></span>|
|<span data-ttu-id="3136b-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3136b-143">userPrincipalName</span></span>|<span data-ttu-id="3136b-144">String</span><span class="sxs-lookup"><span data-stu-id="3136b-144">String</span></span>|<span data-ttu-id="3136b-145">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="3136b-145">User principal name</span></span>|
|<span data-ttu-id="3136b-146">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3136b-146">certificateExpirationDateTime</span></span>|<span data-ttu-id="3136b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3136b-147">DateTimeOffset</span></span>|<span data-ttu-id="3136b-148">Data de vencimento do certificado</span><span class="sxs-lookup"><span data-stu-id="3136b-148">Certificate expiry date</span></span>|
|<span data-ttu-id="3136b-149">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="3136b-149">certificateIssuerName</span></span>|<span data-ttu-id="3136b-150">String</span><span class="sxs-lookup"><span data-stu-id="3136b-150">String</span></span>|<span data-ttu-id="3136b-151">Emissor</span><span class="sxs-lookup"><span data-stu-id="3136b-151">Issuer</span></span>|
|<span data-ttu-id="3136b-152">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="3136b-152">certificateThumbprint</span></span>|<span data-ttu-id="3136b-153">String</span><span class="sxs-lookup"><span data-stu-id="3136b-153">String</span></span>|<span data-ttu-id="3136b-154">Identificação</span><span class="sxs-lookup"><span data-stu-id="3136b-154">Thumbprint</span></span>|
|<span data-ttu-id="3136b-155">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="3136b-155">certificateSerialNumber</span></span>|<span data-ttu-id="3136b-156">String</span><span class="sxs-lookup"><span data-stu-id="3136b-156">String</span></span>|<span data-ttu-id="3136b-157">Número de série</span><span class="sxs-lookup"><span data-stu-id="3136b-157">Serial number</span></span>|
|<span data-ttu-id="3136b-158">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="3136b-158">certificateSubjectName</span></span>|<span data-ttu-id="3136b-159">String</span><span class="sxs-lookup"><span data-stu-id="3136b-159">String</span></span>|<span data-ttu-id="3136b-160">Nome do assunto do certificado</span><span class="sxs-lookup"><span data-stu-id="3136b-160">Certificate subject name</span></span>|
|<span data-ttu-id="3136b-161">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="3136b-161">certificateKeyUsages</span></span>|<span data-ttu-id="3136b-162">Int32</span><span class="sxs-lookup"><span data-stu-id="3136b-162">Int32</span></span>|<span data-ttu-id="3136b-163">Uso de chave</span><span class="sxs-lookup"><span data-stu-id="3136b-163">Key Usage</span></span>|
|<span data-ttu-id="3136b-164">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="3136b-164">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="3136b-165">String</span><span class="sxs-lookup"><span data-stu-id="3136b-165">String</span></span>|<span data-ttu-id="3136b-166">Uso avançado de chave</span><span class="sxs-lookup"><span data-stu-id="3136b-166">Enhanced Key Usage</span></span>|
|<span data-ttu-id="3136b-167">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="3136b-167">certificateIssuanceDateTime</span></span>|<span data-ttu-id="3136b-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3136b-168">DateTimeOffset</span></span>|<span data-ttu-id="3136b-169">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="3136b-169">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="3136b-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="3136b-170">Response</span></span>
<span data-ttu-id="3136b-171">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3136b-171">If successful, this method returns a `200 OK` response code and an updated [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3136b-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3136b-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="3136b-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3136b-173">Request</span></span>
<span data-ttu-id="3136b-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3136b-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3136b-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="3136b-175">Response</span></span>
<span data-ttu-id="3136b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3136b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



