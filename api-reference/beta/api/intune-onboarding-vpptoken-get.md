---
title: Obter vppToken
description: Ler propriedades e relações de objetos vppToken.
author: tfitzmac
ms.openlocfilehash: 983fafa0523add41b72c818dfd428aad2bdfd87b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306927"
---
# <a name="get-vpptoken"></a><span data-ttu-id="6e708-103">Obter vppToken</span><span class="sxs-lookup"><span data-stu-id="6e708-103">Get vppToken</span></span>

> <span data-ttu-id="6e708-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6e708-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e708-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6e708-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e708-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6e708-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6e708-107">Ler propriedades e relações de objetos [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="6e708-107">Read properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6e708-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6e708-108">Prerequisites</span></span>
<span data-ttu-id="6e708-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e708-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e708-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e708-111">Permission type</span></span>|<span data-ttu-id="6e708-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6e708-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e708-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e708-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e708-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e708-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6e708-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e708-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e708-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e708-116">Not supported.</span></span>|
|<span data-ttu-id="6e708-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e708-117">Application</span></span>|<span data-ttu-id="6e708-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e708-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e708-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e708-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e708-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6e708-120">Optional query parameters</span></span>
<span data-ttu-id="6e708-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6e708-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6e708-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e708-122">Request headers</span></span>
|<span data-ttu-id="6e708-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e708-123">Header</span></span>|<span data-ttu-id="6e708-124">Valor</span><span class="sxs-lookup"><span data-stu-id="6e708-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e708-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e708-125">Authorization</span></span>|<span data-ttu-id="6e708-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e708-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e708-127">Accept</span><span class="sxs-lookup"><span data-stu-id="6e708-127">Accept</span></span>|<span data-ttu-id="6e708-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6e708-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e708-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e708-129">Request body</span></span>
<span data-ttu-id="6e708-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6e708-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e708-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e708-131">Response</span></span>
<span data-ttu-id="6e708-132">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [vppToken](../resources/intune-onboarding-vpptoken.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e708-132">If successful, this method returns a `200 OK` response code and [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e708-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e708-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="6e708-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e708-134">Request</span></span>
<span data-ttu-id="6e708-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e708-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
```

### <a name="response"></a><span data-ttu-id="6e708-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e708-136">Response</span></span>
<span data-ttu-id="6e708-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e708-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1124

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
    "claimTokenManagementFromExternalMdm": true
  }
}
```





