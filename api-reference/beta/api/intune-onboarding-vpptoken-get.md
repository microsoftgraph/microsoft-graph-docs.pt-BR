---
title: Obter vppToken
description: Ler propriedades e relações de objetos vppToken.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0105078e9f60806cae28d99741e7b1a8da9d0897
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48047284"
---
# <a name="get-vpptoken"></a><span data-ttu-id="0c4be-103">Obter vppToken</span><span class="sxs-lookup"><span data-stu-id="0c4be-103">Get vppToken</span></span>

<span data-ttu-id="0c4be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c4be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c4be-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0c4be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c4be-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c4be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c4be-107">Ler propriedades e relações de objetos [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="0c4be-107">Read properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c4be-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c4be-108">Prerequisites</span></span>
<span data-ttu-id="0c4be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c4be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c4be-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c4be-111">Permission type</span></span>|<span data-ttu-id="0c4be-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0c4be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c4be-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c4be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c4be-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c4be-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="0c4be-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c4be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c4be-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c4be-116">Not supported.</span></span>|
|<span data-ttu-id="0c4be-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c4be-117">Application</span></span>|<span data-ttu-id="0c4be-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c4be-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c4be-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c4be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0c4be-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0c4be-120">Optional query parameters</span></span>
<span data-ttu-id="0c4be-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0c4be-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c4be-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c4be-122">Request headers</span></span>
|<span data-ttu-id="0c4be-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c4be-123">Header</span></span>|<span data-ttu-id="0c4be-124">Valor</span><span class="sxs-lookup"><span data-stu-id="0c4be-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c4be-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c4be-125">Authorization</span></span>|<span data-ttu-id="0c4be-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c4be-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c4be-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0c4be-127">Accept</span></span>|<span data-ttu-id="0c4be-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0c4be-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c4be-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c4be-129">Request body</span></span>
<span data-ttu-id="0c4be-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0c4be-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c4be-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c4be-131">Response</span></span>
<span data-ttu-id="0c4be-132">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [vppToken](../resources/intune-onboarding-vpptoken.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c4be-132">If successful, this method returns a `200 OK` response code and [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c4be-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c4be-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c4be-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c4be-134">Request</span></span>
<span data-ttu-id="0c4be-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c4be-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
```

### <a name="response"></a><span data-ttu-id="0c4be-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c4be-136">Response</span></span>
<span data-ttu-id="0c4be-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c4be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1192

{
  "value": {
    "@odata.type": "#microsoft.graph.vppToken",
    "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
    "organizationName": "Organization Name value",
    "vppTokenAccountType": "education",
    "appleId": "Apple Id value",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "token": "Token value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "state": "valid",
    "tokenActionResults": [
      {
        "@odata.type": "microsoft.graph.vppTokenActionResult",
        "actionName": "Action Name value",
        "actionState": "pending",
        "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
        "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
      }
    ],
    "lastSyncStatus": "inProgress",
    "automaticallyUpdateApps": true,
    "countryOrRegion": "Country Or Region value",
    "dataSharingConsentGranted": true,
    "displayName": "Display Name value",
    "locationName": "Location Name value",
    "claimTokenManagementFromExternalMdm": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```






