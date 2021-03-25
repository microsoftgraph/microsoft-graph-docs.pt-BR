---
title: Obter mobileAppIntentAndState
description: Ler propriedades e relações do objeto mobileAppIntentAndState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d71c3ab2615285594d1025f4c799b16bc584309d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151834"
---
# <a name="get-mobileappintentandstate"></a><span data-ttu-id="d2bad-103">Obter mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="d2bad-103">Get mobileAppIntentAndState</span></span>

<span data-ttu-id="d2bad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2bad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2bad-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d2bad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2bad-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d2bad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2bad-107">Ler propriedades e relações do [objeto mobileAppIntentAndState.](../resources/intune-troubleshooting-mobileappintentandstate.md)</span><span class="sxs-lookup"><span data-stu-id="d2bad-107">Read properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2bad-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d2bad-108">Prerequisites</span></span>
<span data-ttu-id="d2bad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2bad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2bad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2bad-111">Permission type</span></span>|<span data-ttu-id="d2bad-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2bad-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2bad-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2bad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2bad-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2bad-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d2bad-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2bad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2bad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2bad-116">Not supported.</span></span>|
|<span data-ttu-id="d2bad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2bad-117">Application</span></span>|<span data-ttu-id="d2bad-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2bad-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2bad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2bad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2bad-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d2bad-120">Optional query parameters</span></span>
<span data-ttu-id="d2bad-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d2bad-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2bad-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2bad-122">Request headers</span></span>
|<span data-ttu-id="d2bad-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d2bad-123">Header</span></span>|<span data-ttu-id="d2bad-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d2bad-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2bad-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2bad-125">Authorization</span></span>|<span data-ttu-id="d2bad-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2bad-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2bad-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d2bad-127">Accept</span></span>|<span data-ttu-id="d2bad-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d2bad-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2bad-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2bad-129">Request body</span></span>
<span data-ttu-id="d2bad-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d2bad-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2bad-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2bad-131">Response</span></span>
<span data-ttu-id="d2bad-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2bad-132">If successful, this method returns a `200 OK` response code and [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2bad-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2bad-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2bad-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2bad-134">Request</span></span>
<span data-ttu-id="d2bad-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2bad-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

### <a name="response"></a><span data-ttu-id="d2bad-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2bad-136">Response</span></span>
<span data-ttu-id="d2bad-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2bad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 943

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
    "id": "45a775d6-75d6-45a7-d675-a745d675a745",
    "managedDeviceIdentifier": "Managed Device Identifier value",
    "userId": "User Id value",
    "mobileAppList": [
      {
        "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
        "applicationId": "Application Id value",
        "displayName": "Display Name value",
        "mobileAppIntent": "notAvailable",
        "displayVersion": "Display Version value",
        "installState": "failed",
        "supportedDeviceTypes": [
          {
            "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
            "type": "windowsRT",
            "minimumOperatingSystemVersion": "Minimum Operating System Version value",
            "maximumOperatingSystemVersion": "Maximum Operating System Version value"
          }
        ]
      }
    ]
  }
}
```




