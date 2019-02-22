---
title: Listar remoteAssistancePartners
description: Listar propriedades e relações de objetos de remoteAssistancePartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e320f3fedcb8c17329b199e5213b42522a349889
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141983"
---
# <a name="list-remoteassistancepartners"></a><span data-ttu-id="bb664-103">Listar remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="bb664-103">List remoteAssistancePartners</span></span>

> <span data-ttu-id="bb664-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bb664-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb664-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb664-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb664-106">Listar propriedades e relações de objetos de [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="bb664-106">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb664-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bb664-107">Prerequisites</span></span>
<span data-ttu-id="bb664-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bb664-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bb664-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb664-110">Permission type</span></span>|<span data-ttu-id="bb664-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bb664-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb664-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb664-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bb664-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb664-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="bb664-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb664-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb664-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb664-115">Not supported.</span></span>|
|<span data-ttu-id="bb664-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb664-116">Application</span></span>|<span data-ttu-id="bb664-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb664-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb664-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb664-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="bb664-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb664-119">Request headers</span></span>
|<span data-ttu-id="bb664-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bb664-120">Header</span></span>|<span data-ttu-id="bb664-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bb664-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb664-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb664-122">Authorization</span></span>|<span data-ttu-id="bb664-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb664-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb664-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bb664-124">Accept</span></span>|<span data-ttu-id="bb664-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bb664-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb664-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb664-126">Request body</span></span>
<span data-ttu-id="bb664-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bb664-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb664-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb664-128">Response</span></span>
<span data-ttu-id="bb664-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb664-129">If successful, this method returns a `200 OK` response code and a collection of [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb664-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb664-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb664-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb664-131">Request</span></span>
<span data-ttu-id="bb664-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb664-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners
```

### <a name="response"></a><span data-ttu-id="bb664-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb664-133">Response</span></span>
<span data-ttu-id="bb664-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb664-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




