---
title: Ação syncLicenses
description: Sincroniza as licenças associadas a um appleVolumePurchaseProgramToken específico
ms.openlocfilehash: 36b0e141c398b17319711753928312a1353d2ab5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038843"
---
# <a name="synclicenses-action"></a><span data-ttu-id="bf89e-103">Ação syncLicenses</span><span class="sxs-lookup"><span data-stu-id="bf89e-103">syncLicenses action</span></span>

> <span data-ttu-id="bf89e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bf89e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf89e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bf89e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf89e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bf89e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf89e-107">Sincroniza as licenças associadas a um appleVolumePurchaseProgramToken específico</span><span class="sxs-lookup"><span data-stu-id="bf89e-107">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bf89e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bf89e-108">Prerequisites</span></span>
<span data-ttu-id="bf89e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf89e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf89e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf89e-111">Permission type</span></span>|<span data-ttu-id="bf89e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bf89e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf89e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf89e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bf89e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf89e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bf89e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf89e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf89e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf89e-116">Not supported.</span></span>|
|<span data-ttu-id="bf89e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf89e-117">Application</span></span>|<span data-ttu-id="bf89e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf89e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf89e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf89e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="bf89e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf89e-120">Request headers</span></span>
|<span data-ttu-id="bf89e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bf89e-121">Header</span></span>|<span data-ttu-id="bf89e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bf89e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf89e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf89e-123">Authorization</span></span>|<span data-ttu-id="bf89e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf89e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf89e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bf89e-125">Accept</span></span>|<span data-ttu-id="bf89e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bf89e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf89e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf89e-127">Request body</span></span>
<span data-ttu-id="bf89e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bf89e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf89e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf89e-129">Response</span></span>
<span data-ttu-id="bf89e-130">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e um [vppToken](../resources/intune-onboarding-vpptoken.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf89e-130">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf89e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf89e-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="bf89e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf89e-132">Request</span></span>
<span data-ttu-id="bf89e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf89e-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="bf89e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf89e-134">Response</span></span>
<span data-ttu-id="bf89e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bf89e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





