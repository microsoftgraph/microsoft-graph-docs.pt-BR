---
title: Acessar windows81CompliancePolicy
description: Leia as propriedades e as relações do objeto windows81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d8360b23b22bbb1c1fed7f3e15608ec1b5531747
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733515"
---
# <a name="get-windows81compliancepolicy"></a><span data-ttu-id="5b83a-103">Acessar windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5b83a-103">Get windows81CompliancePolicy</span></span>

<span data-ttu-id="5b83a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b83a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b83a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5b83a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b83a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5b83a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b83a-107">Leia as propriedades e as relações do objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b83a-107">Read properties and relationships of the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b83a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5b83a-108">Prerequisites</span></span>
<span data-ttu-id="5b83a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b83a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b83a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b83a-111">Permission type</span></span>|<span data-ttu-id="5b83a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5b83a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b83a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b83a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b83a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b83a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5b83a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b83a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b83a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b83a-116">Not supported.</span></span>|
|<span data-ttu-id="5b83a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b83a-117">Application</span></span>|<span data-ttu-id="5b83a-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b83a-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b83a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b83a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5b83a-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5b83a-120">Optional query parameters</span></span>
<span data-ttu-id="5b83a-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5b83a-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b83a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b83a-122">Request headers</span></span>
|<span data-ttu-id="5b83a-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5b83a-123">Header</span></span>|<span data-ttu-id="5b83a-124">Valor</span><span class="sxs-lookup"><span data-stu-id="5b83a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b83a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b83a-125">Authorization</span></span>|<span data-ttu-id="5b83a-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b83a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b83a-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5b83a-127">Accept</span></span>|<span data-ttu-id="5b83a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5b83a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b83a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b83a-129">Request body</span></span>
<span data-ttu-id="5b83a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5b83a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b83a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b83a-131">Response</span></span>
<span data-ttu-id="5b83a-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b83a-132">If successful, this method returns a `200 OK` response code and [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b83a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b83a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b83a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b83a-134">Request</span></span>
<span data-ttu-id="5b83a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b83a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="5b83a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b83a-136">Response</span></span>
<span data-ttu-id="5b83a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b83a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 897

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
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
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "storageRequireEncryption": true
  }
}
```





