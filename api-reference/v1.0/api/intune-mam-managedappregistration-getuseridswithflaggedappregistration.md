---
title: função getUserIdsWithFlaggedAppRegistration
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b29aa1588c4e5a31481339314fe0e3005ac64faa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513095"
---
# <a name="getuseridswithflaggedappregistration-function"></a><span data-ttu-id="695b6-103">função getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="695b6-103">getUserIdsWithFlaggedAppRegistration function</span></span>

<span data-ttu-id="695b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="695b6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="695b6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="695b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="695b6-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="695b6-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="695b6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="695b6-107">Prerequisites</span></span>
<span data-ttu-id="695b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="695b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="695b6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="695b6-110">Permission type</span></span>|<span data-ttu-id="695b6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="695b6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="695b6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="695b6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="695b6-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="695b6-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="695b6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="695b6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="695b6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="695b6-115">Not supported.</span></span>|
|<span data-ttu-id="695b6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="695b6-116">Application</span></span>|<span data-ttu-id="695b6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="695b6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="695b6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="695b6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

## <a name="request-headers"></a><span data-ttu-id="695b6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="695b6-119">Request headers</span></span>
|<span data-ttu-id="695b6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="695b6-120">Header</span></span>|<span data-ttu-id="695b6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="695b6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="695b6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="695b6-122">Authorization</span></span>|<span data-ttu-id="695b6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="695b6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="695b6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="695b6-124">Accept</span></span>|<span data-ttu-id="695b6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="695b6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="695b6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="695b6-126">Request body</span></span>
<span data-ttu-id="695b6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="695b6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="695b6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="695b6-128">Response</span></span>
<span data-ttu-id="695b6-129">Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="695b6-129">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="695b6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="695b6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="695b6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="695b6-131">Request</span></span>
<span data-ttu-id="695b6-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="695b6-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

### <a name="response"></a><span data-ttu-id="695b6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="695b6-133">Response</span></span>
<span data-ttu-id="695b6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="695b6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": [
    "Get User Ids With Flagged App Registration value"
  ]
}
```




