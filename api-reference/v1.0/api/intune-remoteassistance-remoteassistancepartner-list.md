---
title: Listar remoteAssistancePartners
description: Listar propriedades e relações de objetos de remoteAssistancePartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae6350fd7d519991d8741d2f90350c1b7ee08201
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987024"
---
# <a name="list-remoteassistancepartners"></a><span data-ttu-id="e6c45-103">Listar remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="e6c45-103">List remoteAssistancePartners</span></span>

> <span data-ttu-id="e6c45-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6c45-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6c45-105">Listar propriedades e relações de objetos de [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="e6c45-105">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6c45-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e6c45-106">Prerequisites</span></span>
<span data-ttu-id="e6c45-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6c45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6c45-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6c45-109">Permission type</span></span>|<span data-ttu-id="e6c45-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e6c45-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6c45-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6c45-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e6c45-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6c45-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e6c45-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6c45-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6c45-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6c45-114">Not supported.</span></span>|
|<span data-ttu-id="e6c45-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6c45-115">Application</span></span>|<span data-ttu-id="e6c45-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6c45-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6c45-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6c45-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="e6c45-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6c45-118">Request headers</span></span>
|<span data-ttu-id="e6c45-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e6c45-119">Header</span></span>|<span data-ttu-id="e6c45-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e6c45-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6c45-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6c45-121">Authorization</span></span>|<span data-ttu-id="e6c45-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6c45-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6c45-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e6c45-123">Accept</span></span>|<span data-ttu-id="e6c45-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e6c45-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6c45-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6c45-125">Request body</span></span>
<span data-ttu-id="e6c45-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e6c45-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6c45-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6c45-127">Response</span></span>
<span data-ttu-id="e6c45-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6c45-128">If successful, this method returns a `200 OK` response code and a collection of [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6c45-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6c45-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6c45-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6c45-130">Request</span></span>
<span data-ttu-id="e6c45-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6c45-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners
```

### <a name="response"></a><span data-ttu-id="e6c45-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6c45-132">Response</span></span>
<span data-ttu-id="e6c45-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6c45-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



