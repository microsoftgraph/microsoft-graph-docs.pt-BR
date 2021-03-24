---
title: Listar windowsPhone81CompliancePolicies
description: Listar propriedades e relações dos objetos windowsPhone81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ed2c1394499284ffcf309eda71dc2bb5853b9217
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132279"
---
# <a name="list-windowsphone81compliancepolicies"></a><span data-ttu-id="8d561-103">Listar windowsPhone81CompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="8d561-103">List windowsPhone81CompliancePolicies</span></span>

<span data-ttu-id="8d561-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d561-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d561-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8d561-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d561-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8d561-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d561-107">Listar propriedades e relações dos objetos [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8d561-107">List properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d561-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8d561-108">Prerequisites</span></span>
<span data-ttu-id="8d561-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d561-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d561-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d561-111">Permission type</span></span>|<span data-ttu-id="8d561-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d561-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d561-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d561-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d561-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d561-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d561-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d561-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d561-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d561-116">Not supported.</span></span>|
|<span data-ttu-id="8d561-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d561-117">Application</span></span>|<span data-ttu-id="8d561-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d561-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d561-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d561-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="8d561-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d561-120">Request headers</span></span>
|<span data-ttu-id="8d561-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8d561-121">Header</span></span>|<span data-ttu-id="8d561-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8d561-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d561-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d561-123">Authorization</span></span>|<span data-ttu-id="8d561-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d561-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d561-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8d561-125">Accept</span></span>|<span data-ttu-id="8d561-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d561-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d561-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d561-127">Request body</span></span>
<span data-ttu-id="8d561-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8d561-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d561-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d561-129">Response</span></span>
<span data-ttu-id="8d561-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d561-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d561-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d561-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d561-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d561-132">Request</span></span>
<span data-ttu-id="8d561-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d561-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="8d561-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d561-134">Response</span></span>
<span data-ttu-id="8d561-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d561-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




