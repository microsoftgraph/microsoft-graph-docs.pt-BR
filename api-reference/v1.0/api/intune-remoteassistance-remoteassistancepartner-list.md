---
title: Listar remoteAssistancePartners
description: Listar propriedades e relações de objetos de remoteAssistancePartner.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 24992a39c9e7d0ed204455f0ae6387859a910bf7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512143"
---
# <a name="list-remoteassistancepartners"></a><span data-ttu-id="7b0f0-103">Listar remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="7b0f0-103">List remoteAssistancePartners</span></span>

<span data-ttu-id="7b0f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b0f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b0f0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7b0f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b0f0-106">Listar propriedades e relações de objetos de [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="7b0f0-106">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b0f0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7b0f0-107">Prerequisites</span></span>
<span data-ttu-id="7b0f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b0f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b0f0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b0f0-110">Permission type</span></span>|<span data-ttu-id="7b0f0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7b0f0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b0f0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b0f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7b0f0-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b0f0-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="7b0f0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b0f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b0f0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b0f0-115">Not supported.</span></span>|
|<span data-ttu-id="7b0f0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b0f0-116">Application</span></span>|<span data-ttu-id="7b0f0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b0f0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b0f0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b0f0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="7b0f0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b0f0-119">Request headers</span></span>
|<span data-ttu-id="7b0f0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7b0f0-120">Header</span></span>|<span data-ttu-id="7b0f0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7b0f0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b0f0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b0f0-122">Authorization</span></span>|<span data-ttu-id="7b0f0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b0f0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b0f0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7b0f0-124">Accept</span></span>|<span data-ttu-id="7b0f0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7b0f0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b0f0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b0f0-126">Request body</span></span>
<span data-ttu-id="7b0f0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7b0f0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b0f0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b0f0-128">Response</span></span>
<span data-ttu-id="7b0f0-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b0f0-129">If successful, this method returns a `200 OK` response code and a collection of [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b0f0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b0f0-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b0f0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b0f0-131">Request</span></span>
<span data-ttu-id="7b0f0-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b0f0-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners
```

### <a name="response"></a><span data-ttu-id="7b0f0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b0f0-133">Response</span></span>
<span data-ttu-id="7b0f0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7b0f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.remoteAssistancePartner",
      "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
      "displayName": "Display Name value",
      "onboardingUrl": "https://example.com/onboardingUrl/",
      "onboardingStatus": "onboarding",
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
    }
  ]
}
```




