---
title: Criar managedAllDeviceCertificateState
description: Criar um novo objeto managedAllDeviceCertificateState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 024aaee657dbb8bd67491e793ceb99f82ca6d0fd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725816"
---
# <a name="create-managedalldevicecertificatestate"></a><span data-ttu-id="6e045-103">Criar managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="6e045-103">Create managedAllDeviceCertificateState</span></span>

> <span data-ttu-id="6e045-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6e045-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e045-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6e045-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e045-106">Criar um novo objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="6e045-106">Create a new [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e045-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6e045-107">Prerequisites</span></span>
<span data-ttu-id="6e045-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e045-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e045-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e045-110">Permission type</span></span>|<span data-ttu-id="6e045-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6e045-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e045-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e045-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6e045-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e045-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e045-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e045-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e045-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e045-115">Not supported.</span></span>|
|<span data-ttu-id="6e045-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e045-116">Application</span></span>|<span data-ttu-id="6e045-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e045-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e045-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e045-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="6e045-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e045-119">Request headers</span></span>
|<span data-ttu-id="6e045-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e045-120">Header</span></span>|<span data-ttu-id="6e045-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6e045-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e045-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e045-122">Authorization</span></span>|<span data-ttu-id="6e045-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e045-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e045-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6e045-124">Accept</span></span>|<span data-ttu-id="6e045-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6e045-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e045-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e045-126">Request body</span></span>
<span data-ttu-id="6e045-127">No corpo da solicitação, forneça uma representação JSON do objeto managedAllDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="6e045-127">In the request body, supply a JSON representation for the managedAllDeviceCertificateState object.</span></span>

<span data-ttu-id="6e045-128">A tabela a seguir mostra as propriedades que são necessárias ao criar managedAllDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="6e045-128">The following table shows the properties that are required when you create the managedAllDeviceCertificateState.</span></span>

|<span data-ttu-id="6e045-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e045-129">Property</span></span>|<span data-ttu-id="6e045-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e045-130">Type</span></span>|<span data-ttu-id="6e045-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e045-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e045-132">id</span><span class="sxs-lookup"><span data-stu-id="6e045-132">id</span></span>|<span data-ttu-id="6e045-133">String</span><span class="sxs-lookup"><span data-stu-id="6e045-133">String</span></span>|<span data-ttu-id="6e045-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6e045-134">Key of the entity.</span></span>|
|<span data-ttu-id="6e045-135">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="6e045-135">certificateRevokeStatus</span></span>|[<span data-ttu-id="6e045-136">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="6e045-136">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="6e045-137">Revogar status.</span><span class="sxs-lookup"><span data-stu-id="6e045-137">Revoke status.</span></span> <span data-ttu-id="6e045-138">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="6e045-138">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="6e045-139">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6e045-139">managedDeviceDisplayName</span></span>|<span data-ttu-id="6e045-140">String</span><span class="sxs-lookup"><span data-stu-id="6e045-140">String</span></span>|<span data-ttu-id="6e045-141">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6e045-141">Device display name</span></span>|
|<span data-ttu-id="6e045-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6e045-142">userPrincipalName</span></span>|<span data-ttu-id="6e045-143">String</span><span class="sxs-lookup"><span data-stu-id="6e045-143">String</span></span>|<span data-ttu-id="6e045-144">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="6e045-144">User principal name</span></span>|
|<span data-ttu-id="6e045-145">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6e045-145">certificateExpirationDateTime</span></span>|<span data-ttu-id="6e045-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e045-146">DateTimeOffset</span></span>|<span data-ttu-id="6e045-147">Data de vencimento do certificado</span><span class="sxs-lookup"><span data-stu-id="6e045-147">Certificate expiry date</span></span>|
|<span data-ttu-id="6e045-148">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="6e045-148">certificateIssuerName</span></span>|<span data-ttu-id="6e045-149">String</span><span class="sxs-lookup"><span data-stu-id="6e045-149">String</span></span>|<span data-ttu-id="6e045-150">Emissor</span><span class="sxs-lookup"><span data-stu-id="6e045-150">Issuer</span></span>|
|<span data-ttu-id="6e045-151">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="6e045-151">certificateThumbprint</span></span>|<span data-ttu-id="6e045-152">String</span><span class="sxs-lookup"><span data-stu-id="6e045-152">String</span></span>|<span data-ttu-id="6e045-153">Identificação</span><span class="sxs-lookup"><span data-stu-id="6e045-153">Thumbprint</span></span>|
|<span data-ttu-id="6e045-154">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="6e045-154">certificateSerialNumber</span></span>|<span data-ttu-id="6e045-155">String</span><span class="sxs-lookup"><span data-stu-id="6e045-155">String</span></span>|<span data-ttu-id="6e045-156">Número de série</span><span class="sxs-lookup"><span data-stu-id="6e045-156">Serial number</span></span>|
|<span data-ttu-id="6e045-157">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="6e045-157">certificateSubjectName</span></span>|<span data-ttu-id="6e045-158">String</span><span class="sxs-lookup"><span data-stu-id="6e045-158">String</span></span>|<span data-ttu-id="6e045-159">Nome do assunto do certificado</span><span class="sxs-lookup"><span data-stu-id="6e045-159">Certificate subject name</span></span>|
|<span data-ttu-id="6e045-160">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="6e045-160">certificateKeyUsages</span></span>|<span data-ttu-id="6e045-161">Int32</span><span class="sxs-lookup"><span data-stu-id="6e045-161">Int32</span></span>|<span data-ttu-id="6e045-162">Uso de chave</span><span class="sxs-lookup"><span data-stu-id="6e045-162">Key Usage</span></span>|
|<span data-ttu-id="6e045-163">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="6e045-163">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="6e045-164">String</span><span class="sxs-lookup"><span data-stu-id="6e045-164">String</span></span>|<span data-ttu-id="6e045-165">Uso avançado de chave</span><span class="sxs-lookup"><span data-stu-id="6e045-165">Enhanced Key Usage</span></span>|
|<span data-ttu-id="6e045-166">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="6e045-166">certificateIssuanceDateTime</span></span>|<span data-ttu-id="6e045-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e045-167">DateTimeOffset</span></span>|<span data-ttu-id="6e045-168">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="6e045-168">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="6e045-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e045-169">Response</span></span>
<span data-ttu-id="6e045-170">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e045-170">If successful, this method returns a `201 Created` response code and a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e045-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e045-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e045-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e045-172">Request</span></span>
<span data-ttu-id="6e045-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e045-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6e045-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e045-174">Response</span></span>
<span data-ttu-id="6e045-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e045-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





