---
title: Get deviceConfiguration
description: Ler propriedades e relações do objeto deviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e3b034220c064babe56a86d5106a29e8ae3813d0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52748380"
---
# <a name="get-deviceconfiguration"></a><span data-ttu-id="12b68-103">Get deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="12b68-103">Get deviceConfiguration</span></span>

<span data-ttu-id="12b68-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12b68-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12b68-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12b68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12b68-106">Ler propriedades e relações do objeto [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12b68-106">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12b68-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="12b68-107">Prerequisites</span></span>
<span data-ttu-id="12b68-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12b68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12b68-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12b68-110">Permission type</span></span>|<span data-ttu-id="12b68-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12b68-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12b68-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12b68-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12b68-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12b68-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="12b68-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12b68-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12b68-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12b68-115">Not supported.</span></span>|
|<span data-ttu-id="12b68-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12b68-116">Application</span></span>|<span data-ttu-id="12b68-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12b68-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12b68-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12b68-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12b68-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="12b68-119">Optional query parameters</span></span>
<span data-ttu-id="12b68-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="12b68-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12b68-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12b68-121">Request headers</span></span>
|<span data-ttu-id="12b68-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12b68-122">Header</span></span>|<span data-ttu-id="12b68-123">Valor</span><span class="sxs-lookup"><span data-stu-id="12b68-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12b68-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="12b68-124">Authorization</span></span>|<span data-ttu-id="12b68-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12b68-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12b68-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="12b68-126">Accept</span></span>|<span data-ttu-id="12b68-127">application/json</span><span class="sxs-lookup"><span data-stu-id="12b68-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12b68-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12b68-128">Request body</span></span>
<span data-ttu-id="12b68-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="12b68-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12b68-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="12b68-130">Response</span></span>
<span data-ttu-id="12b68-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12b68-131">If successful, this method returns a `200 OK` response code and [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12b68-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12b68-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="12b68-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12b68-133">Request</span></span>
<span data-ttu-id="12b68-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12b68-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="12b68-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="12b68-135">Response</span></span>
<span data-ttu-id="12b68-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12b68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 362

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfiguration",
    "id": "34977265-7265-3497-6572-973465729734",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```




