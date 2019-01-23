---
title: Get managedAppPolicy
description: Ler propriedades e relações do objeto managedAppPolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 72e139f796512ab5a97b8c62e71348767c296b45
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416283"
---
# <a name="get-managedapppolicy"></a><span data-ttu-id="40bea-103">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="40bea-103">Get managedAppPolicy</span></span>

> <span data-ttu-id="40bea-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="40bea-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="40bea-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="40bea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40bea-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="40bea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40bea-107">Ler propriedades e relações do objeto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="40bea-107">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40bea-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="40bea-108">Prerequisites</span></span>
<span data-ttu-id="40bea-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="40bea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="40bea-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40bea-111">Permission type</span></span>|<span data-ttu-id="40bea-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="40bea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40bea-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40bea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40bea-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="40bea-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="40bea-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40bea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40bea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40bea-116">Not supported.</span></span>|
|<span data-ttu-id="40bea-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40bea-117">Application</span></span>|<span data-ttu-id="40bea-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40bea-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40bea-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40bea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40bea-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="40bea-120">Optional query parameters</span></span>
<span data-ttu-id="40bea-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="40bea-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40bea-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40bea-122">Request headers</span></span>
|<span data-ttu-id="40bea-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40bea-123">Header</span></span>|<span data-ttu-id="40bea-124">Valor</span><span class="sxs-lookup"><span data-stu-id="40bea-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40bea-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="40bea-125">Authorization</span></span>|<span data-ttu-id="40bea-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40bea-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40bea-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="40bea-127">Accept</span></span>|<span data-ttu-id="40bea-128">application/json</span><span class="sxs-lookup"><span data-stu-id="40bea-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40bea-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40bea-129">Request body</span></span>
<span data-ttu-id="40bea-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="40bea-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40bea-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="40bea-131">Response</span></span>
<span data-ttu-id="40bea-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40bea-132">If successful, this method returns a `200 OK` response code and [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40bea-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40bea-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="40bea-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40bea-134">Request</span></span>
<span data-ttu-id="40bea-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40bea-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="40bea-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="40bea-136">Response</span></span>
<span data-ttu-id="40bea-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40bea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppPolicy",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
    "version": "Version value"
  }
}
```




