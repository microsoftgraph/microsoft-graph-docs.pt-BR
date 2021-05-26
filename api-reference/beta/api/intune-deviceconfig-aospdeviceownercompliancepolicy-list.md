---
title: Listar aospDeviceOwnerCompliancePolicies
description: Listar propriedades e relações dos objetos aospDeviceOwnerCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: abd243eb77d39a09aa128161d806f4f41994293a
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665674"
---
# <a name="list-aospdeviceownercompliancepolicies"></a><span data-ttu-id="0dfec-103">Listar aospDeviceOwnerCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="0dfec-103">List aospDeviceOwnerCompliancePolicies</span></span>

<span data-ttu-id="0dfec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dfec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0dfec-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0dfec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0dfec-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0dfec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dfec-107">Listar propriedades e relações dos [objetos aospDeviceOwnerCompliancePolicy.](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0dfec-107">List properties and relationships of the [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0dfec-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0dfec-108">Prerequisites</span></span>
<span data-ttu-id="0dfec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0dfec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0dfec-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0dfec-111">Permission type</span></span>|<span data-ttu-id="0dfec-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0dfec-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0dfec-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0dfec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0dfec-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dfec-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0dfec-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0dfec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0dfec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0dfec-116">Not supported.</span></span>|
|<span data-ttu-id="0dfec-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0dfec-117">Application</span></span>|<span data-ttu-id="0dfec-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dfec-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0dfec-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0dfec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="0dfec-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0dfec-120">Request headers</span></span>
|<span data-ttu-id="0dfec-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0dfec-121">Header</span></span>|<span data-ttu-id="0dfec-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0dfec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0dfec-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0dfec-123">Authorization</span></span>|<span data-ttu-id="0dfec-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0dfec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0dfec-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0dfec-125">Accept</span></span>|<span data-ttu-id="0dfec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0dfec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0dfec-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0dfec-127">Request body</span></span>
<span data-ttu-id="0dfec-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0dfec-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0dfec-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0dfec-129">Response</span></span>
<span data-ttu-id="0dfec-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0dfec-130">If successful, this method returns a `200 OK` response code and a collection of [aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0dfec-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0dfec-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0dfec-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0dfec-132">Request</span></span>
<span data-ttu-id="0dfec-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0dfec-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="0dfec-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0dfec-134">Response</span></span>
<span data-ttu-id="0dfec-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0dfec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 870

{
  "value": [
    {
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
  ]
}
```




