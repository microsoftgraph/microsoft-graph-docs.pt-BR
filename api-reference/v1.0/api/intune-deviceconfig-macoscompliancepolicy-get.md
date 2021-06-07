---
title: Get macOSCompliancePolicy
description: Ler propriedades e relações do objeto macOSCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cb9b9a9553ecc703d31fbd2bdf86e622988e2b54
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52747876"
---
# <a name="get-macoscompliancepolicy"></a><span data-ttu-id="5ac44-103">Get macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5ac44-103">Get macOSCompliancePolicy</span></span>

<span data-ttu-id="5ac44-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ac44-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ac44-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ac44-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ac44-106">Ler propriedades e relações do objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5ac44-106">Read properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ac44-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ac44-107">Prerequisites</span></span>
<span data-ttu-id="5ac44-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ac44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ac44-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ac44-110">Permission type</span></span>|<span data-ttu-id="5ac44-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ac44-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ac44-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ac44-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5ac44-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ac44-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5ac44-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ac44-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ac44-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ac44-115">Not supported.</span></span>|
|<span data-ttu-id="5ac44-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ac44-116">Application</span></span>|<span data-ttu-id="5ac44-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ac44-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ac44-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ac44-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ac44-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5ac44-119">Optional query parameters</span></span>
<span data-ttu-id="5ac44-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5ac44-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ac44-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ac44-121">Request headers</span></span>
|<span data-ttu-id="5ac44-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ac44-122">Header</span></span>|<span data-ttu-id="5ac44-123">Valor</span><span class="sxs-lookup"><span data-stu-id="5ac44-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ac44-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ac44-124">Authorization</span></span>|<span data-ttu-id="5ac44-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ac44-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ac44-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ac44-126">Accept</span></span>|<span data-ttu-id="5ac44-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5ac44-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ac44-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ac44-128">Request body</span></span>
<span data-ttu-id="5ac44-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ac44-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ac44-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ac44-130">Response</span></span>
<span data-ttu-id="5ac44-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ac44-131">If successful, this method returns a `200 OK` response code and [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ac44-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ac44-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ac44-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ac44-133">Request</span></span>
<span data-ttu-id="5ac44-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ac44-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="5ac44-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ac44-135">Response</span></span>
<span data-ttu-id="5ac44-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ac44-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1088

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
    "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "systemIntegrityProtectionEnabled": true,
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "storageRequireEncryption": true,
    "firewallEnabled": true,
    "firewallBlockAllIncoming": true,
    "firewallEnableStealthMode": true
  }
}
```




