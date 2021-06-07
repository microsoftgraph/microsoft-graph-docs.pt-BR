---
title: Ação syncLicenses
description: Sincroniza as licenças associadas a um appleVolumePurchaseProgramToken específico
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dcd9139bf2d2ca3c7baffbd34fedc064402192f5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759041"
---
# <a name="synclicenses-action"></a><span data-ttu-id="43b63-103">ação syncLicenses</span><span class="sxs-lookup"><span data-stu-id="43b63-103">syncLicenses action</span></span>

<span data-ttu-id="43b63-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43b63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43b63-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="43b63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43b63-106">Sincroniza as licenças associadas a um appleVolumePurchaseProgramToken específico</span><span class="sxs-lookup"><span data-stu-id="43b63-106">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43b63-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="43b63-107">Prerequisites</span></span>
<span data-ttu-id="43b63-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43b63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43b63-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43b63-110">Permission type</span></span>|<span data-ttu-id="43b63-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43b63-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43b63-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43b63-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43b63-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43b63-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="43b63-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43b63-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43b63-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43b63-115">Not supported.</span></span>|
|<span data-ttu-id="43b63-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43b63-116">Application</span></span>|<span data-ttu-id="43b63-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43b63-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43b63-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43b63-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="43b63-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43b63-119">Request headers</span></span>
|<span data-ttu-id="43b63-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43b63-120">Header</span></span>|<span data-ttu-id="43b63-121">Valor</span><span class="sxs-lookup"><span data-stu-id="43b63-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43b63-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="43b63-122">Authorization</span></span>|<span data-ttu-id="43b63-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43b63-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43b63-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="43b63-124">Accept</span></span>|<span data-ttu-id="43b63-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43b63-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43b63-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43b63-126">Request body</span></span>
<span data-ttu-id="43b63-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="43b63-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43b63-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="43b63-128">Response</span></span>
<span data-ttu-id="43b63-129">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e um [vppToken](../resources/intune-onboarding-vpptoken.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43b63-129">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43b63-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43b63-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="43b63-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43b63-131">Request</span></span>
<span data-ttu-id="43b63-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="43b63-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="43b63-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="43b63-133">Response</span></span>
<span data-ttu-id="43b63-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43b63-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




