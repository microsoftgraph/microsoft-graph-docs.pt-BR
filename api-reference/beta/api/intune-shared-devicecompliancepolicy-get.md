---
title: Acessar deviceCompliancePolicy
description: Leia as propriedades e as relações do objeto deviceCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5cc9c1b324d92a7b9a561a053ee9b1949c808fff
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199466"
---
# <a name="get-devicecompliancepolicy"></a><span data-ttu-id="1ff07-103">Acessar deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="1ff07-103">Get deviceCompliancePolicy</span></span>

> <span data-ttu-id="1ff07-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1ff07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ff07-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ff07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ff07-106">Leia as propriedades e as relações do objeto [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1ff07-106">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ff07-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1ff07-107">Prerequisites</span></span>
<span data-ttu-id="1ff07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ff07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ff07-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ff07-110">Permission type</span></span>|<span data-ttu-id="1ff07-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1ff07-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ff07-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ff07-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1ff07-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="1ff07-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="1ff07-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ff07-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="1ff07-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="1ff07-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="1ff07-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ff07-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1ff07-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ff07-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ff07-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ff07-118">Not supported.</span></span>|
|<span data-ttu-id="1ff07-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ff07-119">Application</span></span>|| 
|<span data-ttu-id="1ff07-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="1ff07-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="1ff07-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ff07-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="1ff07-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="1ff07-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="1ff07-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ff07-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ff07-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ff07-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1ff07-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1ff07-125">Optional query parameters</span></span>
<span data-ttu-id="1ff07-126">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1ff07-126">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ff07-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ff07-127">Request headers</span></span>
|<span data-ttu-id="1ff07-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1ff07-128">Header</span></span>|<span data-ttu-id="1ff07-129">Valor</span><span class="sxs-lookup"><span data-stu-id="1ff07-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ff07-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ff07-130">Authorization</span></span>|<span data-ttu-id="1ff07-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ff07-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ff07-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1ff07-132">Accept</span></span>|<span data-ttu-id="1ff07-133">application/json</span><span class="sxs-lookup"><span data-stu-id="1ff07-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ff07-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ff07-134">Request body</span></span>
<span data-ttu-id="1ff07-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1ff07-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ff07-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ff07-136">Response</span></span>
<span data-ttu-id="1ff07-137">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ff07-137">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ff07-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ff07-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ff07-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ff07-139">Request</span></span>
<span data-ttu-id="1ff07-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ff07-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="1ff07-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ff07-141">Response</span></span>
<span data-ttu-id="1ff07-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ff07-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




