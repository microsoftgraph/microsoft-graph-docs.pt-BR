---
title: Ação syncLicenses
description: Sincroniza as licenças associadas a um appleVolumePurchaseProgramToken específico
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a6e6aaed7260754ca1a9e5da9bd90b24a2519a9c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933138"
---
# <a name="synclicenses-action"></a><span data-ttu-id="cf654-103">Ação syncLicenses</span><span class="sxs-lookup"><span data-stu-id="cf654-103">syncLicenses action</span></span>

> <span data-ttu-id="cf654-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cf654-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf654-105">Sincroniza as licenças associadas a um appleVolumePurchaseProgramToken específico</span><span class="sxs-lookup"><span data-stu-id="cf654-105">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf654-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf654-106">Prerequisites</span></span>
<span data-ttu-id="cf654-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf654-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf654-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf654-109">Permission type</span></span>|<span data-ttu-id="cf654-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cf654-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf654-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf654-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cf654-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf654-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cf654-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf654-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf654-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf654-114">Not supported.</span></span>|
|<span data-ttu-id="cf654-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf654-115">Application</span></span>|<span data-ttu-id="cf654-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf654-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf654-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf654-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="cf654-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf654-118">Request headers</span></span>
|<span data-ttu-id="cf654-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf654-119">Header</span></span>|<span data-ttu-id="cf654-120">Valor</span><span class="sxs-lookup"><span data-stu-id="cf654-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf654-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf654-121">Authorization</span></span>|<span data-ttu-id="cf654-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf654-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf654-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cf654-123">Accept</span></span>|<span data-ttu-id="cf654-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cf654-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf654-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf654-125">Request body</span></span>
<span data-ttu-id="cf654-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cf654-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf654-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf654-127">Response</span></span>
<span data-ttu-id="cf654-128">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e um [vppToken](../resources/intune-onboarding-vpptoken.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf654-128">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf654-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf654-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf654-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf654-130">Request</span></span>
<span data-ttu-id="cf654-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf654-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="cf654-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf654-132">Response</span></span>
<span data-ttu-id="cf654-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf654-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



