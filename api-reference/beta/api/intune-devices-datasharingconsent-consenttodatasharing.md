---
title: Ação consentToDataSharing
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9ef22ccd05abb031ea3f109cc6bf28ba6f7d21a7
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945239"
---
# <a name="consenttodatasharing-action"></a><span data-ttu-id="fd6ff-103">Ação consentToDataSharing</span><span class="sxs-lookup"><span data-stu-id="fd6ff-103">consentToDataSharing action</span></span>

> <span data-ttu-id="fd6ff-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fd6ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd6ff-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fd6ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd6ff-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fd6ff-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd6ff-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fd6ff-107">Prerequisites</span></span>
<span data-ttu-id="fd6ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd6ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd6ff-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd6ff-110">Permission type</span></span>|<span data-ttu-id="fd6ff-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fd6ff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd6ff-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd6ff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fd6ff-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd6ff-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fd6ff-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd6ff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd6ff-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd6ff-115">Not supported.</span></span>|
|<span data-ttu-id="fd6ff-116">Application</span><span class="sxs-lookup"><span data-stu-id="fd6ff-116">Application</span></span>|<span data-ttu-id="fd6ff-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd6ff-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd6ff-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd6ff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents/{dataSharingConsentId}/consentToDataSharing
```

## <a name="request-headers"></a><span data-ttu-id="fd6ff-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd6ff-119">Request headers</span></span>
|<span data-ttu-id="fd6ff-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fd6ff-120">Header</span></span>|<span data-ttu-id="fd6ff-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fd6ff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd6ff-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd6ff-122">Authorization</span></span>|<span data-ttu-id="fd6ff-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd6ff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd6ff-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fd6ff-124">Accept</span></span>|<span data-ttu-id="fd6ff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fd6ff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd6ff-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd6ff-126">Request body</span></span>
<span data-ttu-id="fd6ff-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fd6ff-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd6ff-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd6ff-128">Response</span></span>
<span data-ttu-id="fd6ff-129">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e um [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd6ff-129">If successful, this action returns a `200 OK` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd6ff-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd6ff-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd6ff-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd6ff-131">Request</span></span>
<span data-ttu-id="fd6ff-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd6ff-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}/consentToDataSharing
```

### <a name="response"></a><span data-ttu-id="fd6ff-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd6ff-133">Response</span></span>
<span data-ttu-id="fd6ff-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd6ff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 417

{
  "value": {
    "@odata.type": "#microsoft.graph.dataSharingConsent",
    "id": "333387f7-87f7-3333-f787-3333f7873333",
    "serviceDisplayName": "Service Display Name value",
    "termsUrl": "https://example.com/termsUrl/",
    "granted": true,
    "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
    "grantedByUpn": "Granted By Upn value",
    "grantedByUserId": "Granted By User Id value"
  }
}
```





