---
title: Listar windowsPhone81CompliancePolicies
description: Listar propriedades e relações dos objetos windowsPhone81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7076164fa9a2c2e0e19951a577fce55d7c391144
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250464"
---
# <a name="list-windowsphone81compliancepolicies"></a><span data-ttu-id="5f193-103">Listar windowsPhone81CompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="5f193-103">List windowsPhone81CompliancePolicies</span></span>

> <span data-ttu-id="5f193-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5f193-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f193-105">Listar propriedades e relações dos objetos [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5f193-105">List properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f193-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5f193-106">Prerequisites</span></span>
<span data-ttu-id="5f193-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5f193-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5f193-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f193-109">Permission type</span></span>|<span data-ttu-id="5f193-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5f193-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f193-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f193-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5f193-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f193-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5f193-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f193-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f193-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f193-114">Not supported.</span></span>|
|<span data-ttu-id="5f193-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f193-115">Application</span></span>|<span data-ttu-id="5f193-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f193-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f193-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f193-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="5f193-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f193-118">Request headers</span></span>
|<span data-ttu-id="5f193-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5f193-119">Header</span></span>|<span data-ttu-id="5f193-120">Valor</span><span class="sxs-lookup"><span data-stu-id="5f193-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f193-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f193-121">Authorization</span></span>|<span data-ttu-id="5f193-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f193-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f193-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5f193-123">Accept</span></span>|<span data-ttu-id="5f193-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5f193-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f193-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f193-125">Request body</span></span>
<span data-ttu-id="5f193-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5f193-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f193-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f193-127">Response</span></span>
<span data-ttu-id="5f193-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f193-128">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f193-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f193-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f193-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f193-130">Request</span></span>
<span data-ttu-id="5f193-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f193-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="5f193-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f193-132">Response</span></span>
<span data-ttu-id="5f193-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f193-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 884

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
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



