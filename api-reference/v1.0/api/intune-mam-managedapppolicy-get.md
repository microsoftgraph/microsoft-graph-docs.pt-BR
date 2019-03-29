---
title: Get managedAppPolicy
description: Ler propriedades e relações do objeto managedAppPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3eafd1efaf4368d81445d103e1d2e16ce012ba1f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957266"
---
# <a name="get-managedapppolicy"></a><span data-ttu-id="d652f-103">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="d652f-103">Get managedAppPolicy</span></span>

> <span data-ttu-id="d652f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d652f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d652f-105">Ler propriedades e relações do objeto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d652f-105">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d652f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d652f-106">Prerequisites</span></span>
<span data-ttu-id="d652f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d652f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d652f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d652f-109">Permission type</span></span>|<span data-ttu-id="d652f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d652f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d652f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d652f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d652f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d652f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d652f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d652f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d652f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d652f-114">Not supported.</span></span>|
|<span data-ttu-id="d652f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d652f-115">Application</span></span>|<span data-ttu-id="d652f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d652f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d652f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d652f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d652f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d652f-118">Optional query parameters</span></span>
<span data-ttu-id="d652f-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d652f-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d652f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d652f-120">Request headers</span></span>
|<span data-ttu-id="d652f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d652f-121">Header</span></span>|<span data-ttu-id="d652f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d652f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d652f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d652f-123">Authorization</span></span>|<span data-ttu-id="d652f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d652f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d652f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d652f-125">Accept</span></span>|<span data-ttu-id="d652f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d652f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d652f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d652f-127">Request body</span></span>
<span data-ttu-id="d652f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d652f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d652f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d652f-129">Response</span></span>
<span data-ttu-id="d652f-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d652f-130">If successful, this method returns a `200 OK` response code and [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d652f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d652f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d652f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d652f-132">Request</span></span>
<span data-ttu-id="d652f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d652f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="d652f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d652f-134">Response</span></span>
<span data-ttu-id="d652f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d652f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 373

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppPolicy",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
    "version": "Version value"
  }
}
```



