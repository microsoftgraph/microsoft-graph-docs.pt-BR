---
title: Acessar targetedManagedAppConfiguration
description: Leia as propriedades e as relações do objeto targetedManagedAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c2d348884d053e694d06856810424f64995bf460
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43398147"
---
# <a name="get-targetedmanagedappconfiguration"></a><span data-ttu-id="abcef-103">Acessar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="abcef-103">Get targetedManagedAppConfiguration</span></span>

<span data-ttu-id="abcef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abcef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="abcef-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="abcef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abcef-106">Leia as propriedades e as relações do objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="abcef-106">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abcef-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="abcef-107">Prerequisites</span></span>
<span data-ttu-id="abcef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abcef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abcef-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abcef-110">Permission type</span></span>|<span data-ttu-id="abcef-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="abcef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abcef-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abcef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="abcef-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="abcef-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="abcef-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abcef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abcef-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abcef-115">Not supported.</span></span>|
|<span data-ttu-id="abcef-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="abcef-116">Application</span></span>|<span data-ttu-id="abcef-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abcef-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abcef-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abcef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="abcef-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="abcef-119">Optional query parameters</span></span>
<span data-ttu-id="abcef-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="abcef-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="abcef-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abcef-121">Request headers</span></span>
|<span data-ttu-id="abcef-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="abcef-122">Header</span></span>|<span data-ttu-id="abcef-123">Valor</span><span class="sxs-lookup"><span data-stu-id="abcef-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abcef-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="abcef-124">Authorization</span></span>|<span data-ttu-id="abcef-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abcef-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abcef-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="abcef-126">Accept</span></span>|<span data-ttu-id="abcef-127">application/json</span><span class="sxs-lookup"><span data-stu-id="abcef-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abcef-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abcef-128">Request body</span></span>
<span data-ttu-id="abcef-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="abcef-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abcef-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="abcef-130">Response</span></span>
<span data-ttu-id="abcef-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abcef-131">If successful, this method returns a `200 OK` response code and [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abcef-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abcef-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="abcef-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abcef-133">Request</span></span>
<span data-ttu-id="abcef-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abcef-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="abcef-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="abcef-135">Response</span></span>
<span data-ttu-id="abcef-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="abcef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






