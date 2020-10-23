---
title: Obter dataSharingConsent
description: Leia as propriedades e as relações do objeto dataSharingConsent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dcb5b6911cdd112df63115539629765d4522317f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724721"
---
# <a name="get-datasharingconsent"></a><span data-ttu-id="f280e-103">Obter dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="f280e-103">Get dataSharingConsent</span></span>

<span data-ttu-id="f280e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f280e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f280e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f280e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f280e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f280e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f280e-107">Leia as propriedades e as relações do objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="f280e-107">Read properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f280e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f280e-108">Prerequisites</span></span>
<span data-ttu-id="f280e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f280e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f280e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f280e-111">Permission type</span></span>|<span data-ttu-id="f280e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f280e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f280e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f280e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f280e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f280e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f280e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f280e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f280e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f280e-116">Not supported.</span></span>|
|<span data-ttu-id="f280e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f280e-117">Application</span></span>|<span data-ttu-id="f280e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f280e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f280e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f280e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f280e-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f280e-120">Optional query parameters</span></span>
<span data-ttu-id="f280e-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f280e-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f280e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f280e-122">Request headers</span></span>
|<span data-ttu-id="f280e-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f280e-123">Header</span></span>|<span data-ttu-id="f280e-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f280e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f280e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f280e-125">Authorization</span></span>|<span data-ttu-id="f280e-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f280e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f280e-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f280e-127">Accept</span></span>|<span data-ttu-id="f280e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f280e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f280e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f280e-129">Request body</span></span>
<span data-ttu-id="f280e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f280e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f280e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f280e-131">Response</span></span>
<span data-ttu-id="f280e-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f280e-132">If successful, this method returns a `200 OK` response code and [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f280e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f280e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f280e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f280e-134">Request</span></span>
<span data-ttu-id="f280e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f280e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

### <a name="response"></a><span data-ttu-id="f280e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f280e-136">Response</span></span>
<span data-ttu-id="f280e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f280e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





