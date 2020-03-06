---
title: Acessar windows10EnterpriseModernAppManagementConfiguration
description: Leia as propriedades e as relações do objeto windows10EnterpriseModernAppManagementConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a6d06cd83e400eca8591286c261e74f1569e4eaf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514067"
---
# <a name="get-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="720bc-103">Acessar windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="720bc-103">Get windows10EnterpriseModernAppManagementConfiguration</span></span>

<span data-ttu-id="720bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="720bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="720bc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="720bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="720bc-106">Leia as propriedades e as relações do objeto [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="720bc-106">Read properties and relationships of the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="720bc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="720bc-107">Prerequisites</span></span>
<span data-ttu-id="720bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="720bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="720bc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="720bc-110">Permission type</span></span>|<span data-ttu-id="720bc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="720bc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="720bc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="720bc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="720bc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="720bc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="720bc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="720bc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="720bc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="720bc-115">Not supported.</span></span>|
|<span data-ttu-id="720bc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="720bc-116">Application</span></span>|<span data-ttu-id="720bc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="720bc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="720bc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="720bc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="720bc-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="720bc-119">Optional query parameters</span></span>
<span data-ttu-id="720bc-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="720bc-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="720bc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="720bc-121">Request headers</span></span>
|<span data-ttu-id="720bc-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="720bc-122">Header</span></span>|<span data-ttu-id="720bc-123">Valor</span><span class="sxs-lookup"><span data-stu-id="720bc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="720bc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="720bc-124">Authorization</span></span>|<span data-ttu-id="720bc-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="720bc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="720bc-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="720bc-126">Accept</span></span>|<span data-ttu-id="720bc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="720bc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="720bc-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="720bc-128">Request body</span></span>
<span data-ttu-id="720bc-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="720bc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="720bc-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="720bc-130">Response</span></span>
<span data-ttu-id="720bc-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="720bc-131">If successful, this method returns a `200 OK` response code and [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="720bc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="720bc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="720bc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="720bc-133">Request</span></span>
<span data-ttu-id="720bc-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="720bc-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="720bc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="720bc-135">Response</span></span>
<span data-ttu-id="720bc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="720bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 429

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
    "id": "d6577687-7687-d657-8776-57d6877657d6",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "uninstallBuiltInApps": true
  }
}
```




