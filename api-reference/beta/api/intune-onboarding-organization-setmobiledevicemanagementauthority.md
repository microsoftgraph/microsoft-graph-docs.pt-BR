---
title: Ação setMobileDeviceManagementAuthority
description: Define uma autoridade de gerenciamento de dispositivo móvel
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ee33e4aebe35e3a69947377a6da4f190fbfacbb3
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941579"
---
# <a name="setmobiledevicemanagementauthority-action"></a><span data-ttu-id="217ba-103">ação setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="217ba-103">setMobileDeviceManagementAuthority action</span></span>

> <span data-ttu-id="217ba-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="217ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="217ba-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="217ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="217ba-106">Define uma autoridade de gerenciamento de dispositivo móvel</span><span class="sxs-lookup"><span data-stu-id="217ba-106">Set mobile device management authority</span></span>

## <a name="prerequisites"></a><span data-ttu-id="217ba-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="217ba-107">Prerequisites</span></span>
<span data-ttu-id="217ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="217ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="217ba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="217ba-110">Permission type</span></span>|<span data-ttu-id="217ba-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="217ba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="217ba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="217ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="217ba-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="217ba-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="217ba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="217ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="217ba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="217ba-115">Not supported.</span></span>|
|<span data-ttu-id="217ba-116">Application</span><span class="sxs-lookup"><span data-stu-id="217ba-116">Application</span></span>|<span data-ttu-id="217ba-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="217ba-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="217ba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="217ba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/setMobileDeviceManagementAuthority
```

## <a name="request-headers"></a><span data-ttu-id="217ba-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="217ba-119">Request headers</span></span>
|<span data-ttu-id="217ba-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="217ba-120">Header</span></span>|<span data-ttu-id="217ba-121">Valor</span><span class="sxs-lookup"><span data-stu-id="217ba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="217ba-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="217ba-122">Authorization</span></span>|<span data-ttu-id="217ba-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="217ba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="217ba-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="217ba-124">Accept</span></span>|<span data-ttu-id="217ba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="217ba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="217ba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="217ba-126">Request body</span></span>
<span data-ttu-id="217ba-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="217ba-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="217ba-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="217ba-128">Response</span></span>
<span data-ttu-id="217ba-129">Se tiver êxito, esta ação retorna o código de resposta `200 OK` e a Int32 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="217ba-129">If successful, this action returns a `200 OK` response code and a Int32 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="217ba-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="217ba-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="217ba-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="217ba-131">Request</span></span>
<span data-ttu-id="217ba-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="217ba-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/organization/{organizationId}/setMobileDeviceManagementAuthority
```

### <a name="response"></a><span data-ttu-id="217ba-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="217ba-133">Response</span></span>
<span data-ttu-id="217ba-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="217ba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 2
}
```





