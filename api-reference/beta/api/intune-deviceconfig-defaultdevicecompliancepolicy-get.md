---
title: Obter defaultDeviceCompliancePolicy
description: Leia as propriedades e as relações do objeto defaultDeviceCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa78c14abe23ee1c4311cfc01e610c733a0c0fa3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968767"
---
# <a name="get-defaultdevicecompliancepolicy"></a><span data-ttu-id="50002-103">Obter defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="50002-103">Get defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="50002-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50002-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50002-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50002-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50002-106">Leia as propriedades e as relações do objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="50002-106">Read properties and relationships of the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50002-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50002-107">Prerequisites</span></span>
<span data-ttu-id="50002-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50002-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50002-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50002-110">Permission type</span></span>|<span data-ttu-id="50002-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50002-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50002-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50002-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50002-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="50002-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="50002-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50002-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50002-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50002-115">Not supported.</span></span>|
|<span data-ttu-id="50002-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50002-116">Application</span></span>|<span data-ttu-id="50002-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50002-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50002-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50002-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="50002-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="50002-119">Optional query parameters</span></span>
<span data-ttu-id="50002-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="50002-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50002-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50002-121">Request headers</span></span>
|<span data-ttu-id="50002-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50002-122">Header</span></span>|<span data-ttu-id="50002-123">Valor</span><span class="sxs-lookup"><span data-stu-id="50002-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50002-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="50002-124">Authorization</span></span>|<span data-ttu-id="50002-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50002-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50002-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50002-126">Accept</span></span>|<span data-ttu-id="50002-127">application/json</span><span class="sxs-lookup"><span data-stu-id="50002-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50002-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50002-128">Request body</span></span>
<span data-ttu-id="50002-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="50002-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50002-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="50002-130">Response</span></span>
<span data-ttu-id="50002-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50002-131">If successful, this method returns a `200 OK` response code and [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50002-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50002-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="50002-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50002-133">Request</span></span>
<span data-ttu-id="50002-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50002-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="50002-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="50002-135">Response</span></span>
<span data-ttu-id="50002-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50002-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 440

{
  "value": {
    "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "a285f027-f027-a285-27f0-85a227f085a2",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7
  }
}
```




