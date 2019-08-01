---
title: Acessar windowsPhone81CustomConfiguration
description: Leia as propriedades e as relações do objeto windowsPhone81CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1d236a1ee41b15c4b44c775f8a041c66aada394e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997040"
---
# <a name="get-windowsphone81customconfiguration"></a><span data-ttu-id="5a942-103">Acessar windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="5a942-103">Get windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="5a942-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5a942-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a942-105">Leia as propriedades e as relações do objeto [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a942-105">Read properties and relationships of the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a942-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5a942-106">Prerequisites</span></span>
<span data-ttu-id="5a942-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a942-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a942-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a942-109">Permission type</span></span>|<span data-ttu-id="5a942-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5a942-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a942-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a942-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5a942-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a942-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5a942-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a942-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a942-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a942-114">Not supported.</span></span>|
|<span data-ttu-id="5a942-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a942-115">Application</span></span>|<span data-ttu-id="5a942-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a942-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a942-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a942-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5a942-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5a942-118">Optional query parameters</span></span>
<span data-ttu-id="5a942-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5a942-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a942-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a942-120">Request headers</span></span>
|<span data-ttu-id="5a942-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5a942-121">Header</span></span>|<span data-ttu-id="5a942-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5a942-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a942-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a942-123">Authorization</span></span>|<span data-ttu-id="5a942-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a942-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a942-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5a942-125">Accept</span></span>|<span data-ttu-id="5a942-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5a942-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a942-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a942-127">Request body</span></span>
<span data-ttu-id="5a942-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5a942-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a942-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a942-129">Response</span></span>
<span data-ttu-id="5a942-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a942-130">If successful, this method returns a `200 OK` response code and [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a942-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a942-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a942-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a942-132">Request</span></span>
<span data-ttu-id="5a942-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a942-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5a942-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a942-134">Response</span></span>
<span data-ttu-id="5a942-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a942-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 632

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
    "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "omaSettings": [
      {
        "@odata.type": "microsoft.graph.omaSettingInteger",
        "displayName": "Display Name value",
        "description": "Description value",
        "omaUri": "Oma Uri value",
        "value": 5
      }
    ]
  }
}
```



