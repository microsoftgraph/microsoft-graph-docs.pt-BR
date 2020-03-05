---
title: Atualizar managedAllDeviceCertificateState
description: Atualiza as propriedades de um objeto managedAllDeviceCertificateState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ae99c18b065e2b40259a84ae869bf0d1d6008f7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448624"
---
# <a name="update-managedalldevicecertificatestate"></a><span data-ttu-id="e79d1-103">Atualizar managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="e79d1-103">Update managedAllDeviceCertificateState</span></span>

<span data-ttu-id="e79d1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e79d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e79d1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e79d1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e79d1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e79d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e79d1-107">Atualiza as propriedades de um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="e79d1-107">Update the properties of a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e79d1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e79d1-108">Prerequisites</span></span>
<span data-ttu-id="e79d1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e79d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e79d1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e79d1-111">Permission type</span></span>|<span data-ttu-id="e79d1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e79d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e79d1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e79d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e79d1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e79d1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e79d1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e79d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e79d1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e79d1-116">Not supported.</span></span>|
|<span data-ttu-id="e79d1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e79d1-117">Application</span></span>|<span data-ttu-id="e79d1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e79d1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e79d1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e79d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="e79d1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e79d1-120">Request headers</span></span>
|<span data-ttu-id="e79d1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e79d1-121">Header</span></span>|<span data-ttu-id="e79d1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e79d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e79d1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e79d1-123">Authorization</span></span>|<span data-ttu-id="e79d1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e79d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e79d1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e79d1-125">Accept</span></span>|<span data-ttu-id="e79d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e79d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e79d1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e79d1-127">Request body</span></span>
<span data-ttu-id="e79d1-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="e79d1-128">In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

<span data-ttu-id="e79d1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="e79d1-129">The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span></span>

|<span data-ttu-id="e79d1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e79d1-130">Property</span></span>|<span data-ttu-id="e79d1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e79d1-131">Type</span></span>|<span data-ttu-id="e79d1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e79d1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e79d1-133">id</span><span class="sxs-lookup"><span data-stu-id="e79d1-133">id</span></span>|<span data-ttu-id="e79d1-134">String</span><span class="sxs-lookup"><span data-stu-id="e79d1-134">String</span></span>|<span data-ttu-id="e79d1-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e79d1-135">Key of the entity.</span></span>|
|<span data-ttu-id="e79d1-136">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="e79d1-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="e79d1-137">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="e79d1-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="e79d1-138">Revogar status.</span><span class="sxs-lookup"><span data-stu-id="e79d1-138">Revoke status.</span></span> <span data-ttu-id="e79d1-139">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="e79d1-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="e79d1-140">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e79d1-140">managedDeviceDisplayName</span></span>|<span data-ttu-id="e79d1-141">String</span><span class="sxs-lookup"><span data-stu-id="e79d1-141">String</span></span>|<span data-ttu-id="e79d1-142">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e79d1-142">Device display name</span></span>|
|<span data-ttu-id="e79d1-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e79d1-143">userPrincipalName</span></span>|<span data-ttu-id="e79d1-144">String</span><span class="sxs-lookup"><span data-stu-id="e79d1-144">String</span></span>|<span data-ttu-id="e79d1-145">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="e79d1-145">User principal name</span></span>|
|<span data-ttu-id="e79d1-146">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e79d1-146">certificateExpirationDateTime</span></span>|<span data-ttu-id="e79d1-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e79d1-147">DateTimeOffset</span></span>|<span data-ttu-id="e79d1-148">Data de vencimento do certificado</span><span class="sxs-lookup"><span data-stu-id="e79d1-148">Certificate expiry date</span></span>|
|<span data-ttu-id="e79d1-149">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="e79d1-149">certificateIssuerName</span></span>|<span data-ttu-id="e79d1-150">String</span><span class="sxs-lookup"><span data-stu-id="e79d1-150">String</span></span>|<span data-ttu-id="e79d1-151">Emissor</span><span class="sxs-lookup"><span data-stu-id="e79d1-151">Issuer</span></span>|
|<span data-ttu-id="e79d1-152">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="e79d1-152">certificateThumbprint</span></span>|<span data-ttu-id="e79d1-153">String</span><span class="sxs-lookup"><span data-stu-id="e79d1-153">String</span></span>|<span data-ttu-id="e79d1-154">Identificação</span><span class="sxs-lookup"><span data-stu-id="e79d1-154">Thumbprint</span></span>|
|<span data-ttu-id="e79d1-155">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="e79d1-155">certificateSerialNumber</span></span>|<span data-ttu-id="e79d1-156">String</span><span class="sxs-lookup"><span data-stu-id="e79d1-156">String</span></span>|<span data-ttu-id="e79d1-157">Número de série</span><span class="sxs-lookup"><span data-stu-id="e79d1-157">Serial number</span></span>|
|<span data-ttu-id="e79d1-158">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="e79d1-158">certificateSubjectName</span></span>|<span data-ttu-id="e79d1-159">String</span><span class="sxs-lookup"><span data-stu-id="e79d1-159">String</span></span>|<span data-ttu-id="e79d1-160">Nome do assunto do certificado</span><span class="sxs-lookup"><span data-stu-id="e79d1-160">Certificate subject name</span></span>|
|<span data-ttu-id="e79d1-161">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="e79d1-161">certificateKeyUsages</span></span>|<span data-ttu-id="e79d1-162">Int32</span><span class="sxs-lookup"><span data-stu-id="e79d1-162">Int32</span></span>|<span data-ttu-id="e79d1-163">Uso de chave</span><span class="sxs-lookup"><span data-stu-id="e79d1-163">Key Usage</span></span>|
|<span data-ttu-id="e79d1-164">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="e79d1-164">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="e79d1-165">String</span><span class="sxs-lookup"><span data-stu-id="e79d1-165">String</span></span>|<span data-ttu-id="e79d1-166">Uso avançado de chave</span><span class="sxs-lookup"><span data-stu-id="e79d1-166">Enhanced Key Usage</span></span>|
|<span data-ttu-id="e79d1-167">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="e79d1-167">certificateIssuanceDateTime</span></span>|<span data-ttu-id="e79d1-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e79d1-168">DateTimeOffset</span></span>|<span data-ttu-id="e79d1-169">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="e79d1-169">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="e79d1-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="e79d1-170">Response</span></span>
<span data-ttu-id="e79d1-171">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e79d1-171">If successful, this method returns a `200 OK` response code and an updated [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e79d1-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e79d1-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="e79d1-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e79d1-173">Request</span></span>
<span data-ttu-id="e79d1-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e79d1-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e79d1-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="e79d1-175">Response</span></span>
<span data-ttu-id="e79d1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e79d1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





