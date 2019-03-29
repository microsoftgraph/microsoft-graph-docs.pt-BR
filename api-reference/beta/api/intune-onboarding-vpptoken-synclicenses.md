---
title: Ação syncLicenses
description: Sincroniza as licenças associadas a um appleVolumePurchaseProgramToken específico
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fafcb15fb6911cf1c8ec7c25284ac95f6d848408
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968963"
---
# <a name="synclicenses-action"></a><span data-ttu-id="6c698-103">ação syncLicenses</span><span class="sxs-lookup"><span data-stu-id="6c698-103">syncLicenses action</span></span>

> <span data-ttu-id="6c698-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c698-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c698-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c698-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c698-106">Sincroniza as licenças associadas a um appleVolumePurchaseProgramToken específico</span><span class="sxs-lookup"><span data-stu-id="6c698-106">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c698-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6c698-107">Prerequisites</span></span>
<span data-ttu-id="6c698-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c698-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c698-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c698-110">Permission type</span></span>|<span data-ttu-id="6c698-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6c698-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c698-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c698-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c698-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c698-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6c698-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c698-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c698-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c698-115">Not supported.</span></span>|
|<span data-ttu-id="6c698-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c698-116">Application</span></span>|<span data-ttu-id="6c698-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c698-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c698-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c698-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="6c698-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c698-119">Request headers</span></span>
|<span data-ttu-id="6c698-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c698-120">Header</span></span>|<span data-ttu-id="6c698-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6c698-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c698-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c698-122">Authorization</span></span>|<span data-ttu-id="6c698-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c698-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c698-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6c698-124">Accept</span></span>|<span data-ttu-id="6c698-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6c698-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c698-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c698-126">Request body</span></span>
<span data-ttu-id="6c698-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6c698-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c698-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c698-128">Response</span></span>
<span data-ttu-id="6c698-129">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e um [vppToken](../resources/intune-onboarding-vpptoken.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c698-129">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c698-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c698-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c698-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c698-131">Request</span></span>
<span data-ttu-id="6c698-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c698-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="6c698-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c698-133">Response</span></span>
<span data-ttu-id="6c698-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c698-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




