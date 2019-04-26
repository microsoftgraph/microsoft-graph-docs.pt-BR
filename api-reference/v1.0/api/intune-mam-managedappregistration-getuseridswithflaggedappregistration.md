---
title: função getUserIdsWithFlaggedAppRegistration
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0fb55917b9172fa5836e44a864c1ba41e9e06371
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570845"
---
# <a name="getuseridswithflaggedappregistration-function"></a><span data-ttu-id="96c44-103">função getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="96c44-103">getUserIdsWithFlaggedAppRegistration function</span></span>

> <span data-ttu-id="96c44-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96c44-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96c44-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="96c44-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96c44-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="96c44-106">Prerequisites</span></span>
<span data-ttu-id="96c44-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96c44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96c44-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96c44-109">Permission type</span></span>|<span data-ttu-id="96c44-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="96c44-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96c44-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96c44-111">Delegated (work or school account)</span></span>|<span data-ttu-id="96c44-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="96c44-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="96c44-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96c44-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96c44-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96c44-114">Not supported.</span></span>|
|<span data-ttu-id="96c44-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96c44-115">Application</span></span>|<span data-ttu-id="96c44-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96c44-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96c44-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96c44-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

## <a name="request-headers"></a><span data-ttu-id="96c44-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96c44-118">Request headers</span></span>
|<span data-ttu-id="96c44-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96c44-119">Header</span></span>|<span data-ttu-id="96c44-120">Valor</span><span class="sxs-lookup"><span data-stu-id="96c44-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96c44-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="96c44-121">Authorization</span></span>|<span data-ttu-id="96c44-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96c44-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96c44-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="96c44-123">Accept</span></span>|<span data-ttu-id="96c44-124">application/json</span><span class="sxs-lookup"><span data-stu-id="96c44-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96c44-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96c44-125">Request body</span></span>
<span data-ttu-id="96c44-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="96c44-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96c44-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="96c44-127">Response</span></span>
<span data-ttu-id="96c44-128">Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96c44-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96c44-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96c44-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="96c44-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96c44-130">Request</span></span>
<span data-ttu-id="96c44-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96c44-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

### <a name="response"></a><span data-ttu-id="96c44-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="96c44-132">Response</span></span>
<span data-ttu-id="96c44-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96c44-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



