---
title: Get windowsPhone81CompliancePolicy
description: Ler propriedades e relações do objeto windowsPhone81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1b607397c1c9fb4a88c46c99b86a4f2d71991fd2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785402"
---
# <a name="get-windowsphone81compliancepolicy"></a><span data-ttu-id="dc56a-103">Get windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="dc56a-103">Get windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="dc56a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dc56a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc56a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc56a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc56a-106">Ler propriedades e relações do objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dc56a-106">Read properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc56a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dc56a-107">Prerequisites</span></span>
<span data-ttu-id="dc56a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc56a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc56a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc56a-110">Permission type</span></span>|<span data-ttu-id="dc56a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dc56a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc56a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc56a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dc56a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc56a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dc56a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc56a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc56a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc56a-115">Not supported.</span></span>|
|<span data-ttu-id="dc56a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc56a-116">Application</span></span>|<span data-ttu-id="dc56a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc56a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc56a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc56a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dc56a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dc56a-119">Optional query parameters</span></span>
<span data-ttu-id="dc56a-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dc56a-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc56a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc56a-121">Request headers</span></span>
|<span data-ttu-id="dc56a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc56a-122">Header</span></span>|<span data-ttu-id="dc56a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="dc56a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc56a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc56a-124">Authorization</span></span>|<span data-ttu-id="dc56a-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc56a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc56a-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dc56a-126">Accept</span></span>|<span data-ttu-id="dc56a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="dc56a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc56a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc56a-128">Request body</span></span>
<span data-ttu-id="dc56a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dc56a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc56a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc56a-130">Response</span></span>
<span data-ttu-id="dc56a-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc56a-131">If successful, this method returns a `200 OK` response code and [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc56a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc56a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc56a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc56a-133">Request</span></span>
<span data-ttu-id="dc56a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc56a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="dc56a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc56a-135">Response</span></span>
<span data-ttu-id="dc56a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc56a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 902

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "passwordRequired": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "storageRequireEncryption": true
  }
}
```





