---
title: Get androidCustomConfiguration
description: Ler propriedades e relações do objeto androidCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e624efd590c8de44a35a239cfada54323cb7d95
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455011"
---
# <a name="get-androidcustomconfiguration"></a><span data-ttu-id="84b5f-103">Get androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="84b5f-103">Get androidCustomConfiguration</span></span>

<span data-ttu-id="84b5f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84b5f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84b5f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84b5f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84b5f-106">Ler propriedades e relações do objeto [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84b5f-106">Read properties and relationships of the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84b5f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="84b5f-107">Prerequisites</span></span>
<span data-ttu-id="84b5f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84b5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84b5f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84b5f-110">Permission type</span></span>|<span data-ttu-id="84b5f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="84b5f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84b5f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84b5f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84b5f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="84b5f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="84b5f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84b5f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84b5f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84b5f-115">Not supported.</span></span>|
|<span data-ttu-id="84b5f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84b5f-116">Application</span></span>|<span data-ttu-id="84b5f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84b5f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84b5f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84b5f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="84b5f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="84b5f-119">Optional query parameters</span></span>
<span data-ttu-id="84b5f-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="84b5f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84b5f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84b5f-121">Request headers</span></span>
|<span data-ttu-id="84b5f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="84b5f-122">Header</span></span>|<span data-ttu-id="84b5f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="84b5f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84b5f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="84b5f-124">Authorization</span></span>|<span data-ttu-id="84b5f-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84b5f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84b5f-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="84b5f-126">Accept</span></span>|<span data-ttu-id="84b5f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="84b5f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84b5f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84b5f-128">Request body</span></span>
<span data-ttu-id="84b5f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="84b5f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84b5f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="84b5f-130">Response</span></span>
<span data-ttu-id="84b5f-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84b5f-131">If successful, this method returns a `200 OK` response code and [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84b5f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84b5f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="84b5f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84b5f-133">Request</span></span>
<span data-ttu-id="84b5f-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84b5f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="84b5f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="84b5f-135">Response</span></span>
<span data-ttu-id="84b5f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84b5f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 625

{
  "value": {
    "@odata.type": "#microsoft.graph.androidCustomConfiguration",
    "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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






