---
title: Listar vppTokens
description: Lista propriedades e relações de objetos vppToken.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a4abf542d692595e8de8b3b8757519693461144c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42461673"
---
# <a name="list-vpptokens"></a><span data-ttu-id="5fd18-103">Listar vppTokens</span><span class="sxs-lookup"><span data-stu-id="5fd18-103">List vppTokens</span></span>

<span data-ttu-id="5fd18-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5fd18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5fd18-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5fd18-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5fd18-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5fd18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fd18-107">Lista propriedades e relações de objetos [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="5fd18-107">List properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5fd18-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5fd18-108">Prerequisites</span></span>
<span data-ttu-id="5fd18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fd18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fd18-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5fd18-111">Permission type</span></span>|<span data-ttu-id="5fd18-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5fd18-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fd18-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5fd18-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5fd18-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5fd18-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5fd18-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5fd18-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fd18-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5fd18-116">Not supported.</span></span>|
|<span data-ttu-id="5fd18-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5fd18-117">Application</span></span>|<span data-ttu-id="5fd18-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5fd18-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fd18-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5fd18-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="5fd18-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5fd18-120">Request headers</span></span>
|<span data-ttu-id="5fd18-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5fd18-121">Header</span></span>|<span data-ttu-id="5fd18-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5fd18-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fd18-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5fd18-123">Authorization</span></span>|<span data-ttu-id="5fd18-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fd18-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fd18-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5fd18-125">Accept</span></span>|<span data-ttu-id="5fd18-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5fd18-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fd18-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5fd18-127">Request body</span></span>
<span data-ttu-id="5fd18-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5fd18-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5fd18-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fd18-129">Response</span></span>
<span data-ttu-id="5fd18-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [vppToken](../resources/intune-onboarding-vpptoken.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5fd18-130">If successful, this method returns a `200 OK` response code and a collection of [vppToken](../resources/intune-onboarding-vpptoken.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fd18-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5fd18-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5fd18-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5fd18-132">Request</span></span>
<span data-ttu-id="5fd18-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5fd18-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens
```

### <a name="response"></a><span data-ttu-id="5fd18-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fd18-134">Response</span></span>
<span data-ttu-id="5fd18-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5fd18-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1264

{
  "value": [
    {
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
  ]
}
```





