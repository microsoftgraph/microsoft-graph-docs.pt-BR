---
title: Ação syncLicenses
description: Sincroniza as licenças associadas a um appleVolumePurchaseProgramToken específico
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 79660c8de56cdf449d3fd407767bed37245ceb2c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414274"
---
# <a name="synclicenses-action"></a><span data-ttu-id="67f00-103">Ação syncLicenses</span><span class="sxs-lookup"><span data-stu-id="67f00-103">syncLicenses action</span></span>

> <span data-ttu-id="67f00-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="67f00-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="67f00-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="67f00-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67f00-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="67f00-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67f00-107">Sincroniza as licenças associadas a um appleVolumePurchaseProgramToken específico</span><span class="sxs-lookup"><span data-stu-id="67f00-107">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67f00-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67f00-108">Prerequisites</span></span>
<span data-ttu-id="67f00-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="67f00-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="67f00-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67f00-111">Permission type</span></span>|<span data-ttu-id="67f00-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="67f00-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67f00-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67f00-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67f00-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67f00-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="67f00-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67f00-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67f00-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67f00-116">Not supported.</span></span>|
|<span data-ttu-id="67f00-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67f00-117">Application</span></span>|<span data-ttu-id="67f00-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67f00-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67f00-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67f00-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="67f00-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67f00-120">Request headers</span></span>
|<span data-ttu-id="67f00-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67f00-121">Header</span></span>|<span data-ttu-id="67f00-122">Valor</span><span class="sxs-lookup"><span data-stu-id="67f00-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67f00-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="67f00-123">Authorization</span></span>|<span data-ttu-id="67f00-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67f00-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67f00-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67f00-125">Accept</span></span>|<span data-ttu-id="67f00-126">application/json</span><span class="sxs-lookup"><span data-stu-id="67f00-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67f00-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67f00-127">Request body</span></span>
<span data-ttu-id="67f00-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="67f00-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67f00-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="67f00-129">Response</span></span>
<span data-ttu-id="67f00-130">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e um [vppToken](../resources/intune-onboarding-vpptoken.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67f00-130">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67f00-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67f00-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="67f00-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67f00-132">Request</span></span>
<span data-ttu-id="67f00-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67f00-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="67f00-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="67f00-134">Response</span></span>
<span data-ttu-id="67f00-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67f00-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




