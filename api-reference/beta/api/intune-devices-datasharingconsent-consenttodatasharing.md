---
title: Ação consentToDataSharing
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 848deb8f7b7f9b0b28873cce0e3058e6582bfbaa
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154431"
---
# <a name="consenttodatasharing-action"></a><span data-ttu-id="4d2e6-103">Ação consentToDataSharing</span><span class="sxs-lookup"><span data-stu-id="4d2e6-103">consentToDataSharing action</span></span>

<span data-ttu-id="4d2e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d2e6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d2e6-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4d2e6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d2e6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4d2e6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d2e6-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4d2e6-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d2e6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4d2e6-108">Prerequisites</span></span>
<span data-ttu-id="4d2e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d2e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d2e6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d2e6-111">Permission type</span></span>|<span data-ttu-id="4d2e6-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d2e6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d2e6-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d2e6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4d2e6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d2e6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4d2e6-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d2e6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d2e6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d2e6-116">Not supported.</span></span>|
|<span data-ttu-id="4d2e6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d2e6-117">Application</span></span>|<span data-ttu-id="4d2e6-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d2e6-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d2e6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d2e6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents/{dataSharingConsentId}/consentToDataSharing
```

## <a name="request-headers"></a><span data-ttu-id="4d2e6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d2e6-120">Request headers</span></span>
|<span data-ttu-id="4d2e6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4d2e6-121">Header</span></span>|<span data-ttu-id="4d2e6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4d2e6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d2e6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d2e6-123">Authorization</span></span>|<span data-ttu-id="4d2e6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d2e6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d2e6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4d2e6-125">Accept</span></span>|<span data-ttu-id="4d2e6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d2e6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d2e6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d2e6-127">Request body</span></span>
<span data-ttu-id="4d2e6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4d2e6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d2e6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d2e6-129">Response</span></span>
<span data-ttu-id="4d2e6-130">Se tiver êxito, essa ação retornará um código de resposta e um `200 OK` [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d2e6-130">If successful, this action returns a `200 OK` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d2e6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d2e6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d2e6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d2e6-132">Request</span></span>
<span data-ttu-id="4d2e6-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d2e6-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}/consentToDataSharing
```

### <a name="response"></a><span data-ttu-id="4d2e6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d2e6-134">Response</span></span>
<span data-ttu-id="4d2e6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d2e6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




