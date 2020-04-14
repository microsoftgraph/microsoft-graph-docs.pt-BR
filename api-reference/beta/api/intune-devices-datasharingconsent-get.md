---
title: Obter dataSharingConsent
description: Leia as propriedades e as relações do objeto dataSharingConsent.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1d182694ac86188e4db52c4aede31a39d31276d6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43426671"
---
# <a name="get-datasharingconsent"></a><span data-ttu-id="f00ae-103">Obter dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="f00ae-103">Get dataSharingConsent</span></span>

<span data-ttu-id="f00ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f00ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f00ae-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f00ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f00ae-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f00ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f00ae-107">Leia as propriedades e as relações do objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="f00ae-107">Read properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f00ae-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f00ae-108">Prerequisites</span></span>
<span data-ttu-id="f00ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f00ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f00ae-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f00ae-111">Permission type</span></span>|<span data-ttu-id="f00ae-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f00ae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f00ae-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f00ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f00ae-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f00ae-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f00ae-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f00ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f00ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f00ae-116">Not supported.</span></span>|
|<span data-ttu-id="f00ae-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f00ae-117">Application</span></span>|<span data-ttu-id="f00ae-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f00ae-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f00ae-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f00ae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f00ae-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f00ae-120">Optional query parameters</span></span>
<span data-ttu-id="f00ae-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f00ae-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f00ae-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f00ae-122">Request headers</span></span>
|<span data-ttu-id="f00ae-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f00ae-123">Header</span></span>|<span data-ttu-id="f00ae-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f00ae-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f00ae-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f00ae-125">Authorization</span></span>|<span data-ttu-id="f00ae-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f00ae-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f00ae-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f00ae-127">Accept</span></span>|<span data-ttu-id="f00ae-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f00ae-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f00ae-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f00ae-129">Request body</span></span>
<span data-ttu-id="f00ae-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f00ae-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f00ae-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f00ae-131">Response</span></span>
<span data-ttu-id="f00ae-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f00ae-132">If successful, this method returns a `200 OK` response code and [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f00ae-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f00ae-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f00ae-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f00ae-134">Request</span></span>
<span data-ttu-id="f00ae-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f00ae-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

### <a name="response"></a><span data-ttu-id="f00ae-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f00ae-136">Response</span></span>
<span data-ttu-id="f00ae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f00ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



