---
title: Listar windowsPhone81CompliancePolicies
description: Listar propriedades e relações dos objetos windowsPhone81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bd8b1e0a5d062d9482e9188b643be759c8e55807
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696864"
---
# <a name="list-windowsphone81compliancepolicies"></a><span data-ttu-id="3c16d-103">Listar windowsPhone81CompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="3c16d-103">List windowsPhone81CompliancePolicies</span></span>

<span data-ttu-id="3c16d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c16d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c16d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3c16d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c16d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c16d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c16d-107">Listar propriedades e relações dos objetos [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3c16d-107">List properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c16d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3c16d-108">Prerequisites</span></span>
<span data-ttu-id="3c16d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c16d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c16d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c16d-111">Permission type</span></span>|<span data-ttu-id="3c16d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3c16d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c16d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c16d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c16d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c16d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3c16d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c16d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c16d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c16d-116">Not supported.</span></span>|
|<span data-ttu-id="3c16d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c16d-117">Application</span></span>|<span data-ttu-id="3c16d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c16d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c16d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c16d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="3c16d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c16d-120">Request headers</span></span>
|<span data-ttu-id="3c16d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c16d-121">Header</span></span>|<span data-ttu-id="3c16d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3c16d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c16d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c16d-123">Authorization</span></span>|<span data-ttu-id="3c16d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c16d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c16d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3c16d-125">Accept</span></span>|<span data-ttu-id="3c16d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c16d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c16d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c16d-127">Request body</span></span>
<span data-ttu-id="3c16d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c16d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c16d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c16d-129">Response</span></span>
<span data-ttu-id="3c16d-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c16d-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c16d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c16d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c16d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c16d-132">Request</span></span>
<span data-ttu-id="3c16d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c16d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="3c16d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c16d-134">Response</span></span>
<span data-ttu-id="3c16d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c16d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 958

{
  "value": [
    {
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
  ]
}
```





