---
title: Ação syncLicenses
description: Sincroniza as licenças associadas a um appleVolumePurchaseProgramToken específico
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5194165cb6760e2fb3fddc7ae703a7f9938b755f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49211457"
---
# <a name="synclicenses-action"></a><span data-ttu-id="7c43e-103">ação syncLicenses</span><span class="sxs-lookup"><span data-stu-id="7c43e-103">syncLicenses action</span></span>

<span data-ttu-id="7c43e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c43e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c43e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7c43e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c43e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c43e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c43e-107">Sincroniza as licenças associadas a um appleVolumePurchaseProgramToken específico</span><span class="sxs-lookup"><span data-stu-id="7c43e-107">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c43e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7c43e-108">Prerequisites</span></span>
<span data-ttu-id="7c43e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c43e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c43e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c43e-111">Permission type</span></span>|<span data-ttu-id="7c43e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7c43e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c43e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c43e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c43e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c43e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7c43e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c43e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c43e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c43e-116">Not supported.</span></span>|
|<span data-ttu-id="7c43e-117">Application</span><span class="sxs-lookup"><span data-stu-id="7c43e-117">Application</span></span>|<span data-ttu-id="7c43e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c43e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c43e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c43e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="7c43e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c43e-120">Request headers</span></span>
|<span data-ttu-id="7c43e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7c43e-121">Header</span></span>|<span data-ttu-id="7c43e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7c43e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c43e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c43e-123">Authorization</span></span>|<span data-ttu-id="7c43e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c43e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c43e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7c43e-125">Accept</span></span>|<span data-ttu-id="7c43e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c43e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c43e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c43e-127">Request body</span></span>
<span data-ttu-id="7c43e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7c43e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c43e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c43e-129">Response</span></span>
<span data-ttu-id="7c43e-130">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e um [vppToken](../resources/intune-onboarding-vpptoken.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c43e-130">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c43e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c43e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c43e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c43e-132">Request</span></span>
<span data-ttu-id="7c43e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c43e-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="7c43e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c43e-134">Response</span></span>
<span data-ttu-id="7c43e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c43e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




