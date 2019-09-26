---
title: Listar deviceCompliancePolicies
description: Listar propriedades e relações dos objetos deviceCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f74e59746e30dd4da6153acb268b3cf47bc64d87
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199463"
---
# <a name="list-devicecompliancepolicies"></a><span data-ttu-id="49b93-103">Listar deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="49b93-103">List deviceCompliancePolicies</span></span>

> <span data-ttu-id="49b93-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="49b93-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49b93-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49b93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49b93-106">Listar propriedades e relações dos objetos [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="49b93-106">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49b93-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="49b93-107">Prerequisites</span></span>
<span data-ttu-id="49b93-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49b93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49b93-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49b93-110">Permission type</span></span>|<span data-ttu-id="49b93-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="49b93-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49b93-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49b93-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="49b93-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="49b93-113">&nbsp; &nbsp; **Device configuration**</span></span>  | <span data-ttu-id="49b93-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="49b93-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="49b93-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="49b93-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="49b93-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="49b93-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="49b93-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49b93-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49b93-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49b93-118">Not supported.</span></span>|
|<span data-ttu-id="49b93-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49b93-119">Application</span></span>||
| <span data-ttu-id="49b93-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="49b93-120">&nbsp; &nbsp; **Device configuration**</span></span>  | <span data-ttu-id="49b93-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="49b93-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="49b93-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="49b93-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="49b93-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="49b93-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49b93-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49b93-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="49b93-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49b93-125">Request headers</span></span>
|<span data-ttu-id="49b93-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49b93-126">Header</span></span>|<span data-ttu-id="49b93-127">Valor</span><span class="sxs-lookup"><span data-stu-id="49b93-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49b93-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="49b93-128">Authorization</span></span>|<span data-ttu-id="49b93-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49b93-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49b93-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="49b93-130">Accept</span></span>|<span data-ttu-id="49b93-131">application/json</span><span class="sxs-lookup"><span data-stu-id="49b93-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49b93-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49b93-132">Request body</span></span>
<span data-ttu-id="49b93-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="49b93-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49b93-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="49b93-134">Response</span></span>
<span data-ttu-id="49b93-135">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49b93-135">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49b93-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49b93-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="49b93-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49b93-137">Request</span></span>
<span data-ttu-id="49b93-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49b93-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="49b93-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="49b93-139">Response</span></span>
<span data-ttu-id="49b93-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49b93-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 467

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "4214b716-b716-4214-16b7-144216b71442",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```




