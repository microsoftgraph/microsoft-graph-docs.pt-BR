---
title: Acessar targetedManagedAppConfiguration
description: Leia as propriedades e as relações do objeto targetedManagedAppConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f6f4edd792e42fc3d3db0cfd9326ede4a474ec10
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37363231"
---
# <a name="get-targetedmanagedappconfiguration"></a><span data-ttu-id="50532-103">Acessar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="50532-103">Get targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="50532-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50532-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50532-105">Leia as propriedades e as relações do objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50532-105">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50532-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50532-106">Prerequisites</span></span>
<span data-ttu-id="50532-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50532-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50532-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50532-109">Permission type</span></span>|<span data-ttu-id="50532-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50532-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50532-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50532-111">Delegated (work or school account)</span></span>|<span data-ttu-id="50532-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="50532-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="50532-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50532-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50532-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50532-114">Not supported.</span></span>|
|<span data-ttu-id="50532-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50532-115">Application</span></span>|<span data-ttu-id="50532-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50532-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50532-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50532-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="50532-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="50532-118">Optional query parameters</span></span>
<span data-ttu-id="50532-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="50532-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50532-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50532-120">Request headers</span></span>
|<span data-ttu-id="50532-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50532-121">Header</span></span>|<span data-ttu-id="50532-122">Valor</span><span class="sxs-lookup"><span data-stu-id="50532-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50532-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="50532-123">Authorization</span></span>|<span data-ttu-id="50532-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50532-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50532-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50532-125">Accept</span></span>|<span data-ttu-id="50532-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50532-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50532-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50532-127">Request body</span></span>
<span data-ttu-id="50532-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="50532-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50532-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="50532-129">Response</span></span>
<span data-ttu-id="50532-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50532-130">If successful, this method returns a `200 OK` response code and [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50532-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50532-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="50532-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50532-132">Request</span></span>
<span data-ttu-id="50532-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50532-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="50532-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="50532-134">Response</span></span>
<span data-ttu-id="50532-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50532-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 611

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "2444e029-e029-2444-29e0-442429e04424",
    "version": "Version value",
    "customSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "deployedAppCount": 0,
    "isAssigned": true
  }
}
```




