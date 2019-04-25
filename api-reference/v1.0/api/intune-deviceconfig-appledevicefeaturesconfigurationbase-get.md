---
title: Acessar appleDeviceFeaturesConfigurationBase
description: Leia as propriedades e as relações do objeto appleDeviceFeaturesConfigurationBase.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5050ad58e92991f3deaf221ae84680d1b009d6f6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542001"
---
# <a name="get-appledevicefeaturesconfigurationbase"></a><span data-ttu-id="cff5c-103">Acessar appleDeviceFeaturesConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="cff5c-103">Get appleDeviceFeaturesConfigurationBase</span></span>

> <span data-ttu-id="cff5c-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cff5c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cff5c-105">Leia as propriedades e as relações do objeto [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="cff5c-105">Read properties and relationships of the [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cff5c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cff5c-106">Prerequisites</span></span>
<span data-ttu-id="cff5c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cff5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cff5c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cff5c-109">Permission type</span></span>|<span data-ttu-id="cff5c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cff5c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cff5c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cff5c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cff5c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cff5c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cff5c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cff5c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cff5c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cff5c-114">Not supported.</span></span>|
|<span data-ttu-id="cff5c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cff5c-115">Application</span></span>|<span data-ttu-id="cff5c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cff5c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cff5c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cff5c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cff5c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cff5c-118">Optional query parameters</span></span>
<span data-ttu-id="cff5c-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cff5c-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cff5c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cff5c-120">Request headers</span></span>
|<span data-ttu-id="cff5c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cff5c-121">Header</span></span>|<span data-ttu-id="cff5c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cff5c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cff5c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cff5c-123">Authorization</span></span>|<span data-ttu-id="cff5c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cff5c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cff5c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cff5c-125">Accept</span></span>|<span data-ttu-id="cff5c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cff5c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cff5c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cff5c-127">Request body</span></span>
<span data-ttu-id="cff5c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cff5c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cff5c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cff5c-129">Response</span></span>
<span data-ttu-id="cff5c-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cff5c-130">If successful, this method returns a `200 OK` response code and [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cff5c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cff5c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cff5c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cff5c-132">Request</span></span>
<span data-ttu-id="cff5c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cff5c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="cff5c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cff5c-134">Response</span></span>
<span data-ttu-id="cff5c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cff5c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 379

{
  "value": {
    "@odata.type": "#microsoft.graph.appleDeviceFeaturesConfigurationBase",
    "id": "ca0bb5ff-b5ff-ca0b-ffb5-0bcaffb50bca",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```



