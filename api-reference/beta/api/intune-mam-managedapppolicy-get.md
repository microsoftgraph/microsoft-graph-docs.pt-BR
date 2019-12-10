---
title: Get managedAppPolicy
description: Ler propriedades e relações do objeto managedAppPolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: adc64b3df1fb26af8b824022f618317b70a11603
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39942364"
---
# <a name="get-managedapppolicy"></a><span data-ttu-id="d49ef-103">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="d49ef-103">Get managedAppPolicy</span></span>

> <span data-ttu-id="d49ef-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d49ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d49ef-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d49ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d49ef-106">Ler propriedades e relações do objeto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d49ef-106">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d49ef-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d49ef-107">Prerequisites</span></span>
<span data-ttu-id="d49ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d49ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d49ef-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d49ef-110">Permission type</span></span>|<span data-ttu-id="d49ef-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d49ef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d49ef-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d49ef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d49ef-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d49ef-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d49ef-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d49ef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d49ef-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d49ef-115">Not supported.</span></span>|
|<span data-ttu-id="d49ef-116">Application</span><span class="sxs-lookup"><span data-stu-id="d49ef-116">Application</span></span>|<span data-ttu-id="d49ef-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d49ef-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d49ef-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d49ef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d49ef-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d49ef-119">Optional query parameters</span></span>
<span data-ttu-id="d49ef-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d49ef-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d49ef-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d49ef-121">Request headers</span></span>
|<span data-ttu-id="d49ef-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d49ef-122">Header</span></span>|<span data-ttu-id="d49ef-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d49ef-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d49ef-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d49ef-124">Authorization</span></span>|<span data-ttu-id="d49ef-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d49ef-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d49ef-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d49ef-126">Accept</span></span>|<span data-ttu-id="d49ef-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d49ef-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d49ef-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d49ef-128">Request body</span></span>
<span data-ttu-id="d49ef-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d49ef-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d49ef-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d49ef-130">Response</span></span>
<span data-ttu-id="d49ef-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d49ef-131">If successful, this method returns a `200 OK` response code and [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d49ef-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d49ef-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d49ef-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d49ef-133">Request</span></span>
<span data-ttu-id="d49ef-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d49ef-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="d49ef-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d49ef-135">Response</span></span>
<span data-ttu-id="d49ef-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d49ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





