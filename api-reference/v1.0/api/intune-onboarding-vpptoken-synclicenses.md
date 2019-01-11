---
title: Ação syncLicenses
description: Sincroniza as licenças associadas a um appleVolumePurchaseProgramToken específico
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0c81fa85d2b884bc40c580b19635f453645c66af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851041"
---
# <a name="synclicenses-action"></a><span data-ttu-id="3ad87-103">Ação syncLicenses</span><span class="sxs-lookup"><span data-stu-id="3ad87-103">syncLicenses action</span></span>

> <span data-ttu-id="3ad87-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3ad87-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3ad87-105">Sincroniza as licenças associadas a um appleVolumePurchaseProgramToken específico</span><span class="sxs-lookup"><span data-stu-id="3ad87-105">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3ad87-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3ad87-106">Prerequisites</span></span>
<span data-ttu-id="3ad87-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ad87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ad87-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ad87-109">Permission type</span></span>|<span data-ttu-id="3ad87-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3ad87-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ad87-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ad87-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3ad87-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ad87-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3ad87-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ad87-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ad87-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ad87-114">Not supported.</span></span>|
|<span data-ttu-id="3ad87-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ad87-115">Application</span></span>|<span data-ttu-id="3ad87-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ad87-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ad87-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ad87-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="3ad87-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ad87-118">Request headers</span></span>
|<span data-ttu-id="3ad87-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3ad87-119">Header</span></span>|<span data-ttu-id="3ad87-120">Valor</span><span class="sxs-lookup"><span data-stu-id="3ad87-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ad87-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ad87-121">Authorization</span></span>|<span data-ttu-id="3ad87-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ad87-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ad87-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3ad87-123">Accept</span></span>|<span data-ttu-id="3ad87-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3ad87-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ad87-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ad87-125">Request body</span></span>
<span data-ttu-id="3ad87-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3ad87-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ad87-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ad87-127">Response</span></span>
<span data-ttu-id="3ad87-128">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e um [vppToken](../resources/intune-onboarding-vpptoken.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ad87-128">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ad87-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ad87-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="3ad87-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ad87-130">Request</span></span>
<span data-ttu-id="3ad87-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ad87-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="3ad87-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ad87-132">Response</span></span>
<span data-ttu-id="3ad87-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ad87-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 619

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
    "lastSyncStatus": "inProgress",
    "automaticallyUpdateApps": true,
    "countryOrRegion": "Country Or Region value"
  }
}
```



