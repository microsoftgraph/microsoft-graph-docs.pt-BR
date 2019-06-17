---
title: Acessar remoteAssistancePartner
description: Leia as propriedades e as relações do objeto remoteAssistancePartner.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 959692d93ef7710fa1d687f0f522c40d42afe4a3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989627"
---
# <a name="get-remoteassistancepartner"></a><span data-ttu-id="17921-103">Acessar remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="17921-103">Get remoteAssistancePartner</span></span>

> <span data-ttu-id="17921-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="17921-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17921-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="17921-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17921-106">Leia as propriedades e as relações do objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="17921-106">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17921-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="17921-107">Prerequisites</span></span>
<span data-ttu-id="17921-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17921-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17921-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17921-110">Permission type</span></span>|<span data-ttu-id="17921-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="17921-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17921-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17921-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17921-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="17921-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="17921-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17921-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17921-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17921-115">Not supported.</span></span>|
|<span data-ttu-id="17921-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17921-116">Application</span></span>|<span data-ttu-id="17921-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17921-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17921-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17921-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="17921-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="17921-119">Optional query parameters</span></span>
<span data-ttu-id="17921-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="17921-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="17921-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17921-121">Request headers</span></span>
|<span data-ttu-id="17921-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17921-122">Header</span></span>|<span data-ttu-id="17921-123">Valor</span><span class="sxs-lookup"><span data-stu-id="17921-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17921-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="17921-124">Authorization</span></span>|<span data-ttu-id="17921-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17921-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17921-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="17921-126">Accept</span></span>|<span data-ttu-id="17921-127">application/json</span><span class="sxs-lookup"><span data-stu-id="17921-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17921-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17921-128">Request body</span></span>
<span data-ttu-id="17921-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="17921-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17921-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="17921-130">Response</span></span>
<span data-ttu-id="17921-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17921-131">If successful, this method returns a `200 OK` response code and [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17921-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17921-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="17921-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17921-133">Request</span></span>
<span data-ttu-id="17921-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17921-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

### <a name="response"></a><span data-ttu-id="17921-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="17921-135">Response</span></span>
<span data-ttu-id="17921-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17921-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
    "@odata.type": "#microsoft.graph.remoteAssistancePartner",
    "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
    "displayName": "Display Name value",
    "onboardingUrl": "https://example.com/onboardingUrl/",
    "onboardingStatus": "onboarding",
    "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
  }
}
```





