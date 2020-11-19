---
title: Acessar deviceCompliancePolicy
description: Leia as propriedades e as relações do objeto deviceCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fa9c5a6cdea76b19f865adc5eda2798d0d484797
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295905"
---
# <a name="get-devicecompliancepolicy"></a><span data-ttu-id="22285-103">Acessar deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="22285-103">Get deviceCompliancePolicy</span></span>

<span data-ttu-id="22285-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22285-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22285-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="22285-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22285-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22285-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22285-107">Leia as propriedades e as relações do objeto [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="22285-107">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22285-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22285-108">Prerequisites</span></span>
<span data-ttu-id="22285-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22285-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22285-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22285-111">Permission type</span></span>|<span data-ttu-id="22285-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22285-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22285-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22285-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="22285-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="22285-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="22285-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22285-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="22285-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="22285-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="22285-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22285-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="22285-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22285-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22285-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22285-119">Not supported.</span></span>|
|<span data-ttu-id="22285-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22285-120">Application</span></span>|| 
|<span data-ttu-id="22285-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="22285-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="22285-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22285-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="22285-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="22285-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="22285-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22285-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22285-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22285-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22285-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="22285-126">Optional query parameters</span></span>
<span data-ttu-id="22285-127">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="22285-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22285-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22285-128">Request headers</span></span>
|<span data-ttu-id="22285-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22285-129">Header</span></span>|<span data-ttu-id="22285-130">Valor</span><span class="sxs-lookup"><span data-stu-id="22285-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22285-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="22285-131">Authorization</span></span>|<span data-ttu-id="22285-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22285-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22285-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22285-133">Accept</span></span>|<span data-ttu-id="22285-134">application/json</span><span class="sxs-lookup"><span data-stu-id="22285-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22285-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22285-135">Request body</span></span>
<span data-ttu-id="22285-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22285-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22285-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="22285-137">Response</span></span>
<span data-ttu-id="22285-138">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22285-138">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22285-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22285-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="22285-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22285-140">Request</span></span>
<span data-ttu-id="22285-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22285-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="22285-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="22285-142">Response</span></span>
<span data-ttu-id="22285-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22285-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 433

{
  "value": {
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
}
```







