---
title: Acessar deviceManagement
description: Leia as propriedades e as relações do objeto deviceManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3a95ded22a59bf5c29f1cda1349749b7c3f4adb2
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756405"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="2c81a-103">Acessar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="2c81a-103">Get deviceManagement</span></span>

<span data-ttu-id="2c81a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c81a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c81a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2c81a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c81a-106">Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-remoteassistance-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="2c81a-106">Read properties and relationships of the [deviceManagement](../resources/intune-remoteassistance-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c81a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2c81a-107">Prerequisites</span></span>
<span data-ttu-id="2c81a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c81a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c81a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c81a-110">Permission type</span></span>|<span data-ttu-id="2c81a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c81a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c81a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c81a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2c81a-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c81a-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2c81a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c81a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c81a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c81a-115">Not supported.</span></span>|
|<span data-ttu-id="2c81a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c81a-116">Application</span></span>|<span data-ttu-id="2c81a-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c81a-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c81a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c81a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2c81a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2c81a-119">Optional query parameters</span></span>
<span data-ttu-id="2c81a-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2c81a-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c81a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c81a-121">Request headers</span></span>
|<span data-ttu-id="2c81a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2c81a-122">Header</span></span>|<span data-ttu-id="2c81a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2c81a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c81a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c81a-124">Authorization</span></span>|<span data-ttu-id="2c81a-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c81a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c81a-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2c81a-126">Accept</span></span>|<span data-ttu-id="2c81a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2c81a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c81a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c81a-128">Request body</span></span>
<span data-ttu-id="2c81a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2c81a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c81a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c81a-130">Response</span></span>
<span data-ttu-id="2c81a-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceManagement](../resources/intune-remoteassistance-devicemanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c81a-131">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-remoteassistance-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c81a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c81a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c81a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c81a-133">Request</span></span>
<span data-ttu-id="2c81a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c81a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a><span data-ttu-id="2c81a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c81a-135">Response</span></span>
<span data-ttu-id="2c81a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2c81a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```




