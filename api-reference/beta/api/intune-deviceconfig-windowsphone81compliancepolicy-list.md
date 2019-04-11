---
title: Listar windowsPhone81CompliancePolicies
description: Listar propriedades e relações dos objetos windowsPhone81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ecd3bc2577745a52c899e56f0f050c870e5e12f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31800746"
---
# <a name="list-windowsphone81compliancepolicies"></a><span data-ttu-id="19199-103">Listar windowsPhone81CompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="19199-103">List windowsPhone81CompliancePolicies</span></span>

> <span data-ttu-id="19199-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="19199-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19199-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="19199-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19199-106">Listar propriedades e relações dos objetos [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="19199-106">List properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19199-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="19199-107">Prerequisites</span></span>
<span data-ttu-id="19199-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19199-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19199-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19199-110">Permission type</span></span>|<span data-ttu-id="19199-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="19199-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19199-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19199-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19199-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="19199-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="19199-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19199-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19199-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19199-115">Not supported.</span></span>|
|<span data-ttu-id="19199-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19199-116">Application</span></span>|<span data-ttu-id="19199-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19199-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19199-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19199-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="19199-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19199-119">Request headers</span></span>
|<span data-ttu-id="19199-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="19199-120">Header</span></span>|<span data-ttu-id="19199-121">Valor</span><span class="sxs-lookup"><span data-stu-id="19199-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19199-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="19199-122">Authorization</span></span>|<span data-ttu-id="19199-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19199-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19199-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="19199-124">Accept</span></span>|<span data-ttu-id="19199-125">application/json</span><span class="sxs-lookup"><span data-stu-id="19199-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19199-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19199-126">Request body</span></span>
<span data-ttu-id="19199-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="19199-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19199-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="19199-128">Response</span></span>
<span data-ttu-id="19199-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19199-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19199-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19199-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="19199-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19199-131">Request</span></span>
<span data-ttu-id="19199-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19199-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="19199-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="19199-133">Response</span></span>
<span data-ttu-id="19199-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19199-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





