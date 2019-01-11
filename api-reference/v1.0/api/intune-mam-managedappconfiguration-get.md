---
title: Get managedAppConfiguration
description: Ler propriedades e relações do objeto managedAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7638112219202d6a76e10691b31092bdc065c32e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837055"
---
# <a name="get-managedappconfiguration"></a><span data-ttu-id="57424-103">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="57424-103">Get managedAppConfiguration</span></span>

> <span data-ttu-id="57424-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="57424-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57424-105">Ler propriedades e relações do objeto [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="57424-105">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="57424-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57424-106">Prerequisites</span></span>
<span data-ttu-id="57424-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57424-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57424-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57424-109">Permission type</span></span>|<span data-ttu-id="57424-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="57424-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57424-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57424-111">Delegated (work or school account)</span></span>|<span data-ttu-id="57424-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="57424-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="57424-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57424-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57424-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57424-114">Not supported.</span></span>|
|<span data-ttu-id="57424-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57424-115">Application</span></span>|<span data-ttu-id="57424-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57424-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57424-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57424-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="57424-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="57424-118">Optional query parameters</span></span>
<span data-ttu-id="57424-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="57424-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="57424-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57424-120">Request headers</span></span>
|<span data-ttu-id="57424-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57424-121">Header</span></span>|<span data-ttu-id="57424-122">Valor</span><span class="sxs-lookup"><span data-stu-id="57424-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57424-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="57424-123">Authorization</span></span>|<span data-ttu-id="57424-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57424-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57424-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="57424-125">Accept</span></span>|<span data-ttu-id="57424-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57424-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57424-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57424-127">Request body</span></span>
<span data-ttu-id="57424-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57424-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57424-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="57424-129">Response</span></span>
<span data-ttu-id="57424-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57424-130">If successful, this method returns a `200 OK` response code and [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57424-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57424-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="57424-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57424-132">Request</span></span>
<span data-ttu-id="57424-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57424-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="57424-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="57424-134">Response</span></span>
<span data-ttu-id="57424-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57424-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 550

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppConfiguration",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "2ed27cb5-7cb5-2ed2-b57c-d22eb57cd22e",
    "version": "Version value",
    "customSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ]
  }
}
```



