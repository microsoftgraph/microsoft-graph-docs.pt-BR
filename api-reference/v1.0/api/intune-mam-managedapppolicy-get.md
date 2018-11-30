---
title: Get managedAppPolicy
description: Ler propriedades e relações do objeto managedAppPolicy.
ms.openlocfilehash: 606e592afb95c2bb68067559bc54e50219781d4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005064"
---
# <a name="get-managedapppolicy"></a><span data-ttu-id="97b73-103">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="97b73-103">Get managedAppPolicy</span></span>

> <span data-ttu-id="97b73-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="97b73-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97b73-105">Ler propriedades e relações do objeto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="97b73-105">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="97b73-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97b73-106">Prerequisites</span></span>
<span data-ttu-id="97b73-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97b73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97b73-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97b73-109">Permission type</span></span>|<span data-ttu-id="97b73-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="97b73-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97b73-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97b73-111">Delegated (work or school account)</span></span>|<span data-ttu-id="97b73-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="97b73-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="97b73-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97b73-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97b73-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97b73-114">Not supported.</span></span>|
|<span data-ttu-id="97b73-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97b73-115">Application</span></span>|<span data-ttu-id="97b73-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97b73-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97b73-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97b73-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="97b73-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="97b73-118">Optional query parameters</span></span>
<span data-ttu-id="97b73-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="97b73-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="97b73-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97b73-120">Request headers</span></span>
|<span data-ttu-id="97b73-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97b73-121">Header</span></span>|<span data-ttu-id="97b73-122">Valor</span><span class="sxs-lookup"><span data-stu-id="97b73-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97b73-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="97b73-123">Authorization</span></span>|<span data-ttu-id="97b73-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97b73-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97b73-125">Accept</span><span class="sxs-lookup"><span data-stu-id="97b73-125">Accept</span></span>|<span data-ttu-id="97b73-126">application/json</span><span class="sxs-lookup"><span data-stu-id="97b73-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97b73-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97b73-127">Request body</span></span>
<span data-ttu-id="97b73-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97b73-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97b73-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="97b73-129">Response</span></span>
<span data-ttu-id="97b73-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97b73-130">If successful, this method returns a `200 OK` response code and [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97b73-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97b73-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="97b73-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97b73-132">Request</span></span>
<span data-ttu-id="97b73-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97b73-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="97b73-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="97b73-134">Response</span></span>
<span data-ttu-id="97b73-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97b73-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



