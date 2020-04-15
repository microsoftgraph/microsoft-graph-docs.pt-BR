---
title: Ação setMobileDeviceManagementAuthority
description: Define uma autoridade de gerenciamento de dispositivo móvel
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 872a9b590aba6150a8d38789b9dea0a5a132281e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452884"
---
# <a name="setmobiledevicemanagementauthority-action"></a><span data-ttu-id="6de6d-103">ação setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="6de6d-103">setMobileDeviceManagementAuthority action</span></span>

<span data-ttu-id="6de6d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6de6d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6de6d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6de6d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6de6d-106">Define uma autoridade de gerenciamento de dispositivo móvel</span><span class="sxs-lookup"><span data-stu-id="6de6d-106">Set mobile device management authority</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6de6d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6de6d-107">Prerequisites</span></span>
<span data-ttu-id="6de6d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6de6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6de6d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6de6d-110">Permission type</span></span>|<span data-ttu-id="6de6d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6de6d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6de6d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6de6d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6de6d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6de6d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6de6d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6de6d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6de6d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6de6d-115">Not supported.</span></span>|
|<span data-ttu-id="6de6d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6de6d-116">Application</span></span>|<span data-ttu-id="6de6d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6de6d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6de6d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6de6d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/setMobileDeviceManagementAuthority
```

## <a name="request-headers"></a><span data-ttu-id="6de6d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6de6d-119">Request headers</span></span>
|<span data-ttu-id="6de6d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6de6d-120">Header</span></span>|<span data-ttu-id="6de6d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6de6d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6de6d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6de6d-122">Authorization</span></span>|<span data-ttu-id="6de6d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6de6d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6de6d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6de6d-124">Accept</span></span>|<span data-ttu-id="6de6d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6de6d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6de6d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6de6d-126">Request body</span></span>
<span data-ttu-id="6de6d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6de6d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6de6d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6de6d-128">Response</span></span>
<span data-ttu-id="6de6d-129">Se tiver êxito, esta ação retorna o código de resposta `200 OK` e a Int32 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6de6d-129">If successful, this action returns a `200 OK` response code and a Int32 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6de6d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6de6d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6de6d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6de6d-131">Request</span></span>
<span data-ttu-id="6de6d-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6de6d-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/organization/{organizationId}/setMobileDeviceManagementAuthority
```

### <a name="response"></a><span data-ttu-id="6de6d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6de6d-133">Response</span></span>
<span data-ttu-id="6de6d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6de6d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 2
}
```






