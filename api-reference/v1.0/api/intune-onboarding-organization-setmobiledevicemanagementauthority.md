---
title: Ação setMobileDeviceManagementAuthority
description: Define uma autoridade de gerenciamento de dispositivo móvel
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 93a8c0c6e3d9f8aa3e02c11550e7b8a920a30701
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582574"
---
# <a name="setmobiledevicemanagementauthority-action"></a><span data-ttu-id="30003-103">ação setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="30003-103">setMobileDeviceManagementAuthority action</span></span>

> <span data-ttu-id="30003-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30003-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30003-105">Define uma autoridade de gerenciamento de dispositivo móvel</span><span class="sxs-lookup"><span data-stu-id="30003-105">Set mobile device management authority</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30003-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="30003-106">Prerequisites</span></span>
<span data-ttu-id="30003-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30003-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30003-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30003-109">Permission type</span></span>|<span data-ttu-id="30003-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="30003-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30003-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30003-111">Delegated (work or school account)</span></span>|<span data-ttu-id="30003-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30003-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="30003-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30003-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30003-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30003-114">Not supported.</span></span>|
|<span data-ttu-id="30003-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30003-115">Application</span></span>|<span data-ttu-id="30003-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30003-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30003-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30003-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/setMobileDeviceManagementAuthority
```

## <a name="request-headers"></a><span data-ttu-id="30003-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30003-118">Request headers</span></span>
|<span data-ttu-id="30003-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30003-119">Header</span></span>|<span data-ttu-id="30003-120">Valor</span><span class="sxs-lookup"><span data-stu-id="30003-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30003-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="30003-121">Authorization</span></span>|<span data-ttu-id="30003-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30003-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30003-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="30003-123">Accept</span></span>|<span data-ttu-id="30003-124">application/json</span><span class="sxs-lookup"><span data-stu-id="30003-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30003-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30003-125">Request body</span></span>
<span data-ttu-id="30003-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="30003-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30003-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="30003-127">Response</span></span>
<span data-ttu-id="30003-128">Se tiver êxito, esta ação retorna o código de resposta `200 OK` e a Int32 no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30003-128">If successful, this action returns a `200 OK` response code and a Int32 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30003-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30003-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="30003-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30003-130">Request</span></span>
<span data-ttu-id="30003-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30003-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/organization/{organizationId}/setMobileDeviceManagementAuthority
```

### <a name="response"></a><span data-ttu-id="30003-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="30003-132">Response</span></span>
<span data-ttu-id="30003-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30003-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 2
}
```



