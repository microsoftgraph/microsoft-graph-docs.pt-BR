---
title: Obter aospDeviceOwnerCompliancePolicy
description: Leia propriedades e relações do objeto aospDeviceOwnerCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b3ba46583fd770bab0d0a418b7ee749c058dc01f
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665677"
---
# <a name="get-aospdeviceownercompliancepolicy"></a><span data-ttu-id="ba559-103">Obter aospDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ba559-103">Get aospDeviceOwnerCompliancePolicy</span></span>

<span data-ttu-id="ba559-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba559-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba559-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ba559-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba559-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ba559-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba559-107">Leia propriedades e relações do [objeto aospDeviceOwnerCompliancePolicy.](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ba559-107">Read properties and relationships of the [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba559-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ba559-108">Prerequisites</span></span>
<span data-ttu-id="ba559-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba559-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba559-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba559-111">Permission type</span></span>|<span data-ttu-id="ba559-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba559-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba559-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba559-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba559-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba559-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ba559-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba559-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba559-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba559-116">Not supported.</span></span>|
|<span data-ttu-id="ba559-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba559-117">Application</span></span>|<span data-ttu-id="ba559-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba559-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba559-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba559-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba559-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ba559-120">Optional query parameters</span></span>
<span data-ttu-id="ba559-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ba559-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba559-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba559-122">Request headers</span></span>
|<span data-ttu-id="ba559-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ba559-123">Header</span></span>|<span data-ttu-id="ba559-124">Valor</span><span class="sxs-lookup"><span data-stu-id="ba559-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba559-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba559-125">Authorization</span></span>|<span data-ttu-id="ba559-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba559-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba559-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ba559-127">Accept</span></span>|<span data-ttu-id="ba559-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ba559-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba559-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba559-129">Request body</span></span>
<span data-ttu-id="ba559-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ba559-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba559-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba559-131">Response</span></span>
<span data-ttu-id="ba559-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba559-132">If successful, this method returns a `200 OK` response code and [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba559-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba559-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba559-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba559-134">Request</span></span>
<span data-ttu-id="ba559-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba559-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="ba559-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba559-136">Response</span></span>
<span data-ttu-id="ba559-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba559-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 820

{
  "value": {
    "@odata.type": "#microsoft.graph.aospDeviceOwnerCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "0837b942-b942-0837-42b9-370842b93708",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
    "passwordRequired": true,
    "passwordRequiredType": "required",
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordMinimumLength": 5,
    "storageRequireEncryption": true
  }
}
```




