---
title: Acessar deviceCompliancePolicy
description: Leia as propriedades e as relações do objeto deviceCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b83f9dbd62ff8e54119af023c0ee5646ace8db22
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43390817"
---
# <a name="get-devicecompliancepolicy"></a><span data-ttu-id="fe7ee-103">Acessar deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="fe7ee-103">Get deviceCompliancePolicy</span></span>

<span data-ttu-id="fe7ee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe7ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe7ee-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fe7ee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe7ee-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fe7ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe7ee-107">Leia as propriedades e as relações do objeto [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fe7ee-107">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe7ee-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fe7ee-108">Prerequisites</span></span>
<span data-ttu-id="fe7ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe7ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe7ee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe7ee-111">Permission type</span></span>|<span data-ttu-id="fe7ee-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fe7ee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe7ee-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe7ee-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fe7ee-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="fe7ee-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="fe7ee-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe7ee-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="fe7ee-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="fe7ee-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="fe7ee-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe7ee-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fe7ee-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe7ee-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe7ee-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe7ee-119">Not supported.</span></span>|
|<span data-ttu-id="fe7ee-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe7ee-120">Application</span></span>|| 
|<span data-ttu-id="fe7ee-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="fe7ee-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="fe7ee-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe7ee-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="fe7ee-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="fe7ee-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="fe7ee-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe7ee-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe7ee-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe7ee-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe7ee-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fe7ee-126">Optional query parameters</span></span>
<span data-ttu-id="fe7ee-127">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fe7ee-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe7ee-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe7ee-128">Request headers</span></span>
|<span data-ttu-id="fe7ee-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe7ee-129">Header</span></span>|<span data-ttu-id="fe7ee-130">Valor</span><span class="sxs-lookup"><span data-stu-id="fe7ee-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe7ee-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe7ee-131">Authorization</span></span>|<span data-ttu-id="fe7ee-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe7ee-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe7ee-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fe7ee-133">Accept</span></span>|<span data-ttu-id="fe7ee-134">application/json</span><span class="sxs-lookup"><span data-stu-id="fe7ee-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe7ee-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe7ee-135">Request body</span></span>
<span data-ttu-id="fe7ee-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe7ee-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe7ee-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe7ee-137">Response</span></span>
<span data-ttu-id="fe7ee-138">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe7ee-138">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe7ee-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe7ee-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe7ee-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe7ee-140">Request</span></span>
<span data-ttu-id="fe7ee-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe7ee-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="fe7ee-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe7ee-142">Response</span></span>
<span data-ttu-id="fe7ee-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe7ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






