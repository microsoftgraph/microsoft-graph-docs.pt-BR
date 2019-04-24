---
title: Obter dataSharingConsent
description: Leia as propriedades e as relações do objeto dataSharingConsent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 816f87b3345fb925e148ff794da16caff3647b50
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465969"
---
# <a name="get-datasharingconsent"></a><span data-ttu-id="63f1a-103">Obter dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="63f1a-103">Get dataSharingConsent</span></span>

> <span data-ttu-id="63f1a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="63f1a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63f1a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63f1a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63f1a-106">Leia as propriedades e as relações do objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="63f1a-106">Read properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63f1a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63f1a-107">Prerequisites</span></span>
<span data-ttu-id="63f1a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63f1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63f1a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63f1a-110">Permission type</span></span>|<span data-ttu-id="63f1a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="63f1a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63f1a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63f1a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="63f1a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63f1a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="63f1a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63f1a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63f1a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63f1a-115">Not supported.</span></span>|
|<span data-ttu-id="63f1a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63f1a-116">Application</span></span>|<span data-ttu-id="63f1a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63f1a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63f1a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63f1a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="63f1a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="63f1a-119">Optional query parameters</span></span>
<span data-ttu-id="63f1a-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="63f1a-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="63f1a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63f1a-121">Request headers</span></span>
|<span data-ttu-id="63f1a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63f1a-122">Header</span></span>|<span data-ttu-id="63f1a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="63f1a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63f1a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="63f1a-124">Authorization</span></span>|<span data-ttu-id="63f1a-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63f1a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63f1a-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="63f1a-126">Accept</span></span>|<span data-ttu-id="63f1a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="63f1a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63f1a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63f1a-128">Request body</span></span>
<span data-ttu-id="63f1a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="63f1a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63f1a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="63f1a-130">Response</span></span>
<span data-ttu-id="63f1a-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63f1a-131">If successful, this method returns a `200 OK` response code and [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63f1a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63f1a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="63f1a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63f1a-133">Request</span></span>
<span data-ttu-id="63f1a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63f1a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

### <a name="response"></a><span data-ttu-id="63f1a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="63f1a-135">Response</span></span>
<span data-ttu-id="63f1a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63f1a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





