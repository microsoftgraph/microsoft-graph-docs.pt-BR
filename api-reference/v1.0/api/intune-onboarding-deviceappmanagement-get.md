---
title: Get deviceAppManagement
description: Ler propriedades e relações do objeto deviceAppManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 110d36cc1271ed8b3c056bf5204740508ba6e21a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52748922"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="70272-103">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="70272-103">Get deviceAppManagement</span></span>

<span data-ttu-id="70272-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70272-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="70272-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="70272-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70272-106">Ler propriedades e relações do objeto [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="70272-106">Read properties and relationships of the [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70272-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="70272-107">Prerequisites</span></span>
<span data-ttu-id="70272-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70272-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70272-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70272-110">Permission type</span></span>|<span data-ttu-id="70272-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="70272-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70272-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70272-112">Delegated (work or school account)</span></span>|<span data-ttu-id="70272-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70272-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="70272-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70272-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70272-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70272-115">Not supported.</span></span>|
|<span data-ttu-id="70272-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70272-116">Application</span></span>|<span data-ttu-id="70272-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70272-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="70272-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70272-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="70272-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="70272-119">Optional query parameters</span></span>
<span data-ttu-id="70272-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="70272-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70272-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70272-121">Request headers</span></span>
|<span data-ttu-id="70272-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="70272-122">Header</span></span>|<span data-ttu-id="70272-123">Valor</span><span class="sxs-lookup"><span data-stu-id="70272-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70272-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="70272-124">Authorization</span></span>|<span data-ttu-id="70272-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70272-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70272-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="70272-126">Accept</span></span>|<span data-ttu-id="70272-127">application/json</span><span class="sxs-lookup"><span data-stu-id="70272-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70272-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70272-128">Request body</span></span>
<span data-ttu-id="70272-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="70272-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70272-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="70272-130">Response</span></span>
<span data-ttu-id="70272-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70272-131">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70272-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70272-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="70272-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70272-133">Request</span></span>
<span data-ttu-id="70272-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="70272-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="70272-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="70272-135">Response</span></span>
<span data-ttu-id="70272-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70272-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 474

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb",
    "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:57:45.2453148-08:00",
    "isEnabledForMicrosoftStoreForBusiness": true,
    "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
    "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:02:00.0421137-08:00"
  }
}
```




